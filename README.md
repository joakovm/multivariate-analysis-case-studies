# Análisis Multivariante: casos prácticos en R

Dos proyectos de análisis estadístico multivariante aplicados a datos reales de micología, ecología y zootecnia, desarrollados en R con [Quarto](https://quarto.org/).

## Contenido

| Proyecto | Datos | Técnicas |
|---|---|---|
| [`amanita-ponderosa-mineral-analysis/`](./amanita-ponderosa-mineral-analysis) | Composición mineral de *Amanita ponderosa* (cuerpo fructífero y suelo) | Estadística descriptiva, test LSD, estadísticos robustos, Análisis de Componentes Principales (ACP), escalado multidimensional no métrico (NMDS) |
| [`normality-clustering-discriminant-analysis/`](./normality-clustering-discriminant-analysis) | Composición corporal, dieta del búho real, razas bovinas | Contraste de normalidad multivariante, T² de Hotelling, clustering jerárquico / k-means / PAM, análisis discriminante lineal (LDA) |

Cada carpeta tiene su propio README con el detalle del análisis y de los datos que necesita.

## Cómo usarlo

Abre `multivariate-analysis-case-studies.Rproj` con RStudio: todo el repositorio queda como un único proyecto, con los dos análisis en sus subcarpetas.

Requisitos:
- R (≥ 4.2)
- [Quarto](https://quarto.org/)
- Paquetes de R usados: `dplyr`, `kableExtra`, `agricolae`, `MASS`, `vegan`, `MVN`, `mvnormtest`, `cluster`, `ggplot2` (cada script los instala automáticamente si no los encuentra)

\`\`\`bash
quarto render amanita-ponderosa-mineral-analysis/caracterizacion-inorganica-amanita-ponderosa.qmd
quarto render normality-clustering-discriminant-analysis/metodos-multivariantes-normalidad-clustering-discriminante.qmd
\`\`\`

## Datos

Ningún archivo de datos crudo está incluido en este repositorio. Cada proyecto necesita sus datos colocados junto al `.qmd` correspondiente para poder ejecutarse.

## Autor

Joaquín Villegas

## Licencia

El código de este repositorio se publica bajo licencia MIT (ver [LICENSE](./LICENSE)). Esta licencia cubre únicamente el código; los datos, cuando se usan, mantienen los términos de sus fuentes originales.
