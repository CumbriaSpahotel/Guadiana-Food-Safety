# 📋 Registro de Versiones y Control de Cambios - Food Safety · Hotel Guadiana

Este documento es el registro oficial de versiones del sistema **Food Safety (Plan de Gestión de Alérgenos y Seguridad Alimentaria)** del Hotel Guadiana.

---

## 🚀 Versión Global del Sistema

| Sistema | Versión Actual | Última Actualización | Estado |
| :--- | :---: | :---: | :---: |
| **Food Safety · Hotel Guadiana** | **`v1.0.0`** | **27/10/2026** | **Operativo** |

> ⚠️ **Regla de Mantenimiento (Versión Única Global):**  
> Existe **una única versión para todo el sistema**.  
> Cada vez que realicemos una modificación en **cualquier módulo, pantalla, componente, base de datos o lógica del sistema**:
> 1. Se **incrementará el número de versión global** del sistema (`vX.Y.Z`).
> 2. Se **actualizará la fecha de actualización** en este registro.
> 3. Se registrará la entrada correspondiente en el **Historial de Modificaciones**, detallando el módulo afectado y los cambios realizados.

---

## 📦 Módulos Integrados en el Sistema

Todos los módulos comparten la misma versión global del sistema:

| Módulo | Archivos Principales | Responsabilidad / Descripción |
| :--- | :--- | :--- |
| **Núcleo & Autenticación** | [`src/App.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/App.tsx), [`src/main.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/main.tsx) | Control de sesión con Supabase Auth, control de acceso por roles (RBAC) y notificaciones toast. |
| **Estructura y Navegación** | [`src/components/Layout.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/Layout.tsx) | Navegación lateral, cabecera corporativa, perfil de usuario activo y responsive layout. |
| **Panel de Inicio (Dashboard)** | [`src/components/Dashboard.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/Dashboard.tsx) | Indicadores clave (KPIs), métricas de alérgenos, proveedores y tareas sanitarias. |
| **Catálogo de Alérgenos & Platos** | [`src/components/FoodItemsTable.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/FoodItemsTable.tsx), [`src/components/FoodItemForm.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/FoodItemForm.tsx), [`src/utils/allergens.ts`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/utils/allergens.ts) | Fichas de elaboraciones, declaración de los 14 alérgenos oficiales y trazas, filtros y estados de validación. |
| **Dossier Sanidad & Auditoría** | [`src/components/AuditPanel.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/AuditPanel.tsx) | Informe oficial para inspección sanitaria, trazabilidad de cambios y formato de impresión PDF. |
| **Gestión de Proveedores** | [`src/components/SuppliersTable.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/SuppliersTable.tsx), [`src/components/SupplierForm.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/SupplierForm.tsx) | Registro de proveedores homologados y verificación de fichas técnicas sanitarias. |
| **Control de Tareas Sanitarias** | [`src/components/TasksPanel.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/TasksPanel.tsx) | Seguimiento y asignación de tareas operativas de seguridad alimentaria para cocina y sala. |
| **Usuarios & Permisos (RBAC)** | [`src/components/UsersPanel.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/UsersPanel.tsx) | Gestión de cuentas de usuario y asignación de roles (`admin`, `gestor`, `cocina`, `sala`, `consulta`). |
| **Importación / Exportación** | [`src/components/ImportExportPanel.tsx`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/components/ImportExportPanel.tsx) | Respaldo y carga masiva de datos en formato JSON y CSV. |
| **Base de Datos & Supabase** | [`src/utils/supabase.ts`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/utils/supabase.ts), [`supabase/schema.sql`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/supabase/schema.sql) | Cliente Supabase, esquemas de tablas, políticas RLS y logs de auditoría en PostgreSQL. |
| **Estilos & Impresión Sanitaria** | [`src/styles/app.css`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/src/styles/app.css) | Hojas de estilo y reglas `@media print` para exportación oficial de documentos. |

---

## 📝 Historial Detallado de Versiones

### [v1.0.0] - 27/10/2026
- **Línea Base del Sistema (Versión Única Global)**:
  - Unificación de todo el sistema bajo una única versión global `v1.0.0`.
  - Establecimiento de la norma de versionado unificado: cualquier modificación en cualquier módulo incrementa la versión global del sistema y su fecha de actualización en este registro.
  - Creación del documento [`REGISTRO_VERSIONES.md`](file:///c:/Users/comun/Documents/GitHub/Guadiana-Food-Safety/REGISTRO_VERSIONES.md).

---

## 🏷️ Criterio de Versionado Global (SemVer)

La versión única global del sistema sigue la convención `vX.Y.Z`:
- **`X` (Versión Mayor)**: Cambios estructurales completos, rediseños globales o modificaciones incompatibles en la base de datos o arquitectura.
- **`Y` (Versión Menor)**: Incorporación de nuevos módulos, nuevas herramientas o ampliaciones funcionales en cualquier parte del sistema.
- **`Z` (Parche / Corrección)**: Ajustes puntuales, resolución de errores (bugs), optimizaciones visuales, cambios de texto o correcciones en cualquier módulo.
