# Monitorización del Almacenamiento
La monitorización del almacenamiento se refiere a la supervisión del uso de discos y sistemas de archivos, permite conocer el estado de los discos duros, particiones y sistemas de archivos. Es fundamental para prevenir problemas como falta de espacio, fallos en dispositivos de almacenamiento y para optimizar la gestión de los recursos disponibles. A continuación, se describen las herramientas básicas para analizar el uso del almacenamiento.

### Algunas herramientas útiles son:

[### 1. DF]()

El comando *df* permite ver información del almacenamiento de las unidades conectadas al sistema en el momento de ejecutar el comando. Permite ver cada una de ellas su capacidad total y espacio libre restante que le queda, dispositivo hardware, sus particiones y puntos de montaje.
  - Sintáxis básica: *df [opciones]*
  - Opciones comunes
    
      [-df -h: ]() Muestra el tamaño de los sistemas de archivos en un formato legible para humanos (KB,MB,GB).
    
      [-df -T: ]() Muestra el tipo de sistema de archivos (ext4,xfs...).
    
      [-df -x tipo archivo: ]() Excluye sistemas de archivos del tipo especificado.

[### 2. DU]()

Informa sobre el uso de espacio en disco de archivos y directorios.
  - Sintáxis básica: *du [opciones] [ruta]*
  - Opciones comunes:
    
    [-du -h: ]() Muestra el tamaño legible para humanos.
      
    [-du -s: ]() Muestra el tamaño total del directorio en lugar de listar cada subdirectorio.
      
    [-du -a: ]() Muestra el tamaño de cada archivo individual dentro de los directorios.
      
    [-du -c: ]() Muestra el tamaño de los archivos/directorios y un total al final.
      
    [-du -sh: ]() Muestra sólo el tamaño total del directorio.

[### 3. IOSTAT]()

Muestra las estadísticas de entrada/salida del sistema. Genera informes a nivel de dispositivo al monitorear el perídodo de tiempo activo en relación con las tasas de transferencia medias (medidas de rendimiento, uso, longitudes de cola, tasas de transacciones y tiempo de servicio). También muestra las estadísticas de la CPU.
  - Sintáxis básica: *iostat [opciones]*
  - Sintáxis compleja: *iostat [opciones] [intervalos] [repeticiones]*
  - Opciones comunes:
    
      [-iostat -c: ]() Muestra estadísticas detalladas del uso de la CPU (usuario, sistema, inactivo, etc).
        
      [-iostat -d: ]() Muestra estadísticas de entrada/salida por dispositivo de almacenamiento (lecturas, escrituras, etc).
        
      [-iostat -x: ]() Proporciona estadísticas ampliadas y detalladas de cada dispositivo de almacenamiento, como el tiempo de espera y la utilización.
        
      [-iostat -t: ]() Incluye la marca de tiempo en la salida pra cada informe.
        
      [-iostat -p: ]() Muestra estadísticas de las particiones de un dispositivo específico. Si no se especifica un dispositivo, incluye todas las particiones.
        
      [-iostat -s: ]() Muestra un resumen compacto del rendimiento del sistema, que incluye estadísticas generales de CPU, dispositivos y transferencia de datos.
        
      [-iostat -h: ]() Muestra las estadísticas en un formato más legible para humanos, utilizando unidades como KB, MB, GB, en lugar de bloques o valores sin contexto.
        
      [-iostat -free: ]() Permite ver la memoria física del sistema y la cantidad de memoria virtual o swap.
        
