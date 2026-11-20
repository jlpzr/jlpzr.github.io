# Xanders

Sitio oficial: <https://xanders.me/>. Landing en español de la marca de desarrollo
de aplicaciones, publicada con GitHub Pages desde `main`.

## Estructura

- `index.html`: inicio, aplicaciones, sobre Xanders y contacto. Jekyll procesa su
  front matter con `layout: null` e incluye el código existente de AdSense desde
  `_includes/head-custom.html`.
- `assets/xanders/site.css`: diseño adaptable, azul medianoche y acento lima,
  titulares editoriales en Georgia, cuerpo en fuentes del sistema, navegación por
  teclado y `prefers-reduced-motion`. La animación se concentra en la entrada de la
  portada, el símbolo de marca y el titular de escritura progresiva.
- `assets/xanders/`: logotipo vectorial, favicon y dos imágenes WebP.
- `privacidad/index.html`: índice de políticas de privacidad de las aplicaciones.
- `cotizame/privacidad/index.html`: política de privacidad de Cotizame.
- `CHANGELOG.md`: registro interno de cambios, excluido de la salida de Jekyll por `_config.yml`.
- `googleeb36ee55bdb6964e.html`: archivo de propiedad de Search Console.
- `CNAME`: dominio `xanders.me`.

La landing no requiere frameworks, fuentes remotas ni un build de Node. El titular
usa un pequeño script progresivo para animar su escritura; sin JavaScript se muestra
completo. Los cambios se publican al hacer push a `main`; la verificación definitiva
es el despliegue de Pages y el HTML servido en el dominio.

## Contenido y recursos confirmados

- Logo: vector existente de Xanders, `logo-vectorial (1).svg`. Se conservan las
  geometrías y el color blanco; el favicon añade un fondo azul medianoche.
- Icono de Cotizame: `docs/icono_new.png` del proyecto Cotizame, reducido a 128 px.
- Captura: `normal-app-api29.png`, evidencia de aceptación de Cotizame del
  8 de noviembre de 2026 en Android/API 29. Contiene exclusivamente datos de prueba;
  se conserva completa, incluido el indicador de desarrollo. WebP a 576 × 1280 px.
- Contacto: `soporte.xanders@gmail.com`, [Facebook](https://www.facebook.com/people/Xanders/61596795898686/) e [Instagram](https://www.instagram.com/xanders.dev?bqrl=MXVsdHpmZmh3aDY3ag==).
- Cotizame se presenta en desarrollo. No hay una URL confirmada de la ficha ni de
  la página de desarrollador en Google Play. Añadirlas cuando estén disponibles;
  no construir enlaces a partir del nombre o del identificador del paquete.

## Verificación de la landing

En una vista previa local se expandió únicamente el include de Jekyll para comprobar
el diseño con Microsoft Edge/Playwright. Anchos: 320, 390, 768, 1024 y 1440 px;
anclas, foco visible, salto al contenido, imágenes y enlace de privacidad correctos.
Sin desbordamiento horizontal, también al simular zoom al 200 %. Recorrido principal
funcional sin JavaScript y movimiento reducido verificado. Axe (WCAG 2 A/AA y 2.1 AA)
sin infracciones automáticas en esos tamaños; no sustituye una evaluación manual
completa con tecnologías de asistencia. Capturas de escritorio/móvil revisadas.

El servicio externo de AdSense se excluye de las pruebas locales de diseño. Su
snippet sigue integrado; estas pruebas no acreditan aprobación ni entrega de anuncios.
