# Feature Specification

## Title
<!-- Short, descriptive name -->
Filtrar por estación

## Status
<!-- Draft | In Progress | Review | Done -->

## Description
La función deberá obtener la estación y el los productos en ella, los productos quedarán agrupados por estación, de modo que el operario podra:

    - Obtener una estación especifica usando para ello un deplegable donde se muestren todas las estaciones o escribir el nombre de una estación especifica

    - Por defecto siempre se devolverá una lista completa de las estaciones y sus productos

    - En caso de solo fitrar por una o x estaciones se devolverá una lista con las estaciones seleccionadas y su stock.

    - Siempre que se muestren los productos se mostrará:
        - Stock actual del producto

## User Stories
- Como [operario], quiero [filtrar] para obtener una [lista de estaciones y sus productos]
- Como [operario], quiero poder [elegir una o ver todas] para tener [información] del stock por estación.

## Acceptance Criteria
- [ ] La función puede concetarse a la API
- [ ] La consulta a la API es exitosa
- [ ] La función devuelve exclusivamente la información pedida en la descripción
- [ ] La función solo se encarga de lo pedido y usa otras funciones para obtener lo necesario


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
