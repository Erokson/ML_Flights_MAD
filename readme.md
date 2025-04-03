# Proyecto de Machine Learning: Predicción de Pasajeros con Series Temporales

Este proyecto consiste en el desarrollo de un modelo de Machine Learning basado en LSTM (Long Short-Term Memory) para predecir la cantidad de pasajeros que viajan desde/hacia el aeropuerto de Madrid-Barajas a otros destinos. Se trata de un ejercicio completo de predicción con series temporales aplicado a datos reales del sector aeronáutico.

---

## 📅 Objetivo

Predecir el número mensual de pasajeros para diferentes rutas aéreas con origen o destino en Madrid durante el año 2024, usando modelos LSTM entrenados con datos de los 15 años anteriores. Las predicciones se comparan con los valores reales y con un modelo baseline (naïve).

---

## 📂 Estructura del repositorio

```
ML_SeriesTemporales/
│
├── README.md                        # Este documento
├── src/
│   ├── data_sample/
│   │   └── estat_avia_par_es_filtered_en.csv   # Dataset original
│   ├── notebooks/
│   │   └── lstm_series_temporales.ipynb        # Notebook con todo el flujo del proyecto
│   ├── results/
│   │   ├── errores_comparacion_modelos.csv     # MAE y RMSE de LSTM y modelo naive
│   │   ├── predicciones_lstm_2024.csv           # Predicciones LSTM para 2024
│   │   ├── valores_reales_2024.csv              # Datos reales de pasajeros 2024
│   │   └── comparativa_predicciones.png         # Gráfico comparativo LSTM vs naive
```

---

## 📊 Flujo de trabajo

1. **Carga y limpieza de datos:** se filtran las rutas desde/hacia MADRID y se transforman a formato serie temporal.
2. **Filtrado de rutas:** se consideran solo aquellas con más de 10 años de historial.
3. **Preparación para LSTM:** escalado con `MinMaxScaler` y generación de secuencias con `TimeseriesGenerator`.
4. **Entrenamiento del modelo:** LSTM de dos capas con dropout, entrenado hasta 2023.
5. **Predicción de 2024:** usando autoregresión desde la última secuencia de 2023.
6. **Evaluación:** comparación con datos reales de 2024 y modelo naive (que repite el último valor conocido).

---

## 🔹 Ejecución

Desde la carpeta `src/notebooks`, abre y ejecuta `lstm_series_temporales.ipynb`. Asegúrate de tener instaladas las dependencias indicadas en requirements.txt

---

## 📄 Licencia

Uso educativo exclusivamente. Datos de origen público procedentes de Eurostat.

## 👤 Autor

Adrian Gonzalez

---

## 📜 Notas

- Este proyecto es un ejercicio académico y no debe utilizarse para fines comerciales.
- Los datos utilizados son de acceso público y se han utilizado con fines educativos.

---
