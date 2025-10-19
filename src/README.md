# Source Code (src)

Este directorio contiene el código fuente principal del proyecto.

## Estructura de módulos:

### `data_processing/`
Módulos para procesamiento y transformación de datos:
- Carga de datos
- Limpieza y preprocesamiento
- Transformaciones de features
- Data augmentation

### `models/`
Definiciones de arquitecturas de modelos:
- Definición de modelos
- Capas personalizadas
- Arquitecturas de redes neuronales

### `training/`
Lógica de entrenamiento de modelos:
- Pipelines de entrenamiento
- Callbacks y métricas
- Validación y evaluación
- Manejo de experimentos

### `deployment/`
Código para despliegue de modelos:
- API endpoints
- Serialización de modelos
- Inferencia
- Monitoreo de producción

### `utils/`
Utilidades y funciones auxiliares:
- Helpers generales
- Logging
- Validación
- Configuración

## Convenciones:
- Cada módulo debe tener su propio `__init__.py`
- Usar docstrings para documentar funciones y clases
- Seguir PEP 8 para estilo de código Python
