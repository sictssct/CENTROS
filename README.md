# Tablero de Control Centros SICT — versión optimizada para GitHub Pages

## Archivos
- `index.html`: tablero y lógica de navegación.
- `data/`: capas geográficas externas en GeoJSON.
  - `estados_mexico.geojson`
  - `red_vial.geojson`
  - `puntos_tdpa.geojson`
  - `aeropuertos.geojson`
  - `rutas_nacionales.geojson`
  - `rutas_internacionales.geojson`
  - `tramos_aforos.geojson`

## Publicar en GitHub Pages
1. Descomprime este paquete.
2. Sube `index.html` y la carpeta `data` a la raíz del repositorio (conserva los nombres).
3. En GitHub, entra a **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**, elige la rama que uses (por ejemplo `main`) y la carpeta `/ (root)`.
5. Guarda y abre la URL que GitHub Pages te muestre.

## Importante
- No subas únicamente `index.html`: necesita todos los archivos de `data`.
- Los mapas cargan las capas mediante `fetch`, por lo que deben probarse desde GitHub Pages o desde un servidor local; abrir `index.html` directamente con doble clic puede bloquear las solicitudes por restricciones del navegador.
- Se conservan los datos y las propiedades originales del GeoJSON; esta versión cambia su ubicación, no su contenido.
