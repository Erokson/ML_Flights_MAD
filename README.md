
# 📊 Modelización y Predicción de Pasajeros en el Aeropuerto de Madrid

## Descripción

Este proyecto analiza series temporales del volumen mensual de pasajeros en el Aeropuerto Adolfo Suárez Madrid-Barajas. Se aplican técnicas de análisis exploratorio de datos (EDA) y modelos de predicción como Naive, ARIMA, SARIMA y SARIMAX para prever la demanda de pasajeros y apoyar la planificación operativa del aeropuerto.

## Estructura del Proyecto

- `src/`: Contiene los notebooks y scripts principales.
- `requirements.txt`: Lista de dependencias necesarias para ejecutar el proyecto.

## Instalación

```bash
git clone https://github.com/Erokson/ML_Flights_MAD.git
cd ML_Flights_MAD
python -m venv env
source env/bin/activate  # En Windows: env\Scripts\activate
pip install -r requirements.txt
```

## Uso

Ejecuta los notebooks en el directorio `src/` para:

- Realizar EDA y visualizar tendencias estacionales.
- Evaluar la estacionariedad de la serie temporal.
- Entrenar y comparar modelos de predicción.
- Generar gráficos de predicciones y errores.

## Resultados

El modelo SARIMA (manual) mostró el mejor rendimiento con los siguientes errores:

- MAE: 232,495.71
- RMSE: 273,393.69

Esto indica que capturar explícitamente la estacionalidad mejora significativamente la precisión de las predicciones.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para discutir cambios o mejoras.

## Licencia

Este proyecto está bajo la Licencia MIT.


# 📊 Passenger Modeling and Forecasting at Madrid Airport

## Description

This project analyzes time series data of monthly passenger volumes at Adolfo Suárez Madrid-Barajas Airport. It applies exploratory data analysis (EDA) techniques and forecasting models such as Naive, ARIMA, SARIMA, and SARIMAX to predict passenger demand and support airport operational planning.

## Project Structure

- `src/`: Contains the main notebooks and scripts.
- `requirements.txt`: Lists the dependencies required to run the project.

## Installation

```bash
git clone https://github.com/Erokson/ML_Flights_MAD.git
cd ML_Flights_MAD
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
pip install -r requirements.txt
```

## Usage

Run the notebooks in the `src/` directory to:

- Perform EDA and visualize seasonal trends.
- Evaluate the stationarity of the time series.
- Train and compare forecasting models.
- Generate prediction and error plots.

## Results

The manual SARIMA model demonstrated the best performance with the following errors:

- MAE: 232,495.71
- RMSE: 273,393.69

This indicates that explicitly capturing seasonality significantly improves prediction accuracy.

## Contributions

Contributions are welcome. Please open an issue or a pull request to discuss changes or improvements.

## License

This project is licensed under the MIT License.
