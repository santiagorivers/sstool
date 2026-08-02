# SS TOOL V1

Una herramienta avanzada de escaneo y screenshare diseñada para detectar clientes modificados, ghost clients y archivos ocultos (.jar) en entornos competitivos de Minecraft.

## Comandos de Ejecución (Consola / Terminal)

Para utilizar la herramienta, ejecuta el script principal seguido de cualquiera de los siguientes comandos de acción:

* **`py sstool.py -h`** o **`--help`**
  Muestra el menú de ayuda interactivo con la lista completa de comandos disponibles y su sintaxis.

* **`py sstool.py -j <ruta_del_archivo>`** o **`--scan-jar <ruta_del_archivo>`**
  Activa el análisis estructural de "Rayos X" en un archivo `.jar` específico. Descompone el contenedor en memoria para inspeccionar el manifiesto interno y el árbol de clases, anulando por completo las técnicas de evasión por cambio de nombre externo.

* **`py sstool.py -d`** o **`--scan-downloads`**
  Escanea de forma automatizada y recursiva toda la carpeta de Descargas del sistema operativo en busca de archivos `.jar` sospechosos que hayan sido movidos o modificados recientemente.

* **`py sstool.py -m`** o **`--scan-mods`**
  Rastrea directamente el directorio oficial de mods del juego (`%appdata%/.minecraft/mods`) para validar que todos los archivos instalados tengan una estructura legítima y libre de firmas de trampas.

* **`py sstool.py -b`** o **`--browser-history`**
  Inspecciona las bases de datos SQLite de los navegadores web del sistema (Brave, Google Chrome, etc.) para extraer el historial de descargas e identificar si el usuario interactuó con plataformas de distribución de hacks, incluso si los archivos ya fueron eliminados del disco duro.
