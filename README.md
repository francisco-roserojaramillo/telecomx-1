# 🚀 Análisis de Evasión de Clientes para Telecom X

### Desafío 2 - Data Science: Explorando las Causas del Churn

Un análisis exploratorio de datos (EDA) para identificar los factores clave que influyen en la cancelación de servicios en una empresa de telecomunicaciones, con el fin de proponer estrategias de retención basadas en datos.

![Estado del Proyecto](https://img.shields.io/badge/Estado-Finalizado-green.svg)

---

### **Índice**
* [Descripción del Proyecto](#-descripción-del-proyecto)
* [Visualización Interactiva](#-visualización-interactiva)
* [Tecnologías y Librerías](#️-tecnologías-y-librerías)
* [Metodología del Análisis](#-metodología-del-análisis)
* [Principales Hallazgos](#-principales-hallazgos)
* [Recomendaciones Estratégicas](#-recomendaciones-estratégicas)
* [Autor](#-autor)

---

### 📝 Descripción del Proyecto

Este proyecto aborda el desafío crítico de la **evasión de clientes (Churn)** en la empresa ficticia **Telecom X**. El objetivo fue realizar un análisis de datos completo para descubrir los patrones y las variables que más influyen en la decisión de un cliente de cancelar su servicio.

El proceso abarcó desde la extracción y transformación de datos en formato JSON anidado, pasando por una limpieza exhaustiva para garantizar la calidad de la información, hasta un análisis exploratorio profundo. El resultado es un informe estratégico que no solo visualiza las tendencias, sino que también ofrece conclusiones claras y recomendaciones accionables para reducir la tasa de cancelación y mejorar la retención de clientes.

---

### 🎨 Visualización Interactiva

Este proyecto fue desarrollado en un notebook de Google Colaboratory. Puedes visualizar y ejecutar el código de forma interactiva directamente en tu navegador haciendo clic en el siguiente botón. El notebook está configurado para cargar los datos directamente desde el repositorio.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TU_USUARIO_DE_GITHUB/NOMBRE_DEL_REPOSITORIO/blob/main/TelecomX_LATAM_challenge2.ipynb)

---

### 🛠️ Tecnologías y Librerías

Para el desarrollo de este análisis se emplearon las siguientes herramientas del ecosistema de Python:

*   **Lenguaje:** Python 3
*   **Entorno:** Google Colaboratory (Jupyter Notebook)
*   **Análisis de Datos:** Pandas
*   **Visualización de Datos:** Matplotlib, Seaborn y Plotly Express

---

### 📈 Metodología del Análisis

El estudio se estructuró siguiendo un proceso de ETL (Extract, Transform, Load) y un posterior Análisis Exploratorio de Datos (EDA), centrado en los siguientes pasos:

1.  **Extracción y Transformación de Datos:**
    *   Carga de datos desde una API en formato JSON.
    *   Aplanamiento de la estructura JSON anidada a un DataFrame tabular.
    *   Limpieza de inconsistencias, como valores vacíos en la columna `Churn` y corrección de tipos de datos en `Charges.Total`.
    *   **Ingeniería de Características** con la creación de la columna `Cuentas_Diarias` para un análisis más granular.
    *   Estandarización de variables categóricas a formato numérico (0/1) para facilitar el análisis cuantitativo.

2.  **Análisis Exploratorio de Datos (EDA):**
    *   **Análisis Descriptivo:** Cálculo de métricas estadísticas para entender la distribución de las variables numéricas.
    *   **Distribución de la Evasión:** Visualización de la proporción de clientes que cancelaron el servicio (26.5%).
    *   **Análisis por Variables Categóricas:** Estudio del comportamiento del Churn en segmentos como tipo de contrato, método de pago y servicios de internet.
    *   **Análisis por Variables Numéricas:** Investigación de la relación entre la evasión y variables como la antigüedad del cliente (`tenure`) y los cargos mensuales.
    *   **Análisis de Correlación:** Identificación de las relaciones más fuertes entre las variables para comprender qué factores están más asociados con el Churn.

---

### 💡 Principales Hallazgos

El análisis reveló un perfil claro de los clientes con mayor probabilidad de abandonar el servicio, destacando los siguientes puntos:

-   **Tipo de Contrato:** Los clientes con **contratos mes a mes** tienen una tasa de cancelación drásticamente superior en comparación con los de contratos anuales o de dos años.
-   **Antigüedad del Cliente (Tenure):** La evasión es **inversamente proporcional** a la antigüedad. La mayoría de las cancelaciones ocurren durante los primeros meses del servicio.
-   **Servicios Adicionales:** Los clientes sin servicios de valor agregado como **Soporte Técnico** y **Seguridad Online** son mucho más propensos a cancelar, lo que sugiere que estos servicios actúan como un factor de retención.
-   **Cargos Mensuales:** Existe una correlación positiva entre los **cargos mensuales elevados** (especialmente en planes de fibra óptica) y una mayor tasa de Churn.
-   **Método de Pago:** El pago mediante **cheque electrónico** está asociado con la tasa de cancelación más alta, lo que podría indicar una menor lealtad o fricciones en la experiencia de pago.

---

### 🎯 Recomendaciones Estratégicas

Basado en la evidencia cuantitativa, se proponen las siguientes acciones para mitigar la evasión de clientes:

1.  **Incentivar Contratos a Largo Plazo:** Crear ofertas y campañas de marketing para motivar a los clientes de planes mes a mes a migrar a contratos de 1 o 2 años, ofreciendo descuentos o beneficios adicionales.
2.  **Fortalecer el Onboarding de Nuevos Clientes:** Implementar un programa de seguimiento proactivo durante los primeros 3 meses para asegurar una experiencia positiva, resolver dudas y reducir la cancelación temprana.
3.  **Promocionar Paquetes de Servicios de Valor Agregado:** Diseñar y promocionar paquetes que incluyan `Seguridad Online` y `Soporte Técnico` a un precio atractivo, comunicando su valor como un diferenciador clave para la retención.
4.  **Optimizar la Estrategia de Precios y Pagos:** Analizar la competitividad de los planes de fibra óptica de mayor costo y simplificar o incentivar métodos de pago automáticos para reducir la fricción asociada con el cheque electrónico.

---

### 👨‍💻 Autor

**Francisco Xavier Rosero Jaramillo**
<br>
*Estudiante en Data Science*
