# Reducción de Dimensionalidad y Agrupamiento con SVD: Análisis Educativo

Este repositorio documenta un proyecto de aprendizaje no supervisado enfocado en el análisis y agrupamiento de estudiantes según sus calificaciones en distintas asignaturas. Se utiliza descomposición SVD para reducir la dimensionalidad, evaluar errores de reconstrucción y analizar agrupamientos generados a partir de las proyecciones.

## Objetivo

Aplicar técnicas de reducción de dimensionalidad con SVD para interpretar la estructura interna de datos académicos, evaluar la precisión de las reconstrucciones y explorar agrupamientos significativos entre estudiantes.

## Flujo de trabajo

### 1. Preprocesamiento
- Estandarización de datos con `StandardScaler`
- Separación de matriz de características y construcción de matrices SVD: U, Σ, Vᵗ

### 2. Reducción y proyección
- Implementación de función para proyectar datos en 2D y 3D
- Visualización de observaciones en ambas dimensiones
- Identificación visual de agrupamientos

### 3. Análisis de error
- Cálculo de errores individuales y totales para cada proyección
- Comparación de errores entre 2D y 3D
- Diagramas de caja para representar la distribución del error por asignatura

### 4. Agrupamiento e interpretación
- Detección de grupos de estudiantes con comportamiento similar
- Identificación de casos atípicos con base en la distancia al centroide
- Comparación con resultados obtenidos por PCA para validar interpretaciones

## Herramientas utilizadas

- Python 3.x  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

## Conclusiones

- La proyección 3D reduce mejor el error de reconstrucción que la 2D.
- SVD permite simplificar la información sin perder patrones importantes.
- Se identificaron agrupamientos significativos entre estudiantes según rendimiento.
- La comparación con PCA refuerza la utilidad de SVD en análisis exploratorios.
