# Masmundok

Web de Masmundok (Yesi y Pablo): requisitos de entrada, noticias de viaje, descuentos, videos y chat con Mundito.

Es una sola página (`index.html`) y se publica con GitHub Pages.

Para cambiar contenido, buscá estos bloques dentro de `index.html`:
- `SITE`: correo, redes, Cafecito, PayPal y fecha de la edición.
- `PARTNERS`: códigos de descuento.
- `NEWS`: noticias de la sección News (y de la barra roja fija de abajo, que las recorre por categoría). Cada noticia puede llevar `foto:'clave'` con una clave de `FOTOS` para mostrar una foto real; si no carga, queda la ilustración. No se muestran fechas.
- `FOTOS` y `FOTO_PAIS`: fotos reales (Wikimedia Commons, con crédito en cada noticia). `FOTOS` es clave → nombre de archivo; `FOTO_PAIS` dice qué foto usar según el país de la noticia.
- `DEST`: fichas de cada país.
- `VIDEOS`: lista de videos.
- `AFILIADOS`: códigos de Travelpayouts y GetYourGuide y marcas de los buscadores.
- `CITIES` e `IDEAS`: ciudades del buscador y destinos sugeridos. Cada ciudad es `[nombre, código, país, palabras extra, provincia]`: la provincia y las palabras extra hacen que, por ejemplo, "Misiones" muestre Puerto Iguazú y Posadas.
- `ORIGENES` (dentro de `initBuscadores`): países cuyos aeropuertos aparecen en "Salgo desde".
- `MONEDAS_GRUPOS` y `MONEDA_POR_PAIS`: monedas del selector (por región) y la que arranca según el país de salida.
- `REGIONES` y `REGION_DE_PAIS`: desplegable "Región" por continente (LATAM, Norteamérica, Europa, Asia, África, Oceanía) con aerolíneas y destinos populares.
- `AEROLINEAS`: nombre → `[código IATA, sitio oficial]`. Al elegir una aerolínea se filtra la comparativa y se ofrece "Ir al sitio oficial" (ese link no paga comisión).
- `AFILIADOS.travelpayouts.token`: token de la API de Travelpayouts (Perfil → API token). Vacío por defecto. Con token aparecen la comparativa de precios por aerolínea ("Elegir la más barata te ahorra…") y las ofertas de hoy en la barra de abajo. Ojo: el token queda visible en el código de la página.
- En `AFILIADOS.vuelos`, las marcas con `p` vacío (KAYAK, Skyscanner, Turismocity) quedan ocultas hasta cargar su código de Travelpayouts.
- `FESTEJOS`: frases y animaciones de Yesi y Pablo.
- `COMUNIDAD` y `COMENTARIOS`: números reales, contador de visitas y comentarios aprobados.
