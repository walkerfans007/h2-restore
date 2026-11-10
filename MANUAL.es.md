# WalkerFans H2 Tools — Manual rápido

Antes de empezar, haz una copia de seguridad de tu música y ajustes, anota la versión del firmware original y carga el reproductor al menos al 50 %.

**macOS:** descomprime la v0.2.2, mueve la aplicación a Aplicaciones y ábrela. Requiere macOS 13 o posterior, Intel o Apple Silicon.

**Windows:** descomprime por completo la versión preliminar v0.3.1, deja la carpeta `Assets` junto al EXE y acepta la solicitud de permisos de administrador. El entorno .NET va incluido. Esta versión aún no se ha probado en hardware Windows real y no tiene firma Authenticode.

## Instalar Rockbox

1. En el sistema original, consulta System Settings → Device Information → Version Information.
2. Elige **Install Rockbox**, selecciona exactamente esa versión, conecta el reproductor o el lector de tarjetas, confirma que la tarjeta y su capacidad son correctas y sigue el asistente.
3. Formatear borra toda la tarjeta: usa antes la opción de copia de seguridad verificada.
4. Tras la copia, la verificación y la expulsión segura, desconecta el cable y en el reproductor elige System Settings → Firmware Update → YES. No interrumpas la actualización.
5. Vuelve a conectar y elimina el instalador cuando la aplicación lo indique.

Esto instala Rockbox 4.0 estándar. El paquete de desarrollo con Bluetooth es una actualización posterior y separada, solo para dispositivos con hardware revisión 4.

## Restaurar el firmware de fábrica

La restauración incluida es **solo para la V2.3**. Apaga el reproductor, mantén pulsado Volumen + y pulsa Encendido, elige USB mode y usa **Restore factory firmware**. Tras la copia verificada y la expulsión, desconecta, vuelve a entrar en el menú y elige HibyOS Recovery (Aigo Recovery en menús antiguos). Espera a que termine, arranca con normalidad y elimina el instalador. La restauración avanzada solo del cargador de arranque usa Bootloader → Restore.

## Rescate por USB

Menú Help → rescate. Apaga el reproductor por completo, conecta el cable al reproductor, mantén pulsado **M** mientras conectas el otro extremo al ordenador y luego suelta M. En el modo boot ROM la pantalla sigue negra. Selecciona la generación de hardware correcta (V1.0–V1.6 / V1.7–V1.8 / V1.9–V2.3).

En Windows, la primera vez puede hacer falta el controlador WinUSB mediante la web oficial de Zadig: selecciona **solo** el dispositivo con ID USB A108:1000, nunca dispositivos normales de almacenamiento o de entrada. No desactives la comprobación de firmas de controladores.

Detecta el dispositivo y carga el menú de recuperación. Es un arranque temporal en RAM, no una restauración de la memoria flash. Comprueba tú mismo la pantalla del reproductor, elige USB mode y vuelve al asistente principal. Si la pantalla sigue negra, guarda el archivo de diagnóstico.

## Arranque

Enciende normalmente para Rockbox; mantén ▶ al encender para el sistema original; mantén Volumen + al encender para el menú de recuperación. Si cierras la ventana durante una operación con la tarjeta, la aplicación espera a que termine antes de salir.

Mantenimiento y documentación: **WalkerFans Team**. Siguen vigentes los avisos originales de Rockbox, libusb, .NET y del firmware.

Proyecto comunitario sin fines comerciales de WalkerFans Team. Si algún contenido afecta a derechos de autor o patentes que desconozcamos, escribe a walkerfans007@gmail.com y lo retiraremos.
