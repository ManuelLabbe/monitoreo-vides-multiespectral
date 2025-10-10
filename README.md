# monitoreo-vides-multiespectral

Este proyecto desarrolla un sistema de visión multiespectral virtual basado en inteligencia artificial para el monitoreo temprano de la salud en vides. Busca detectar enfermedades como la Botrytis cinerea y el estrés en los cultivos, superando las limitaciones de la inspección visual tradicional.

## Estructura del Proyecto

```
monitoreo-vides-multiespectral/
├── data/                   # Datasets (raw, processed, external)
├── notebooks/              # Jupyter notebooks para exploración y experimentación
├── configs/                # Archivos de configuración (YAML, JSON, etc.)
├── src/                    # Código fuente principal
│   ├── data_processing/    # Procesamiento y transformación de datos
│   ├── models/             # Definiciones de modelos y arquitecturas
│   ├── training/           # Lógica de entrenamiento y evaluación
│   ├── deployment/         # Código para deployment y API
│   └── utils/              # Utilidades y funciones auxiliares
├── scripts/                # Scripts ejecutables de alto nivel
└── tests/                  # Tests unitarios e integrales
```

### Descripción de Carpetas

- **data/**: Contiene los datasets utilizados en el proyecto. Ver [data/README.md](data/README.md) para más detalles.
- **notebooks/**: Jupyter notebooks para análisis exploratorio, experimentación y visualizaciones.
- **configs/**: Archivos de configuración para modelos, entrenamiento y deployment.
- **src/**: Código fuente principal del proyecto, organizado en módulos.
  - **data_processing/**: Carga, limpieza y preprocesamiento de datos.
  - **models/**: Arquitecturas de modelos y capas personalizadas.
  - **training/**: Pipelines de entrenamiento, métricas y callbacks.
  - **deployment/**: APIs, inferencia y monitoreo en producción.
  - **utils/**: Funciones auxiliares, logging y validación.
- **scripts/**: Scripts CLI para ejecutar tareas comunes (entrenar, evaluar, predecir).
- **tests/**: Pruebas unitarias e integrales del proyecto.

## Instalación

```bash
# Clonar el repositorio
git clone https://github.com/ManuelLabbe/monitoreo-vides-multiespectral.git
cd monitoreo-vides-multiespectral

# Crear entorno virtual (recomendado)
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# Instalar dependencias (cuando estén definidas)
# pip install -r requirements.txt
```

## Uso

```bash
# Entrenar un modelo
python scripts/train.py --config configs/model_config.yaml

# Evaluar un modelo
python scripts/evaluate.py --model_path models/best_model.pth

# Realizar predicciones
python scripts/predict.py --image path/to/image.jpg
```

## Contribuir

Por favor, sigue las convenciones de código del proyecto y asegúrate de que todos los tests pasen antes de crear un pull request.

```bash
# Ejecutar tests
pytest tests/

# Ejecutar tests con coverage
pytest --cov=src tests/
```

## Licencia

[Especificar licencia]
