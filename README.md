# sprint7-final-project
analisis de telecomunicaciones 
# 📊 Análisis de Comportamiento y Segmentación de Clientes: ConnectaTel

Este proyecto realiza un análisis exploratorio de datos (EDA) y una segmentación estratégica de la base de clientes de la empresa de telecomunicaciones **ConnectaTel**. El objetivo es identificar patrones de uso, detectar valores atípicos y proponer recomendaciones comerciales basadas en el comportamiento de los usuarios.

## 🎯 Objetivos del Proyecto
* **Limpieza de Datos:** Identificar y tratar valores nulos e inconsistencias.
* **Análisis Exploratorio:** Visualizar la distribución de llamadas, mensajes y minutos consumidos.
* **Segmentación:** Clasificar a los usuarios por niveles de uso y rangos de edad.
* **Insight de Negocio:** Detectar oportunidades de upselling y optimización de planes.

## 🛠️ Herramientas Utilizadas
* **Python 3.x**
* **Pandas:** Manipulación y limpieza de datos.
* **NumPy:** Lógica condicional y operaciones matemáticas.
* **Matplotlib & Seaborn:** Visualización de datos (Histogramas, Boxplots y Countplots).

## 📊 Pasos del Análisis

### 1. Limpieza y Calidad de Datos
Se detectó un 2% de valores nulos en la ubicación de los usuarios, los cuales fueron imputados para mantener la integridad del análisis financiero.

### 2. Identificación de Outliers (Valores Atípicos)
Utilizando el **Método IQR**, identificamos usuarios de consumo extremo ("Power Users"). 
* **Decisión:** Se mantuvieron estos registros ya que representan los ingresos más altos por excedentes de la compañía.

### 3. Segmentación Estratégica
Se crearon nuevas dimensiones para el análisis:
* **Grupo de Uso:** Clasificación en `Bajo uso`, `Uso medio` y `Alto uso` según llamadas y mensajes.
* **Grupo de Edad:** Clasificación en `Joven`, `Adulto` y `Adulto Mayor`.

## 📈 Conclusiones Clave (Análisis Ejecutivo)

### ⚠️ Problemas detectados
- **10 registros nulos** en la columna `city`.
- **Presencia de Outliers** en minutos y mensajes que superan el límite superior estadístico.

### 🔍 Hallazgos por Segmento
- **Adultos (30-59 años):** Constituyen el motor principal de la base de clientes.
- **Alto Uso:** Representan la mayor oportunidad de ingresos, pero también el mayor riesgo de fuga (churn) si no se ajustan sus planes.

### 💡 Recomendaciones
1.  **Migración Proactiva:** Incentivar el paso al Plan Premium para usuarios de "Alto Uso".
2.  **Plan Intermedio:** Crear una oferta para cerrar la brecha entre el Plan Básico y el Premium.
3.  **Personalización:** Ajustar beneficios según el grupo de edad (más datos para jóvenes, más voz para adultos mayores).

## 🚀 Cómo ejecutar el proyecto
1. Clonar el repositorio: `git clone https://github.com/tu-usuario/connectatel-analysis.git`
2. Instalar dependencias: `pip install pandas seaborn matplotlib numpy`
3. Ejecutar el Jupyter Notebook: `jupyter notebook ConnectaTel_Analysis.ipynb`

---
Desarrollado como parte del análisis estratégico de ConnectaTel.
