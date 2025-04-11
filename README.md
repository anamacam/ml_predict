# Proyecto de Modelo Predictivo ML

Este proyecto implementa una arquitectura para crear un modelo predictivo utilizando Machine Learning.

## Estructura del Proyecto

```
├── data/               # Datos crudos y procesados
│   ├── raw/            # Datos sin procesar
│   └── processed/      # Datos procesados listos para entrenamiento
├── notebooks/          # Jupyter notebooks para exploración y visualización
├── src/                # Código fuente del proyecto
│   ├── data/           # Scripts para procesar datos
│   ├── features/       # Scripts para ingeniería de características
│   ├── models/         # Scripts para entrenar y evaluar modelos
│   └── visualization/  # Scripts para visualización
├── models/             # Modelos entrenados
├── reports/            # Reportes generados
│   └── figures/        # Figuras generadas
├── config/             # Archivos de configuración
└── tests/              # Tests para el código
```

## Configuración

1. Crear un entorno virtual:
```
python -m venv .venv
```

2. Activar el entorno virtual:
- Windows: `.venv\Scripts\activate`
- Unix/MacOS: `source .venv/bin/activate`

3. Instalar dependencias:
```
pip install -r requirements.txt
```

## Uso

1. Preparar datos:
```
python src/data/make_dataset.py
```

2. Entrenar modelo:
```
python src/models/train_model.py
```

3. Realizar predicciones:
```
python src/models/predict_model.py
```

## Seguimiento de Experimentos

El proyecto utiliza MLflow para el seguimiento de experimentos. Para ver los resultados:
```
mlflow ui
``` 