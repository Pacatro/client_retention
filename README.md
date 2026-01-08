# Retención de Clientes Bancarios

El objetivo es el de desarrollar un modelo predictivo de clasificación binaria para determinar si un cliente bancario abandonará la entidad (variable `Exited`). El modelo se entrena utilizando datos demográficos, financieros y de comportamiento del cliente.

El problema forma parte de una competición de [Kaggle](https://www.kaggle.com/competitions/retencion-de-clientes-de-una-entidad-financiera/data).

## 🎯 Objetivo

Predecir la probabilidad de que un cliente cierre su cuenta bancaria basándose en características como:

- Información demográfica (edad, género, geografía)
- Datos financieros (puntuación crediticia, saldo, productos)
- Comportamiento bancario (antigüedad, membresía activa)

## 📊 Dataset

El conjunto de datos contiene **10,000 registros** divididos en:

- **Entrenamiento**: 8,000 registros (80%)
- **Prueba**: 2,000 registros (20%)

### Características

#### Identificación del Cliente

- `CustomerId`: Identificador único del cliente
- `Surname`: Apellido del cliente

#### Información Financiera

- `CreditScore`: Calificación crediticia (350-850)
- `Balance`: Saldo en cuenta bancaria
- `NumOfProducts`: Número de productos bancarios utilizados
- `HasCrCard`: Posee tarjeta de crédito (0/1)
- `EstimatedSalary`: Salario estimado

#### Información Demográfica y Personal

- `Geography`: País de residencia (Francia, Alemania, España)
- `Gender`: Género (Male/Female)
- `Age`: Edad del cliente (18-92)
- `Tenure`: Años como cliente del banco (0-10)
- `IsActiveMember`: Miembro activo del banco (0/1)

#### Variable Objetivo

- `Exited`: Indicador de abandono del banco (0 = permanece, 1 = abandona)

## 🛠️ Stack Tecnológico

### Librerías Principales

- **[Pandas](https://pandas.pydata.org/)**: Manipulación y análisis de datos
- **[NumPy](https://numpy.org/)**: Cálculos numéricos eficientes
- **[Scikit-learn](https://scikit-learn.org/)**: Machine Learning y preprocesamiento
- **[XGBoost](https://xgboost.readthedocs.io/)**: Algoritmo de gradient boosting
- **[Optuna](https://optuna.org/)**: Optimización de hiperparámetros

### Visualización

- **[Matplotlib](https://matplotlib.org/)**: Gráficos básicos
- **[Seaborn](https://seaborn.pydata.org/)**: Visualización estadística avanzada

### Manejo de Datos Desbalanceados

- **[Imbalanced-learn](https://imbalanced-learn.org/)**: Técnicas para datos imbalanceados (SMOTE)

## 🚀 Uso del Proyecto

### Requisitos Previos

- Python 3.12+
- Gestor de paquetes [uv](https://docs.astral.sh/uv/)

### Instalación

1. Clonar el repositorio

   ```bash
   git clone https://github.com/Pacatro/client_retention.git
   cd client_retention
   ```

2. Instalar dependencias con uv

   ```bash
   uv sync
   ```

3. Activar el entorno virtual

   ```bash
   source .venv/bin/activate # Linux/Mac
   .venv\Scripts\activate   # Windows
   ```

4. Iniciar Jupyter Notebook

   ```bash
   jupyter notebook main.ipynb
   ```
