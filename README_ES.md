# Análisis de Deuda Pública vs PIB

## Descripción del proyecto
Análisis exploratorio de la deuda pública y el PIB a nivel global mediante Power BI, con el objetivo de comprender la sostenibilidad del endeudamiento a través del ratio Deuda/PIB e identificar economías en situación de riesgo.

El proyecto se materializa en un dashboard interactivo que permite comparar países, analizar patrones globales y segmentar la información por región.

---

## Objetivo
El objetivo principal es analizar la relación entre:

- Deuda pública total  
- Producto Interior Bruto (PIB)  
- Ratio Deuda/PIB  

Para:

- Evaluar la sostenibilidad de la deuda en distintos países  
- Identificar economías con mayor nivel de riesgo  
- Comparar países independientemente de su tamaño económico  

---

## Fuentes de datos
Los datos utilizados proceden de fuentes públicas:

- Deuda pública por país  
- PIB por país (año 2022)  

Fuente: Datosmacro (Expansión)  
Los datos se cargaron en Power BI mediante conexión web con acceso anónimo.

---

## Preparación de datos (Power Query)

### Tabla Deuda Pública
- Eliminación de columnas no relevantes  
- Selección de variables clave:
  - País  
  - Deuda total  
  - Deuda (%PIB)  
  - Deuda per cápita  
- Limpieza de símbolos y separadores  
- Conversión a formato numérico  
- Homogeneización de nombres de países  

### Tabla PIB
- Limpieza del formato del PIB anual  
- Eliminación de errores y valores nulos  
- Homogeneización de nombres de países  

### Enriquecimiento del modelo
- Creación de una tabla auxiliar de países y continentes  
- Relación entre tablas a través del campo país  

---

## Modelo de datos
- Relación entre las tablas de Deuda Pública y PIB por país  
- Inclusión de una dimensión geográfica (continente)  
- Estructura orientada al análisis comparativo  

---

## Métricas clave (DAX)

- Deuda total  
- PIB total  
- Ratio Deuda/PIB  
- Países en riesgo (ratio > 100%)  

Clasificación del riesgo:
- Bajo (< 60%)  
- Medio (60%–100%)  
- Alto (> 100%)  

---

## Funcionalidades del dashboard

### KPIs
- PIB total  
- Deuda total  
- Ratio Deuda/PIB  
- Número de países en riesgo  

### Análisis global
- Mapa por ratio Deuda/PIB  
- Gráfico de dispersión (PIB vs Ratio Deuda/PIB)  
  (el tamaño de la burbuja representa la deuda total)  

### Comparativa
- Top 10 países por:
  - Deuda total  
  - PIB  
  - Ratio Deuda/PIB  

### Segmentación
- Filtros por país y continente  

### Distribución del riesgo
- Visualización de países según nivel de riesgo  

### Funcionalidades avanzadas
- Tooltips personalizados con comparación entre país y promedio del continente  

---

## Insights principales

- Los países con mayor deuda absoluta no son necesariamente los que presentan mayor riesgo  
- El ratio Deuda/PIB es el indicador más relevante para evaluar la sostenibilidad económica  
- Existen economías pequeñas con niveles de endeudamiento elevados en términos relativos  
- La deuda per cápita permite entender mejor la carga sobre la población  
- Se observan patrones diferenciados entre regiones  

---

## Conclusión
El análisis del endeudamiento público requiere ir más allá de los valores absolutos. Incorporar el ratio Deuda/PIB permite contextualizar la deuda en función del tamaño de la economía, ofreciendo una visión más precisa del nivel de riesgo.

El dashboard desarrollado facilita un análisis global y comparativo, permitiendo identificar patrones, outliers y economías en situación de vulnerabilidad de forma clara y estructurada.

---

## Habilidades aplicadas

- Limpieza y transformación de datos (Power Query)  
- Modelado de datos en Power BI  
- Creación de métricas en DAX  
- Diseño de dashboards orientados al análisis  
- Visualización de datos para toma de decisiones  
- Implementación de tooltips personalizados  

---

## Vista del dashboard

<img width="3097" height="1747" alt="image" src="https://github.com/user-attachments/assets/cfaeda20-474f-4d9b-a93c-4f04feea4537" />


---

## Herramientas utilizadas
- Power BI  
- Power Query  
- DAX  
