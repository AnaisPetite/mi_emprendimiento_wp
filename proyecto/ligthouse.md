# Análisis de rendimiento con Lighthouse

**Sitio analizado:** https://nabi-skin.infinityfree.me/ 
**Herramienta:** PageSpeed Insights 
**Dispositivo:** Móvil  
**Fecha del análisis:** 25 de noviembre de 2026  

## 1. Resultados (1 pt)

| Categoría | Puntaje (0 a 100) |
|---|---|
| Rendimiento | 99 |
| Accesibilidad | 100 |
| Prácticas recomendadas | 100 |
| SEO | 92 |

**Evidencia:** <img width="640" height="223" alt="evidencia-sitioweb" src="https://github.com/user-attachments/assets/3f34b5cb-5c42-454d-9acf-9fd5613086b9" />


## 2. Análisis (1 pt)

- **Qué significan mis puntajes:** Son las notas que le da Google a mi sitio web evaluando qué tan rápido carga en el celular, si es fácil de usar para cualquier persona, si cumple con las buenas prácticas de programación y si está bien preparado para aparecer en los buscadores.
- **Mi mejor categoría y por qué:** Accesibilidad y Prácticas recomendadas con **100 puntos**, porque el tema de bloques de WordPress que utiliqué (*Twenty Twenty-Five*) ya viene muy bien estructurado de base con etiquetas limpias y ordenadas.
- **Mi categoría más débil y por qué:** SEO con **92 puntos**, ya que aunque los títulos y textos están claros para los buscadores, siempre quedan pequeños detalles por pulir en las descripciones de las páginas.
- **Problemas que encontré en el informe:** Algunos recursos estáticos y fuentes que cargan al inicio y hacen que el navegador se tome una milésima de segundo más en mostrar la página completa, además de la acumulación de algunos archivos de los plugins.

## 3. Mejoras (1 pt)

| Mejora | Qué problema resuelve | ¿Aplicada o propuesta? | Resultado (si la aplicaste) |
|---|---|---|---|
| Optimización y conversión de imágenes a WebP | Reduce el peso de la transferencia de red y mejora la carga visual de la página principal. | Aplicada | Excelente puntaje de 99 en rendimiento móvil. |
| Uso de la etiqueta `fetchpriority="high"` en la imagen principal (LCP) | Acelera el descubrimiento y la descarga prioritaria del banner de bienvenida. | Aplicada | Tiempos de First Contentful Paint y LCP muy rápidos (~1.6s). |

