# 📺 Sistema de Análisis y Recomendaciones de Netflix - ECBD

## 🎯 Descripción del Proyecto

Este proyecto implementa un **sistema completo de análisis de datos y recomendaciones para Netflix**, desarrollado como parte de la práctica 09 de la materia Estructura y Consulta de Bases de Datos (ECBD). El sistema combina técnicas de análisis exploratorio de datos (EDA) con algoritmos de machine learning para generar recomendaciones de contenido basadas en similitud de características.

## 🗂️ Estructura del Proyecto

```
Practica09-ECBD/
├── datasets/
│   ├── IMDb movies.xls           # Dataset de películas de IMDb
│   ├── IMDb ratings.xls          # Calificaciones de IMDb
│   ├── netflix_dataset.xls       # Dataset principal de Netflix
│   ├── netflix_movies_detailed_up_to_2025.xls    # Películas detalladas hasta 2025
│   └── netflix_tv_shows_detailed_up_to_2025.xls  # Series detalladas hasta 2025
├── Untitled.ipynb              # Notebook principal con análisis completo
└── README.md                   # Documentación del proyecto
```

## 🚀 Características Principales

### 📊 Análisis Exploratorio de Datos (EDA)
- **Distribución de contenido**: Análisis de películas vs series de TV
- **Análisis temporal**: Patrones de lanzamiento por mes y año
- **Calificaciones**: Distribución de ratings y análisis de películas mejor valoradas
- **Análisis geográfico**: Países que más contenido producen
- **Duración**: Análisis de duración de películas y temporadas de series

### 🤖 Sistema de Recomendaciones
- **Basado en contenido**: Utiliza TF-IDF y similitud del coseno
- **Múltiples características**: Considera título, director, reparto, género y descripción
- **Dos enfoques implementados**:
  1. Recomendaciones basadas únicamente en descripción
  2. Recomendaciones basadas en características combinadas

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Pandas**: Manipulación y análisis de datos
- **NumPy**: Operaciones numéricas
- **Matplotlib & Seaborn**: Visualización de datos
- **Plotly**: Gráficos interactivos
- **Scikit-learn**: Machine Learning (TF-IDF, Cosine Similarity)
- **Jupyter Notebook**: Entorno de desarrollo

## 📋 Requisitos

```bash
# Instalar dependencias
pip install pandas numpy matplotlib seaborn plotly scikit-learn jupyter
```

## 🔧 Instalación y Uso

1. **Clonar el repositorio**:
```bash
git clone https://github.com/Nefta11/Practica09-ECBD.git
cd Practica09-ECBD
```

2. **Instalar dependencias**:
```bash
pip install -r requirements.txt
```

3. **Ejecutar el notebook**:
```bash
jupyter notebook Untitled.ipynb
```

## 📈 Análisis Realizados

### 1. Distribución de Contenido
- Comparación entre películas y series de TV
- Identificación de tendencias de contenido

### 2. Análisis Temporal
- **Heatmap de lanzamientos**: Visualiza patrones estacionales
- **Tendencias anuales**: Análisis de los últimos 15 años de contenido

### 3. Calificaciones y Valoraciones
- Integración con datos de IMDb
- Top 10 películas mejor calificadas
- Distribución de ratings de Netflix

### 4. Análisis Geográfico
- Top países productores de contenido
- Análisis específico para series de TV

### 5. Duración y Temporadas
- Distribución de duración de películas
- Series con mayor número de temporadas

## 🎯 Sistema de Recomendaciones

### Algoritmo 1: Basado en Descripción
```python
# Ejemplo de uso
recommendations = get_recommendations('Avengers: Infinity War')
```

### Algoritmo 2: Basado en Características Múltiples
```python
# Considera: título, director, reparto, género, descripción
recommendations = get_recommendations_new('Black Panther', cosine_sim2)
```

### Características del Sistema:
- **TF-IDF Vectorization**: Para procesamiento de texto
- **Cosine Similarity**: Para calcular similitud entre contenidos
- **Optimización de memoria**: Implementación eficiente para datasets grandes
- **Limpieza de datos**: Preprocesamiento robusto de texto

## 📊 Resultados Principales

### Estadísticas del Dataset:
- **Total de contenido analizado**: +20,000 títulos
- **Películas vs Series**: Distribución balanceada
- **Países representados**: +100 países productores
- **Rango temporal**: Contenido desde 1925 hasta 2025

### Insights Destacados:
1. **Pico de producción**: Mayor cantidad de contenido en años recientes
2. **Estacionalidad**: Patrones específicos de lanzamiento por mes
3. **Diversidad geográfica**: Estados Unidos lidera, seguido por India y Reino Unido
4. **Calidad del contenido**: Correlación entre ratings de IMDb y popularidad en Netflix

## 🔮 Funcionalidades del Sistema de Recomendaciones

- ✅ Recomendaciones precisas basadas en similitud de contenido
- ✅ Procesamiento eficiente de grandes volúmenes de datos
- ✅ Interfaz simple para obtener recomendaciones
- ✅ Soporte para múltiples idiomas y géneros
- ✅ Optimización de memoria para datasets extensos

## 🤝 Contribuciones

Este proyecto fue desarrollado como parte del curso de Estructura y Consulta de Bases de Datos. Las contribuciones son bienvenidas siguiendo estos pasos:

1. Fork del proyecto
2. Crear una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit de tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abrir un Pull Request

## 📄 Licencia

Este proyecto es de uso académico y está disponible bajo la licencia MIT.

## 👨‍💻 Autor

**Nefta11** - [GitHub Profile](https://github.com/Nefta11)

## 🙏 Agradecimientos

- Profesores y compañeros del curso ECBD
- Comunidad de Netflix por proporcionar datasets públicos
- IMDb por las calificaciones complementarias
- Documentación de Scikit-learn y Pandas

---
⭐ **¡Si este proyecto te fue útil, no olvides darle una estrella!** ⭐