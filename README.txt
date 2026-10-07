IGORADMIN — Paquete para GitHub Pages

CONTENIDO
index.html
igor-logo.png
login-background.png
README.txt

Los tres archivos del mockup son copias exactas de los adjuntos recibidos. Se eligió index.html; el respaldo index.html.pre-ticket-fix.bak no se incluye. No se han añadido funciones ni corregido el código original.

CÓMO SUBIRLO
1. Descomprime IGORADMIN-GitHub-Pages.zip.
2. En tu repositorio de GitHub, usa Add file > Upload files y carga los archivos descomprimidos. index.html y los dos PNG deben quedar juntos en la raíz de la rama que publicarás. No subas únicamente el ZIP.
3. Guarda los cambios con Commit changes.
4. En Settings > Pages, selecciona Deploy from a branch, la rama correspondiente (normalmente main) y /(root). Guarda.
5. Cuando GitHub termine el despliegue, abre la dirección indicada en Pages.

Si ya tienes otra web en ese repositorio, usa uno nuevo para no reemplazarla.
Guía oficial: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

USO
Pulsa «Usar datos de prueba» en el acceso. Es un prototipo sin backend: los cambios se pierden al recargar, la recuperación de contraseña es una simulación y no se envían correos ni se cobran pagos.
El HTML separado también necesita ambos PNG en la misma carpeta. No requiere instalación ni compilación. La fuente Inter se solicita a Google Fonts; si no está disponible, se usa la fuente alternativa.

COMPROBACIONES REALIZADAS
- Sintaxis válida en los seis bloques JavaScript.
- Ambas imágenes locales presentes; logo con transparencia.
- Rutas relativas y navegación por fragmentos compatibles con una subcarpeta de GitHub Pages.
- Ocho comprobaciones aisladas de las reglas SA/A: protección del último SA, bloqueo de degradación SA+A, autopromoción al eliminar SA en pareja SA+A y solo lectura en cuenta inactiva.
- Presencia del renderizado de tarjetas y acordeones cerrados, modal con Copiar/Cerrar, dos grupos de resultados por correo, Tickets deshabilitado y recuperación simulada.
Estas comprobaciones no sustituyen una prueba completa de interfaz.

INCIDENCIAS QUE YA TRAE EL ORIGINAL
- Algunos textos contienen acentos dañados.
- En index.html, línea 845, un bloque duplicado de códigos promocionales usa q fuera de su ámbito: q se declara dentro de la función autoejecutable que termina en la línea 844. Ese bloque puede lanzar «q is not defined». El siguiente bloque declara qq y vuelve a enlazar esos controles, pero no se ha certificado el flujo completo.
- Hay varios bloques duplicados y redefiniciones anteriores. Se conservaron para mantener el archivo recibido sin cambios.
No pudo completarse la prueba en navegador: Chromium no arrancó por una restricción de sockets del entorno de verificación. No se ha publicado ni verificado un sitio en GitHub Pages.

ANTES DE PUBLICAR
El código contiene identidades, correos y datos de ejemplo, además de credenciales de acceso y tarjeta expresamente usadas como simulación. No se detectaron claves de API ni credenciales de servicios externos. La condición de ejemplo no permite confirmar si cada nombre o correo corresponde a una persona real: revísalos antes de hacer el sitio público. Todo dato incluido en el HTML será visible para sus visitantes. No introduzcas contraseñas, tarjetas ni datos personales reales en este prototipo.
