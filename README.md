# Análisis eventos 2025

Proyecto final del Módulo 4 del bootcamp de Análisis de Datos de Adalab.

## Preguntas
1. ¿Cuántas peticiones de evento acaban confirmándose?
2. ¿De qué se compone la facturación de un evento?
3. ¿Cuándo llega la demanda y cuándo se cierra?
4. ¿Influyen los precios del hotel y los congresos de la ciudad?

## Datos

| `eventos_2025.csv`  Peticiones de eventos: ganadas, perdidas y canceladas
| `facturacion_2025.csv`  Ingresos por evento celebrado
| `precios_habs_2025.csv` Precio y ocupación del hotel
| `congresos_2025.csv` Congresos y ferias de Barcelona

## Proceso
1. **Limpieza y EDA** (`PROYECTO_EVENTOS.ipynb`): tratamiento de nulos, conversión
   de tipos y decisiones documentadas sobre los datos.
2. **Unión**: eventos y facturación se cruzan por `id_booking` con `how='outer'`
   para conservar tanto las peticiones perdidas como los eventos dados de alta
   sin booking file.
3. **Dashboard** (Power BI): dos páginas, una sobre el embudo de peticiones y los
   ingresos por evento, y otra sobre el contexto de la ciudad (precios y congresos).

## Principales hallazgos
- **Se confirma menos de 4 de cada 10 peticiones**
- **El alojamiento es el mayor componente de ingresos** 
- **Lo que se gana se pide con poca antelación**
- **La demanda de eventos se concentra en otoño**

## Herramientas
Python (pandas), Jupyter Notebook, Power BI

## Nota sobre privacidad
Los nombres de clientes están sustituidos por códigos y los importes de
facturación escalados. 