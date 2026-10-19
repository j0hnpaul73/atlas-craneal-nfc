# Atlas craneal NFC

## Contenido
- `index.html`: visor web interactivo.
- `assets/craneo-anatomico.glb`: modelo 3D aportado por el usuario.

## Probar en el ordenador
El visor importa Three.js desde una CDN y carga el modelo mediante una ruta relativa. Por eso no debe abrirse con doble clic como `file://`.

1. Instala Python si no lo tienes.
2. Abre una terminal dentro de esta carpeta.
3. Ejecuta `python -m http.server 8000`.
4. Abre `http://localhost:8000` en el navegador.

## Publicar gratis con GitHub Pages
1. Crea un repositorio público en GitHub.
2. Sube `index.html` y la carpeta `assets` completa.
3. En el repositorio, abre Settings → Pages.
4. Selecciona Deploy from a branch, la rama `main` y la carpeta `/ (root)`.
5. Guarda y espera a que GitHub Pages publique la web.
6. Abre la dirección publicada y comprueba el modelo en un teléfono.
7. Programa la etiqueta NFC con esa URL usando una app de escritura NFC.

## Importante sobre este modelo
El GLB contiene 29 piezas separadas, con nombres anatómicos y materiales de color. El conjunto parece parcial: incluye ocho estructuras agrupadas bajo `Bones` y piezas adicionales del lado derecho, además de dientes. Verifica la cobertura anatómica antes de usarlo como atlas completo.

La página usa Three.js desde jsDelivr, por lo que necesita conexión a internet. Las descripciones incluidas son iniciales y deben revisarse para uso académico.


Corrección de compatibilidad: el HTML incluye un import map para resolver los módulos internos de Three.js.
