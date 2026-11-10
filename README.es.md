# WalkerFans H2 — Restauración e instalador de Rockbox

**WalkerFans para el reproductor HIFIWALKER H2 Hi-Fi / DAP / MP3 — restauración de fábrica, instalador de Rockbox y rescate por USB.**

**Etiquetas:** #HIFIWALKER #HIFIWALKERH2 #Rockbox #DAP #MP3Player #HiFiPlayer #FirmwareRestore

> **Importante — basado en el firmware original HIFIWALKER V2.3.** Estas herramientas se desarrollaron y probaron en un H2 con el firmware original HIFIWALKER **V2.3**. Otras versiones del firmware no se han probado en un reproductor real y podrían no ser compatibles. Si tu reproductor tiene otra versión, haz antes una copia de seguridad y continúa bajo tu propia responsabilidad.

Mantenido y empaquetado por **WalkerFans Team**. Herramientas comunitarias para el HIFI WALKER H2; no es una versión oficial ni una certificación de Rockbox. [English](README.md)

Restaura el firmware de fábrica del reproductor, prepara una instalación de Rockbox o arranca temporalmente su menú de recuperación por USB.

| Descarga | Plataforma | Estado |
|---|---|---|
| HIFIWALKER-Restore-mac-v0.2.2.zip | macOS 13+, Apple Silicon / Intel | Firmada y notarizada por Apple; flujo completo y cierre/reapertura probados en el Mac de desarrollo |
| HIFIWALKER-Restore-Windows-v0.3.2-preview.zip | Windows 10/11 x64 | Versión preliminar; instalación de Rockbox y expulsión segura probadas en hardware Windows; formateo y rescate USB aún sin probar en Windows; sin firma digital |

La aplicación está disponible en inglés, francés, alemán, italiano, español, japonés, chino tradicional, chino simplificado, árabe y ruso. Los nombres de los menús del reproductor se mantienen en inglés para que coincidan con su pantalla.

La instalación de Rockbox admite el firmware original del H2 de la V1.0 a la V2.3. Por ahora, los archivos de restauración de fábrica solo se incluyen para la **V2.3**. No uses ese archivo para otra versión. El rescate por USB (arranque en RAM) admite las tres generaciones de hardware conocidas del H2, pero no puede reparar cualquier fallo de hardware.

El instalador incluye **Rockbox 4.0 estándar**, no la versión de desarrollo WalkerFans con Bluetooth. Para usar esa versión, instala primero Rockbox correctamente y luego sigue las instrucciones de actualización del proyecto Bluetooth (solo hardware revisión 4).

Consulta el [manual en español](MANUAL.es.md), los [cambios](CHANGELOG.md) y las [notas de la versión](RELEASE.md).

## ¿Instalaste la versión equivocada?

La aplicación solo copia archivos a la tarjeta; es el propio reproductor el que realiza la actualización. La aplicación **no** hace copia del firmware interno del reproductor (no puede leerlo), pero la mayoría de los errores se pueden deshacer:

- **Rockbox no sustituye al sistema original.** Mantén pulsado **▶** al encender para arrancar el firmware original en cualquier momento.
- **Instalador o versión de Rockbox equivocados, pero el reproductor arranca:** vuelve a ejecutar la aplicación con la versión que aparece en System Settings → Device Information → Version Information e instala de nuevo. Si mantienes pulsado **Volumen +** al encender se abre el menú de recuperación, donde **USB mode** conecta la tarjeta al ordenador.
- **Pantalla negra / no arranca:** usa **Ayuda → El reproductor no arranca (rescate)…** para cargar el menú de recuperación en la RAM por USB, elige **USB mode** y continúa en el asistente principal con la versión correcta.
- **Volver al firmware de fábrica:** **Restaurar el firmware de fábrica** (incluido **solo para V2.3**; para otras versiones, escríbenos adjuntando el archivo de diagnóstico del menú Ayuda).
- **Copias de la tarjeta:** los archivos de actualización sustituidos y las copias completas hechas antes de formatear se guardan en **Documentos → HIFIWALKER Backups** (Windows) o en la ubicación que indica la app de Mac.

Comprueba siempre el número de versión en el reproductor antes de empezar.

## Créditos

Mantenimiento, empaquetado y documentación: **WalkerFans Team**. Rockbox, los cargadores de arranque, libusb, .NET y sus colaboradores conservan sus avisos originales de copyright y licencia. Consulta THIRD-PARTY.md y los archivos de licencias y código fuente que acompañan a los paquetes.

## Aviso legal

WalkerFans Team es un grupo de aficionados y entusiastas de HIFIWALKER. Este proyecto se comparte solo para desarrollo e intercambio en la comunidad, sin fines comerciales: no obtenemos ningún beneficio económico. No es una versión oficial del proyecto Rockbox. Todas las marcas y derechos de autor pertenecen a sus respectivos propietarios.

Si algún contenido afecta a derechos de autor, patentes u otros derechos que desconozcamos, escríbenos a **walkerfans007@gmail.com** y lo retiraremos.

— **WalkerFans Team** · walkerfans007@gmail.com
