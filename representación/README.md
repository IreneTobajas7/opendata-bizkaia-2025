# Propuesta: Representación Dinámica de Datos
## Deporte Escolar en Bizkaia - Explorador Interactivo

**Categoría:** Representación dinámica de datos  
**Concurso:** Reto del Periodismo de Datos - Open Data Bizkaia  
**Plazo de presentación:** 3 de noviembre - 3 de diciembre de 2025  
**Fecha de elaboración:** Diciembre 2024

---

## RESUMEN EJECUTIVO

### Título del Proyecto
**"Explorador de datos: Deporte escolar en Bizkaia"**

### Objetivo
Crear una visualización interactiva y dinámica que permita a los usuarios explorar los datos del deporte escolar de Bizkaia desde múltiples perspectivas. A diferencia del reportaje narrativo, este dashboard pone el poder de exploración en manos del usuario, permitiendo descubrir patrones, hacer comparaciones y filtrar información según sus intereses.

### Concepto Central
Un dashboard web interactivo con múltiples visualizaciones vinculadas (cross-filtering) que permite:
- Explorar la evolución temporal de la participación
- Analizar la distribución por género en diferentes deportes
- Identificar patrones de paridad o desequilibrio
- Filtrar y comparar datos por temporada, deporte y género
- Visualizar tendencias y crecimiento comparativo

---

## ESTRUCTURA DEL DASHBOARD

### 1. Panel de Controles (Superior)
- **Filtro de temporada**: Seleccionar una temporada específica o "todas"
- **Filtro de deporte**: Filtrar por deporte específico o ver todos
- **Filtro de mínimo participantes**: Deslizador para filtrar deportes por volumen
- **Filtro de género**: Enfocar en participación femenina o masculina
- **Botón reset**: Restablecer todos los filtros

### 2. Métricas Resumen (Panel superior)
- Total de participantes (según filtros)
- Porcentaje de participación femenina
- Número de deportes activos
- Ratio Femenino/Masculino

### 3. Visualizaciones Principales

#### a) Evolución Temporal (Línea)
- Tendencias de participación por género a lo largo de las temporadas
- Permite ver el impacto de la pandemia y la recuperación posterior
- Interactiva con tooltips detallados

#### b) Distribución por Género (Doughnut)
- Vista de la proporción general de participación
- Actualiza según los filtros aplicados
- Incluye porcentajes y valores absolutos

#### c) Top 10 Deportes (Barras apiladas horizontales)
- Los 10 deportes con mayor participación en la temporada seleccionada
- Desglose por género en cada barra
- Se actualiza dinámicamente según filtros

#### d) Mapa de Paridad (Scatter plot)
- Relación entre participación masculina (eje X) y femenina (eje Y)
- Zona sombreada indica deportes con paridad (45-55% femenino)
- Tamaño de burbuja proporcional al total de participantes
- Color indica nivel de equilibrio:
  - Naranja: <30% femenino
  - Verde medio: 30-60% femenino
  - Verde oscuro: >60% femenino
- **Interactivo**: Click en un punto para destacar un deporte específico

#### e) Ratio de Género por Deporte (Barras horizontales)
- Deportes ordenados por porcentaje de participación femenina
- Línea vertical punteada marca la paridad (50%)
- Color coding para identificar desequilibrios
- Limita a 20 deportes principales para legibilidad

#### f) Comparativa de Crecimiento (Barras agrupadas)
- Tasa de crecimiento desde 2018-2019 por género
- Permite comparar el ritmo de crecimiento entre géneros

---

## CRITERIOS DE EVALUACIÓN

### 1. Claridad Comunicativa (30%)

**Estrategias implementadas:**
- **Métricas resumen prominentes**: Los usuarios ven inmediatamente los números clave
- **Títulos y descripciones claras**: Cada visualización incluye un título y una breve descripción
- **Leyendas y etiquetas explícitas**: Todas las visualizaciones incluyen leyendas claras
- **Tooltips informativos**: Al pasar el cursor, los usuarios obtienen información detallada
- **Color coding consistente**: Verde para femenino, naranja para masculino en todo el dashboard
- **Zona de paridad visible**: En el mapa de paridad, la zona objetivo está claramente marcada

**Principio de Knaflic aplicado**: *"Think like a designer"* - Cada elemento visual tiene un propósito comunicativo claro.

### 2. Interactividad (25%)

