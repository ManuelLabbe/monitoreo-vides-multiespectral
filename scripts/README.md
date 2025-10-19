# Scripts

Este directorio contiene scripts ejecutables de alto nivel para operaciones comunes.

## Propósito:
Scripts CLI para ejecutar tareas comunes del proyecto sin necesidad de escribir código.

## Ejemplos de scripts:
- `train.py` - Entrenar un modelo con configuración específica
- `evaluate.py` - Evaluar un modelo entrenado
- `predict.py` - Realizar predicciones con un modelo
- `preprocess_data.py` - Preprocesar datos
- `export_model.py` - Exportar modelo para producción

## Uso:
```bash
python scripts/train.py --config configs/model_config.yaml
python scripts/evaluate.py --model_path models/best_model.pth
python scripts/predict.py --image path/to/image.jpg
```

## Convenciones:
- Usar argparse o click para CLI arguments
- Incluir help messages descriptivos
- Validar inputs antes de procesamiento
- Logging claro de progreso y errores
