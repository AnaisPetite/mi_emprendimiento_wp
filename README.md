# Nabi Skin · Sitio WordPress

> **Este README es tuyo.** Complétalo mientras construyes tu sitio y borra las instrucciones entre paréntesis. Las instrucciones del proyecto están en [`indicaciones/README.md`](indicaciones/README.md).

- **Sitio en producción:** https://nabi-skin.infinityfree.me/
- **Prototipo en Stitch:** https://stitch.google.com/projects/15130692259384807424
- **Repo del Parcial 02:** https://github.com/AnaisPetite/nabi-skin
- **Autor/a:** Anaís Cruz / Sección: 001D

## Contexto de la web

Nabi Skin es un e-commerce y marca de cosmética coreana (K-Beauty) enfocado en clientas jóvenes que buscan una rutina de cuidado facial efectiva y de origen natural. El sitio resuelve la necesidad de encontrar productos especializados en un solo lugar y guía a la usuaria mediante la proto-persona Sofía hacia una experiencia de compra intuitiva, educativa y visualmente limpia. Su propósito principal es captar el interés de la visitante y facilitar la exploración de su catálogo y métodos de pago.

## Mi tema

- [ ] **Tema propio:** `(nombre del tema)`
- [x] **Tema descargado:** `Twenty Twenty-Five` · (https://wordpress.org/themes/twentytwentyfive/)
---

## Instrucciones si uso un tema descargado

### Requisitos del tema

| Dato | Mi tema |
|---|---|
| Nombre y enlace a la ficha | [Twenty Twenty-Five](https://wordpress.org/themes/twentytwentyfive/) |
| Gratis o de pago | Gratis |
| Tipo (clásico o de bloques) | Tema de bloques (Block Theme) |
| Versión de WordPress que requiere | 6.7 o superior |
| Versión de PHP que requiere | 7.2.2 o superior |
| Plugins que necesita (si alguno) | Contact Form 7, Flamingo, All-in-One WP Migration |
| Licencia | Licencia Pública General GNU (GPLv2 o posterior) |


### Cómo llevar mi sitio de Local a producción

Explica cómo exportas los datos de tu sitio en Local WP y los importas en producción (InfinityFree) con un plugin. Completa:

- **Plugin de migración que uso:** [All-in-One WP Migration](https://wordpress.org/plugins/all-in-one-wp-migration/) · Gratis. Límites que tiene: 512 MB de tamaño máximo de importación en la versión gratuita.
- **Qué se exporta:** Entradas, páginas, imágenes, menús, y tema.

Pasos:
1. **En Local:** Abres tu sitio en Local WP, vas al panel de administración de WordPress, instalas el plugin *All-in-One WP Migration*, haces clic en **Exportar > Archivo** y descargas el archivo `.wpress` a tu computador.
2. **En producción:** Entras a tu panel de InfinityFree, instalas un WordPress limpio, y en su panel instalas el mismo tema (*Twenty Twenty-Five*) y el plugin *All-in-One WP Migration*.
3. **Importa:** Vas a *All-in-One WP Migration > Importar*, seleccionas "Archivo" y subes el archivo `.wpress` que exportaste desde Local.
4. **Revisa:** Verifica los enlaces permanentes (en Ajustes > Enlaces permanentes), el menú de navegación, la página de inicio, las imágenes y el formulario de contacto.
5. **Problemas que tuve y cómo los resolví:** El límite de subida del servidor gratuito de InfinityFree. Se solucionó quitando los plugins y comentarios.

---

## Respaldo y reinstalación en otro servidor

El objetivo de este proyecto es que puedas **respaldar tu sitio y reinstalarlo en cualquier servidor**. Explícalo para que otra persona pueda seguir tus pasos.

**Qué respaldar:**
- Los archivos de WordPress (tema Twenty Twenty-Five, plugins como Contact Form 7 y Flamingo, e imágenes subidas a la biblioteca de medios).
- La base de datos (páginas, entradas, menús, formularios y configuración del sitio).

**Cómo respaldo mi sitio:**
- Utilizo el plugin **All-in-One WP Migration** desde el panel de WordPress para generar un archivo comprimido `.wpress` con toda la información. Este archivo queda guardado en mi computador local como respaldo principal. Lo realizo cada vez que hago cambios importantes en el diseño o contenidos del sitio.

**Cómo lo reinstalo en un servidor nuevo:**
1. **Requisitos del servidor:** PHP versión 7.2.2 o superior, MySQL o MariaDB compatible con WordPress 6.7+, y al menos 1 GB de espacio libre en disco.
2. **Instalar WordPress limpio:** Se instala una versión limpia de WordPress en el nuevo servidor mediante el instalador automático del hosting (Softaculous o similar).
3. **Restaurar el respaldo:** Se instala el plugin *All-in-One WP Migration* en la nueva instalación de WordPress, se importa el archivo `.wpress` guardado previamente y se guardan dos veces los enlaces permanentes para actualizar las rutas.
4.  **Ajustar:** Ve a **Ajustes > Enlaces permanentes** en tu panel de WordPress y haz clic dos veces en **Guardar cambios** para refrescar las URLs.
Revisa el menú de navegación principal, que la página de inicio (Home) cargue correctamente y que las imágenes se muestren sin enlaces rotos.
5. **Probar:** 
**Sitio web:** Navega por las diferentes páginas de tu tienda de cosmética coreana para confirmar que todo responde con fluidez.
**Imágenes:** Comprueba que los banners, mockups y fotos de productos se visualizan correctamente desde la biblioteca de medios.
**Formulario de contacto:** Realiza una prueba enviando un mensaje a través del formulario público (`/contacto/`) y verifica que los datos se guarden correctamente en el panel de **Flamingo**. 

**Problemas que tuve y cómo los resolví:** 
   - **Problema:** El servidor gratuito de InfinityFree bloquea por defecto los puertos de salida de correo (`wp_mail`), lo que impedía que Contact Form 7 enviara notificaciones por email y arrojaba un aviso de error al usuario en la página pública.
   - **Solución:** En lugar de depender del envío de correos salientes del servidor, integré el plugin **Flamingo** (creado por el mismo autor de Contact Form 7). Esto permite capturar, respaldar y almacenar localmente todos los mensajes de los clientes directamente en la base de datos de WordPress, garantizando que ningún contacto se pierda y cumpliendo con el objetivo funcional de la sección de contacto.

     
## Plugins instalados

| Plugin | Para qué lo uso | Gratis o de pago | Versión |
|---|---|---|---|
| [Contact Form 7](https://wordpress.org/plugins/contact-form-7/) | Gestión del formulario de contacto principal de la tienda | Gratis | 5.9+ |
| [Flamingo](https://wordpress.org/plugins/flamingo/) | Almacenamiento local de los mensajes de contacto en la base de datos (respaldo ante bloqueo de correo) | Gratis | 2.5+ |
| [All-in-One WP Migration](https://wordpress.org/plugins/all-in-one-wp-migration/) | Exportación e importación del sitio completo entre Local WP y producción | Gratis | 7.8+ |

## Páginas y entradas

- **Páginas:** 
  1. **Inicio:** Presentación de la marca, banner principal de la colección y llamada a la acción.
  2. **Sobre nosotros:** Historia de Nabi Skin, la filosofía K-Beauty y la proto-persona Sofía.
  3. **Blog:** Artículos educativos sobre rutinas de cuidado facial y consejos de belleza.
  4. **Contacto:** Formulario interactivo con almacenamiento local y datos de atención.

- **Entradas del blog:** 
  1. *Centella Asiática: El ingrediente estrella para calmar la piel*
  2. *5 señales de que tu barrera cutánea necesita atención*
  3. *Guía básica de doble limpieza coreana para principiantes*

## Uso de IA

- **Google Gemini:** Utilizado como apoyo académico y de diseño para estructurar los textos comerciales, redactar copy persuasivo para las publicaciones del blog y resolver dudas técnicas de desarrollo con WordPress. Todo el contenido generado fue revisado y adaptado personalmente.

## Cómo me organicé

Mi plan y mi plan B están en [`decisiones.md`](https://github.com/AnaisPetite/mi_emprendimiento_wp/blob/main/proyecto/desiciones.md) 

## Plan de continuidad y rendimiento

- **Plan de continuidad (etapa 2 de mi web):** [`plan-de-continuidad.md`](proyecto/plan-de-continuidad.md)
- **Análisis de rendimiento con Lighthouse:** [`lighthouse.md`](https://github.com/AnaisPetite/mi_emprendimiento_wp/blob/main/proyecto/ligthouse.md)
