# Monitorización del Almacenamiento
La monitorización del almacenamiento se refiere a la supervisión del uso de discos y sistemas de archivos, permite conocer el estado de los discos duros, particiones y sistemas de archivos. Es fundamental para prevenir problemas como falta de espacio, fallos en dispositivos de almacenamiento y para optimizar la gestión de los recursos disponibles. A continuación, se describen las herramientas básicas para analizar el uso del almacenamiento.

### Algunas herramientas útiles son:

[### 1. DF](https://github.com/user-attachments/assets/6e8d6d36-4cbb-48f0-911c-1cb069b89438)

El comando *df* permite ver información del almacenamiento de las unidades conectadas al sistema en el momento de ejecutar el comando. Permite ver cada una de ellas su capacidad total y espacio libre restante que le queda, dispositivo hardware, sus particiones y puntos de montaje.
  - Sintáxis básica: *df [opciones]*
  - Opciones comunes:
    
      [-df -h: ](https://github.com/user-attachments/assets/bb5a9671-8db6-423f-b16c-153bc875ccef) Muestra el tamaño de los sistemas de archivos en un formato legible para humanos (KB,MB,GB).
    
      [-df -T: ](https://github.com/user-attachments/assets/51806cb7-a41e-4fa1-9a88-c705bdefd9c0) Muestra el tipo de sistema de archivos (ext4,xfs...).
    
      [-df -x -tipoarchivo-: ](https://github.com/user-attachments/assets/5c2df9bf-2440-4de0-af03-39b96c7c32a0) Excluye sistemas de archivos del tipo especificado.

[### 2. DU](https://github.com/user-attachments/assets/3958c15a-2ffc-4d1e-a479-b69b6e5a1376)

Informa sobre el uso de espacio en disco de archivos y directorios.
  - Sintáxis básica: *du [opciones] [ruta]*
  - Opciones comunes:
    
    [-du -h: ](https://github.com/user-attachments/assets/a3add6cf-c89e-419b-93f6-d6de317d6ceb) Muestra el tamaño legible para humanos.
      
    [-du -s: ](https://github.com/user-attachments/assets/6295e53a-1a9b-4062-8f0a-6f992343e681) Muestra el tamaño total del directorio en lugar de listar cada subdirectorio.
      
    [-du -a: ](https://github.com/user-attachments/assets/649bbf8b-5772-4f04-8d67-ea590d52f614) Muestra el tamaño de cada archivo individual dentro de los directorios.
      
    [-du -c: ](https://github.com/user-attachments/assets/c880b3d5-a4aa-4fe3-a9d0-3849a83d96c3) Muestra el tamaño de los archivos/directorios y un total al final.
      
    [-du -sh: ](https://github.com/user-attachments/assets/c880b3d5-a4aa-4fe3-a9d0-3849a83d96c3) Muestra sólo el tamaño total del directorio.

[### 3. IOSTAT](https://github.com/user-attachments/assets/42d0b6fa-5e37-41c2-a4fa-1924f2b771cf)

Muestra las estadísticas de entrada/salida del sistema. Genera informes a nivel de dispositivo al monitorear el perídodo de tiempo activo en relación con las tasas de transferencia medias (medidas de rendimiento, uso, longitudes de cola, tasas de transacciones y tiempo de servicio). También muestra las estadísticas de la CPU.
  - Sintáxis básica: *iostat [opciones]*
  - Sintáxis compleja: *iostat [opciones] [intervalos] [repeticiones]*
  - Opciones comunes:
    
      [-iostat -c: ](https://github.com/user-attachments/assets/d06a43a3-bf4e-4905-aeb6-1b9ad701271f) Muestra estadísticas detalladas del uso de la CPU (usuario, sistema, inactivo, etc).
        
      [-iostat -d: ](https://github.com/user-attachments/assets/2ffa4d57-fd85-4b2c-8e1b-5d787c3f0190) Muestra estadísticas de entrada/salida por dispositivo de almacenamiento (lecturas, escrituras, etc).
        
      [-iostat -x: ](https://github.com/user-attachments/assets/9a98da98-f910-4671-b031-95b18518fca1) Proporciona estadísticas ampliadas y detalladas de cada dispositivo de almacenamiento, como el tiempo de espera y la utilización.
        
      [-iostat -t: ](https://github.com/user-attachments/assets/4321a0d5-8b04-4a5e-9c61-85775f47fa97) Incluye la marca de tiempo en la salida pra cada informe.
        
      [-iostat -p: ](https://github.com/user-attachments/assets/a06700a5-0e9d-4948-9ba3-f756dbd94e0e) Muestra estadísticas de las particiones de un dispositivo específico. Si no se especifica un dispositivo, incluye todas las particiones.
        
      [-iostat -s: ](https://github.com/user-attachments/assets/15bdee9d-7e02-476c-a4e6-8182cc2b2781) Muestra un resumen compacto del rendimiento del sistema, que incluye estadísticas generales de CPU, dispositivos y transferencia de datos.
        
      [-iostat -h: ](https://github.com/user-attachments/assets/5019cba6-27dd-4d9a-84ce-93a798be3589) Muestra las estadísticas en un formato más legible para humanos, utilizando unidades como KB, MB, GB, en lugar de bloques o valores sin contexto.
        
      [-iostat -free: ](https://github.com/user-attachments/assets/e694d455-487a-4541-9816-1e83213a7148) Permite ver la memoria física del sistema y la cantidad de memoria virtual o swap.
        
