# Mentes Amplificadas

Sitio estático para la presentación **Mentes Amplificadas** y su guía interactiva de frameworks de prompts.

## Sitio en Producción (GitHub Pages)

- Presentación principal: https://gvaldezr.github.io/memovaldez/
- Guía de frameworks: https://gvaldezr.github.io/memovaldez/pages/frameworks.html
- PDF de apoyo: https://gvaldezr.github.io/memovaldez/assets/docs/Mentes_Amplificadas.pdf

## Estructura del Repositorio

```text
.
├── index.html
├── pages/
│   └── frameworks.html
└── assets/
    └── docs/
        ├── frameworks_qr.png
        └── Mentes_Amplificadas.pdf
```

## Descripción de Archivos

- `index.html`: Deck principal de diapositivas (incluye una diapositiva final con QR local hacia la guía de frameworks).
- `pages/frameworks.html`: Guía interactiva para construir prompts con distintos frameworks.
- `assets/docs/frameworks_qr.png`: QR local que apunta a la guía de frameworks.
- `assets/docs/Mentes_Amplificadas.pdf`: Documento PDF de referencia.

## Ejecutar Localmente

Como es un sitio estático, basta con servir la carpeta del repo con cualquier servidor HTTP.

Ejemplo con Python:

```bash
python3 -m http.server 8080
```

Luego abrir:

- http://localhost:8080/
- http://localhost:8080/pages/frameworks.html

## Publicación

GitHub Pages publica desde la rama `main` de este repositorio.

Flujo recomendado:

```bash
git add .
git commit -m "Actualiza sitio"
git push origin main
```

## Notas

- Mantener rutas relativas para conservar compatibilidad con GitHub Pages.
- El QR de la presentación se sirve desde un archivo local del repositorio para evitar dependencias externas en runtime.
- La guía de frameworks incorpora mejoras de accesibilidad (etiquetado ARIA y anuncio de estado al copiar).
- Evitar agregar archivos de sistema como `.DS_Store`.
