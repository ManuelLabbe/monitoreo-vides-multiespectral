# Tests

Este directorio contiene las pruebas unitarias e integrales del proyecto.

## Estructura:
Debe reflejar la estructura de `src/`:
- `test_data_processing/` - Tests para data_processing
- `test_models/` - Tests para models
- `test_training/` - Tests para training
- `test_deployment/` - Tests para deployment
- `test_utils/` - Tests para utils

## Framework:
- **pytest** (recomendado para Python)

## Convenciones:
- Archivos de test deben comenzar con `test_`
- Funciones de test deben comenzar con `test_`
- Usar fixtures para setup/teardown
- Incluir tests unitarios e integrales
- Mantener alta cobertura de código

## Ejecución:
```bash
# Ejecutar todos los tests
pytest tests/

# Ejecutar tests específicos
pytest tests/test_data_processing/

# Con coverage
pytest --cov=src tests/
```

## Tipos de tests:
- **Unitarios**: Testear funciones individuales
- **Integración**: Testear flujos completos
- **End-to-end**: Testear pipeline completo
