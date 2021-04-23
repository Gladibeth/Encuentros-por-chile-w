# Encuentros por Chile

## Desarrollo:

**Uso de sass**

- Instalar:
  `npm install -g sass`

Nota: Sólo se debe editar los archivos scss, ellos serán compilados y generarán el css

- Compilar:
  `sass --watch assets/scss/main.scss:assets/css/main.css --sourcemap=none --style compressed`

- Reemplazar las rutas anteriores por las de los archivos a utilizar, se pueden compilar varios archivos al mismo tiempo.

- Lo que está antes de los dos puntos (:) es el input, es decir, el archivo scss a compilar, y lo que está luego de los dos puntos (:) es el archivo css donde se compilará.

- Debe agregarse el flag: "--sourcemap=none" en el comando, para que no cree archivos .css.map.
- Debe agregarse el flag: "--style compressed" en el comando, para que al compilar el archivo, expulse un archivo .css comprimido.

### En este proyecto se están utilizando parciales para las pages, que se importan en el archivo main, para que al compilar sea un sólo archivo comprimido, es decir, se compila solo el archivo main.scss