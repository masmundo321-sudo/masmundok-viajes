# Masmundok

Web de Masmundok (Yesi y Pablo): requisitos de entrada, noticias de viaje, descuentos, videos y chat con Mundito.

Es una sola página (`index.html`) y se publica con GitHub Pages.

Para cambiar contenido, buscá estos bloques dentro de `index.html`:
- `SITE`: correo, redes, Cafecito, PayPal y fecha de la edición.
- `PARTNERS`: códigos de descuento.
- `NEWS`: noticias de la sección News.
- `DEST`: fichas de cada país.
- `VIDEOS`: lista de videos.
- `AFILIADOS`: códigos de Travelpayouts y GetYourGuide y marcas de los buscadores.
- `CITIES` e `IDEAS`: ciudades del buscador y destinos sugeridos. Cada ciudad es `[nombre, código, país, palabras extra, provincia]`: la provincia y las palabras extra hacen que, por ejemplo, "Misiones" muestre Puerto Iguazú y Posadas.
- `ORIGENES` (dentro de `initBuscadores`): países cuyos aeropuertos aparecen en "Salgo desde".
- `MONEDAS_GRUPOS` y `MONEDA_POR_PAIS`: monedas del selector (por región) y la que arranca según el país de salida.
- `REGIONES` y `REGION_DE_PAIS`: desplegable de vuelos por región (destinos y aerolíneas populares).
- En `AFILIADOS.vuelos`, las marcas con `p` vacío (KAYAK, Skyscanner, Turismocity) quedan ocultas hasta cargar su código de Travelpayouts.
- `FESTEJOS`: frases y animaciones de Yesi y Pablo.
- `COMUNIDAD` y `COMENTARIOS`: números reales, contador de visitas y comentarios aprobados.
