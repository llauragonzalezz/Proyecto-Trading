# Proyecto-Trading

## Descripción del Proyecto
Este proyecto implementa una estrategia de pairs trading en componentes seleccionados del Dow Jones. El análisis combina técnicas de clustering jerárquico sobre variables fundamentales con estrategias de trading estadístico (PnL) para identificar oportunidades de mercado.

## Objetivos
- Identificar grupos de empresas similares mediante análisis de clustering
- Implementar una estrategia de pairs trading en pares seleccionados
- Evaluar y comparar el rendimiento de la estrategia entre diferentes pares

## Datos Utilizados
- **fundamentals_dji.csv**: Variables fundamentales de las empresas del DJIA
- Series temporales de precios de las acciones seleccionadas

## Metodología

### 1. Análisis de Clustering
- Preprocesado: eliminación de variables redundantes y selección de representativas
- Implementación de clustering jerárquico
- Identificación de 5 grupos distintos de empresas

### 2. Selección de Pares
Pares seleccionados por cluster:
- UnitedHealth y Amgen
- Visa y Johnson & Johnson
- Apple y Microsoft
- Merck y Disney
- IBM e Intel

### 3. Estrategia de Trading
- Análisis de cointegración con ventanas móviles de 3-5 años
- Selección de períodos óptimos basados en p-valores
- Implementación de señales de trading basadas en z-scores
