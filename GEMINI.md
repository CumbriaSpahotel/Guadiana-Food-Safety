# Reglas del Proyecto (Food Safety · Hotel Guadiana)

## Control de Versiones Obligatorio y Automático (Versión Única Global)

Existe **una única versión global para todo el sistema Food Safety**, compartida por todos los módulos.

### Protocolo de Automatización Obligatorio:
Cada vez que se realice cualquier modificación, mejora, corrección o ampliación en cualquier archivo del sistema (`src/App.tsx`, componentes en `src/components/`, `supabase/`, estilos `src/styles/`, utilidades, etc.), el asistente **DEBE ACTUALIZAR AUTOMÁTICAMENTE Y DE MANERA INMEDIATA** (sin necesidad de que el usuario lo recuerde ni lo solicite expresamente):

1. **Número de Versión Global**: Incrementar la versión en [`REGISTRO_VERSIONES.md`](REGISTRO_VERSIONES.md) siguiendo SemVer:
   - **Parche (`+0.0.1`)**: Corrección de errores (bugs), ajustes de estilo visual, textos, pequeñas optimizaciones o validaciones.
   - **Menor (`+0.1.0`)**: Nuevas funcionalidades, nuevos componentes, vistas o módulos añadidos al sistema.
   - **Mayor (`+1.0.0`)**: Cambios estructurales mayores, rediseños globales o modificaciones incompatibles en el modelo de datos.
2. **Fecha de Actualización**: Registrar la fecha actual en formato `DD/MM/AAAA`.
3. **Registro Oficial ([`REGISTRO_VERSIONES.md`](REGISTRO_VERSIONES.md))**:
   - Actualizar la tabla de estado principal con la nueva versión global y fecha.
   - Añadir una nueva entrada en el **Historial Detallado de Versiones** detallando:
     - Versión y fecha (`[vX.Y.Z] - DD/MM/AAAA`).
     - Módulo(s) y archivo(s) intervenidos.
     - Resumen claro y conciso de la mejora implementada.
4. **Sincronización en `package.json`**:
   - Mantener el campo `"version": "X.Y.Z"` de [`package.json`](package.json) sincronizado con la versión global del sistema.
