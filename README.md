# telecomx-churn-analysis

# Análisis de Evasión de Clientes – Challenge Telecom X (Parte 1)

Este proyecto corresponde a la primera parte del Challenge "Telecom X", centrado en el análisis exploratorio de datos (EDA) para comprender los factores que influyen en la evasión de clientes (Churn) en una empresa de telecomunicaciones.

## Objetivo

El objetivo principal es identificar patrones, correlaciones y variables relevantes que permitan entender el comportamiento de los clientes y anticipar su abandono, como paso previo al desarrollo de modelos predictivos.

## Herramientas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Estructura del proyecto

- `TelecomX_EDA.ipynb`: Notebook con el análisis exploratorio completo.
- `data/`: Carpeta de datos fuente (archivos CSV).
- `README.md`: Documento descriptivo del proyecto.

## Limpieza y tratamiento de datos

- Unificación de múltiples archivos CSV en un único DataFrame.
- Desanidamiento de columnas agrupadas por secciones (cliente, teléfono, internet, cuenta).
- Conversión de valores binarios ("Yes"/"No") a numéricos.
- Renombramiento de la variable objetivo de `Churn` a `Abandono`.
- Revisión de valores nulos y tipos de datos.
- Eliminación de columnas innecesarias o redundantes.

## Análisis exploratorio de datos

El análisis se realizó sobre variables categóricas y numéricas:

### Variables categóricas

- Género
- Cliente senior
- Tipo de contrato
- Método de pago
- Servicio de internet
- Soporte técnico
- Uso de múltiples líneas

Principales observaciones:
- Los contratos mensuales tienen mayor tasa de abandono.
- El pago manual se asocia a mayor evasión que el pago automático.
- Los clientes con fibra óptica tienden a abandonar más que quienes usan DSL o no tienen internet.

### Variables numéricas

- Tenure (meses como cliente)
- Cargo mensual
- Cargo total

Principales observaciones:
- La evasión es significativamente más alta en los primeros meses.
- Clientes con cargos mensuales altos presentan mayor probabilidad de abandonar.
- Los clientes con mayores cargos totales tienden a permanecer más tiempo.

## Visualizaciones destacadas

- Distribución de abandono general
- Comparación de abandono por categorías
- Boxplots de cargos mensuales y duración del servicio por tipo de cliente
- Curva de tasa de abandono según la duración del contrato

## Conclusiones

- La tasa general de abandono es del 26,6 %.
- El abandono es más común en clientes recientes, con contrato mensual, que pagan manualmente y tienen servicios limitados.
- Las variables más asociadas al abandono son: tipo de contrato, método de pago, servicio de internet y duración del contrato.

## Recomendaciones

- Promover contratos de mayor duración (anual o bianual).
- Incentivar métodos de pago automáticos.
- Enfocar campañas de fidelización en los primeros meses de relación con el cliente.
- Diseñar ofertas que integren múltiples servicios.
- Avanzar hacia la construcción de modelos de machine learning que permitan predecir con mayor precisión la probabilidad de evasión.