**Funcionalidades implementadas:**
- **Filtros dinámicos**: Todos los filtros actualizan todas las visualizaciones en tiempo real
- **Cross-filtering**: Cuando se selecciona un deporte en el mapa de paridad, todas las demás visualizaciones se ajustan
- **Tooltips interactivos**: Información detallada al pasar el cursor sobre los elementos
- **Selección de puntos**: Click en el scatter plot para destacar un deporte específico
- **Botón reset**: Facilita explorar diferentes escenarios

**Principio de Knaflic aplicado**: *"Understand the context"* - Los filtros permiten al usuario entender diferentes contextos y perspectivas.

### 3. Diseño y Usabilidad (20%)

**Características de diseño:**
- **Layout responsive**: Se adapta a diferentes tamaños de pantalla (móvil, tablet, desktop)
- **Grid system flexible**: Visualizaciones organizadas en grid adaptativo
- **Branding consistente**: Usa la misma paleta de colores que el reportaje (#00534c, #c96a12)
- **Tipografía clara**: Fuente Aptos Regular como en el reportaje
- **Espaciado coherente**: Padding y márgenes consistentes
- **Estados visuales**: Hover effects en las tarjetas de visualización
- **Navegación intuitiva**: Panel de controles siempre visible y accesible

**Principio de Knaflic aplicado**: *"Choose an effective visual"* - Cada tipo de gráfico se selecciona por su capacidad de comunicar el mensaje específico.

### 4. Originalidad en la Representación (15%)

**Elementos innovadores:**
- **Mapa de paridad interactivo**: Scatter plot con zona de paridad sombreada permite identificar visualmente los deportes equilibrados
- **Cross-filtering completo**: Todas las visualizaciones están vinculadas, algo no siempre visto en dashboards
- **Línea de paridad en gráfico de barras**: Referencia visual constante de lo que significa equilibrio
- **Métricas resumen que se actualizan**: Dashboard "vivo" que responde a las interacciones del usuario
- **Combinación de múltiples tipos de gráficos**: Líneas, barras, scatter, doughnut trabajando juntos coherentemente

**Inspiración Tableau**: Inspirado en dashboards de Tableau que permiten exploración profunda de datos con múltiples vistas sincronizadas.

### 5. Rigor y Fidelidad de los Datos (10%)

**Garantías de precisión:**
- **Datos directos de Open Data Bizkaia**: Todos los datos provienen de fuentes oficiales
- **Sin transformaciones que distorsionen**: Los cálculos son transparentes (sumas, porcentajes, ratios)
- **Manejo explícito de valores nulos**: Los datos vacíos o cero se manejan apropiadamente
- **Metodología documentada**: Se incluye referencia a las fuentes de datos
- **Verificación cruzada**: Los totales y porcentajes se calculan sobre los mismos datos base

**Transparencia**: Footer incluye referencia a las fuentes de datos oficiales.

---

## PRINCIPIOS DE KNAFLIC APLICADOS

### 1. Understand the Context
- Los usuarios pueden explorar diferentes contextos (temporadas, deportes, géneros)
- Los filtros permiten cambiar el contexto fácilmente
- Las métricas resumen proporcionan contexto inmediato

### 2. Choose an Appropriate Visual Display
- **Líneas**: Para evolución temporal (tiempo es continuo)
- **Doughnut**: Para proporciones (género es categórico)
- **Barras apiladas**: Para comparar totales y componentes (deportes y género)
- **Scatter plot**: Para relaciones bidimensionales (masculino vs femenino)
- **Barras horizontales**: Para rankings largos (ratio por deporte)

### 3. Eliminate Clutter
- Solo elementos esenciales en cada visualización
- Grids sutiles, no distractores
- Leyendas solo cuando son necesarias
- Espaciado generoso entre elementos

### 4. Focus Attention Where You Want It
- Color branding para los datos de género
- Zona de paridad destacada en el scatter plot
- Línea de paridad en el gráfico de ratio
- Métricas resumen en posición prominente

### 5. Think Like a Designer
- Consistencia visual en toda la interfaz
- Jerarquía visual clara (títulos, descripciones, gráficos)
- Balance entre información y espacio en blanco
- Transiciones suaves en las actualizaciones

### 6. Tell a Story
- El dashboard permite que cada usuario cree su propia historia
- La estructura guía hacia descubrimientos (evolución → distribución → detalles)
- Los filtros permiten explorar diferentes narrativas

---

## INSPIRACIÓN Y REFERENCIAS

### Tableau Dashboard Showcase
- **Multi-view dashboards**: Inspiración en dashboards que combinan múltiples vistas
- **Cross-filtering**: Efecto de selección en una vista que filtra otras vistas
- **Action-oriented design**: Controles claros que invitan a la interacción

### Buenas Prácticas Aplicadas
1. **Progressive disclosure**: Información detallada en tooltips, no sobrecargar la vista principal
2. **Feedback inmediato**: Los cambios de filtro se reflejan instantáneamente
3. **Estado visible**: Los filtros activos son claramente visibles
4. **Exploración guiada**: Estructura que sugiere un flujo de exploración natural

---

## TECNOLOGÍAS UTILIZADAS

- **HTML5/CSS3**: Estructura y estilos
- **JavaScript (ES6+)**: Lógica de interacción
- **Chart.js 4.4.4**: Librería de visualización
- **Chart.js Plugin Datalabels**: Etiquetas en gráficos
- **Fetch API**: Carga asíncrona de datos JSON/CSV

### Ventajas de esta stack:
- **Ligero**: Sin dependencias pesadas
- **Responsive**: Funciona en todos los dispositivos
- **Accesible**: HTML semántico
- **Mantenible**: Código modular y documentado

---

## COMPLEMENTARIEDAD CON EL REPORTAGE

Esta propuesta complementa perfectamente el reportaje narrativo:

### Reportaje ("Reportaje + Datos")
- **Enfoque**: Narrativa guiada, historia contada
- **Objetivo**: Educar y concienciar
- **Formato**: Scroll narrativo con visualizaciones integradas
- **Audiencia**: Lectores que buscan entender la historia completa

### Dashboard ("Representación dinámica de datos")
- **Enfoque**: Exploración libre, descubrimiento
- **Objetivo**: Permitir análisis personalizado
- **Formato**: Múltiples vistas interactivas sincronizadas
- **Audiencia**: Usuarios que quieren explorar los datos por sí mismos

### Sinergia
- El reportaje presenta la narrativa y los hallazgos clave
- El dashboard permite profundizar en los datos
- Ambos comparten la misma paleta de colores y branding
- Se enlazan entre sí para ofrecer una experiencia completa

---

## ESTRUCTURA DE ARCHIVOS

```
representación_dinámica_new/
├── index.html              # Página principal del dashboard
├── dashboard.js            # Lógica JavaScript principal
├── data/                   # Datos procesados
│   ├── evolucion_temporal.json
│   ├── evolucion_por_deporte.csv
│   └── resumen_deportes.json
├── README.md              # Esta documentación
└── PROPUESTA_TECNICA.md   # Documentación técnica detallada
```

---

## USO Y NAVEGACIÓN

### Flujo recomendado de exploración:

1. **Vista general**: Observar las métricas resumen y la evolución temporal
2. **Filtrar por temporada**: Ver cómo cambian los datos en diferentes años
3. **Explorar deportes**: Seleccionar un deporte específico del mapa de paridad
4. **Comparar ratios**: Usar el gráfico de ratio para identificar desequilibrios
5. **Análisis de crecimiento**: Revisar la comparativa de crecimiento para entender tendencias

### Ejemplos de análisis posibles:

- "¿Cómo afectó la pandemia a cada género?"
- "¿Qué deportes han logrado mantener la paridad?"
- "¿Cuál es la tendencia en fútbol vs otros deportes?"
- "¿Qué deportes tienen mayor potencial de crecimiento para la participación femenina?"

---

## MEJORAS FUTURAS (Opcionales)

- **Exportación de datos**: Botón para descargar datos filtrados
- **Compartir vista**: URL con parámetros para compartir una vista específica
- **Comparación de temporadas**: Vista side-by-side de dos temporadas
- **Análisis por municipio**: Si los datos lo permiten, filtro geográfico
- **Gráficos adicionales**: Heatmap temporal, treemap de deportes, etc.

---

## FUENTES DE DATOS

- **Open Data Bizkaia**: https://www.opendatabizkaia.eus/es/catalogo/deporte-escolar
- **Período analizado**: 2018-2019 a 2023-2024
- **Total de participaciones**: 261.015 registros

---

## CONTACTO

**Elaborado por:** Irene Tobajas Sebastián  
**Contacto:** irenetobajas@gmail.com  
**Fecha:** Diciembre 2024

---

**Versión:** 1.0  
**Estado:** Propuesta completa lista para implementación



