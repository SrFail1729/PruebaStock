# Feature Specification

## Title
<!-- Short, descriptive name -->
Modificar stock manual

## Status
<!-- Draft | In Progress | Review | Done -->
Draft

## Description
<!-- What is this feature? Why do we need it? -->
El operario modificará el stock de calquier producto (vinos o destilados) en cualquier estación. Se usará para registrar y modificar el stock para entradas, salidas, correcciones u otros movimientos no generados por ventas.

El operario deberá rellenar un FORM con que contará con:
    - Campo no obligatorio: 
        - Activo
        - Inactivo

    (En caso de no especificarse campo, quedará marcado como su estado anterior)

    - Campos autorrellenados:
        - Fecha y hora del sistema.
        - Usuario
    
    - Campos obligatorios: 
        -Entrada o Salida
        - Producto
        - Estación
        - Cantidad
        - Motivo (texto libre)


Comportamiento:
    - Distinición entre entrada(suma stock) y salida (resta stock)
    - Si uno de los campos obligatorios no esta relleno es decir esta vacio, no se procederá a enviar la petición de stock.
    - Si la Api de GoGuest falla, no se registrará el cambio manual de stock y se avisará al operario.
    - Si la Api devuelve un OK, se guardará un registro en BD para crear un historico.


## Acceptance Criteria
- [ ] La función puede comunicarse con la API de GoGuest
- [ ] La función maneja apropiadamente los errores de la API e informa al usuario sin romper la aplicación.
- [ ] La función solo ejecturará la llamada a la Api de GoGuest si los campos obligatorios han sido previamente llenado.
- [ ] La función solo guardará el FORM en base de datos si la API de GoGuest devuelve un OK.
- [ ]La función solo se encargará de la lógica definida, cualquier otra cosa que necesite será accedida mediante otras funciones.
- [ ] La función devolverá solo lo un mensaje de confirmación o un mensaje informando del error. Guardar en Base de dato u otras cosas son transparentes para el usuario.

## Technical Details

### Files to Create/Modify
| File | Action | Description |
|------|--------|-------------|
| `path/to/file.ts` | Create | Brief description |
| `path/to/file.ts` | Modify | Brief description |

### Dependencies
- New packages needed (if any):
- Existing packages to use:

### Data Models
<!-- Types, interfaces, database schemas -->

### API Changes
<!-- New endpoints, request/response shapes -->

## Edge Cases
- What can go wrong?
- How should it be handled?

## Testing Plan
- Unit tests needed:
- Integration tests needed:
- Manual test steps:

## Notes for Agent
<!-- Specific instructions, preferences, or constraints for the AI agent -->
- Si debes acceder a otro fichero para leerlo porque necesitas una función o información no alteres el documento, solo accederás a el en modo LECTURA.
- Leer ./agents/conventions.md antes de empezar a crear código.
- Antes de dar por finalizado el desarrollo debes leer ./agents/quality/code-review.md y pasarlo completamente
- Los erroes de la api deben tratarse apropiadamente, la webapp no puede dejar de funcionar.