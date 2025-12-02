# PaginaWebCTT

Repositorio del sitio web del Centro de Transferencia Tecnológica (CTT) de la Universidad Técnica de Ambato.

## Descripción del proyecto

Este proyecto es un sitio web estático que presenta la oferta de cursos, información de contacto y objetivos del CTT (Centro de Transferencia Tecnológica). Está construido con HTML, CSS y JavaScript, y utiliza recursos de terceros que se incluyen en el repositorio (Bootstrap, Owl Carousel, etc.).

## Estructura de carpetas (resumen)

- `index.html` — Página principal.
- `about.html` — Página Sobre Nosotros.
- `contact.html` — Página de contacto.
- `course.html` — Listado de cursos.
- `curso1AD.html`, `curso2BP.html`, ... — Páginas individuales de cursos.
- `css/` — Hojas de estilo (Bootstrap y estilos personalizados).
- `img/` — Imágenes usadas en el sitio.
- `js/` — JavaScript personalizado (`main.js`).
- `lib/` — Librerías de terceros (ej.: `owlcarousel`, `easing`).
- `mail/` — Archivos para el formulario de contacto (`contact.php`, validaciones JS).
- `scss/` — Fuentes SCSS (si desea recompilar estilos desde Sass).
- `LICENSE.txt` — Licencia del proyecto (si aplica).
- `READ-ME.txt` — Archivo antiguo de notas (considérelo legado).

> Nota: Esta es una visión general. Para ver el árbol completo, explore el repositorio.

## Instalación (local)

1. Clona el repositorio:

```powershell
git clone https://github.com/CarlosAl21/PaginaWebCTT.git
cd PaginaWebCTT
```

2. Abrir localmente (opciones):

- Abrir `index.html` directamente en el navegador (doble clic).
- O servir los archivos con un servidor local (recomendado para formularios o AJAX):

```powershell
# Usando Python 3
py -3 -m http.server 8000
# o
python -m http.server 8000

# Luego abrir http://localhost:8000
```

Si utiliza un formulario que llama a `mail/contact.php`, necesitará un servidor con PHP (por ejemplo, XAMPP, WAMP o un host que soporte PHP) y desplegar/servir el proyecto desde allí.

## Dependencias

Las dependencias cliente (bibliotecas) ya están incluidas en el repositorio en su forma estática:

- Bootstrap (archivos CSS en `css/`, JS cargado desde CDN en algunas páginas).
- Owl Carousel (`lib/owlcarousel/`).
- Easing (`lib/easing/`).
- jQuery (se carga desde CDN en `about.html` y otras páginas).

No hay un administrador de paquetes (npm, pip) configurado en este repositorio; todas las librerías necesarias para la apariencia/funcionalidad básica están incluidas o son cargadas desde CDN.

## Ejecución / Uso

- Para ver el sitio: abrir `index.html` o usar el servidor local mostrado en la sección de instalación.
- Para probar el formulario de contacto (`mail/contact.php`) ejecute el sitio en un servidor con PHP y configure el envío de correo según el host.

## Despliegue (sugerencia rápida)

- GitHub Pages: en la configuración del repositorio (Settings → Pages) habilite Pages desde la rama `main` (root). Si todo está en `main`, GitHub servirá `index.html` como página estática.
- Alternativa: subir los archivos a cualquier hosting estático (Netlify, Vercel, Surge, Firebase Hosting, etc.).

## Contribuciones

Si desea contribuir:

1. Cree un fork del repositorio.
2. Abra una rama (`git checkout -b feature/nombre`).
3. Realice cambios y cree un pull request con una descripción clara.

## Licencia

Consulte `LICENSE.txt` para los términos de licencia del proyecto.

---

Si desea, puedo también crear un `README` en inglés, o generar un `index` optimizado para GitHub Pages (carpeta `docs/`). ¿Quiere que haga commit y push estos cambios por usted?
