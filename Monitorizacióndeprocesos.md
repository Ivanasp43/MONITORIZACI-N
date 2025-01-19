# Monitorización de Procesos
La monitorización de procesos en la administración de sistemas informáticos y redes, se centra en la observación y gestión de las aplicaciones y servicios que se ejecutan en un sistema. La monitorización de procesos permite supervisar las aplicaciones y servicios que se están ejecutando en un sistema. Esto es esencial para identificar cuellos de botella, procesos que consumen demasiados recursos y garantizar que los servicios críticos estén funcionando correctamente. En este apartado, se presentan las herramientas principales para analizar los procesos en tiempo real y realizar diagnósticos rápidos. Linux ofrece varias herramientas en línea de comandos para monitorizar el hardware: CPU, memoria, uso de disco duro y red.

### Algunas herramientas útiles son:
[### 1. TOP](ImagenesProcesos.md)
Herramienta que permite monitorizar los procesos del sistema en tiempo real, ver cuánto porcentaje de procesador se está usando, cuanta memoria se está usando y qué procesos lo están haciendo, además de conocer qué cantidad de memoria total tiene el sistema.
  - Sintáxis básica: *top [opciones]*
  - Opciones comunes
      - top T: Ordena los procesos según el tiempo total de CPU utilizado.
      - top M: Cambia la visualización de la memoria a unidades de Megabytes(MB).
      - top P: Ordena los procesos por uso de CPU (de mayor a menor porcentaje).
      - top R: Invierte el orden actual de la lista de los procesos.
      - top U: Filtra y muestra procesos de un usuario específico.
      - top q: Salida inmediata del programa *top*.
      - top k: Permite finalizar un proceso ingresando su PID.
        
<img width="638" alt="top" src="https://github.com/user-attachments/assets/2fddf2a2-40b6-4218-8854-edec304f82f0" />
<img width="638" alt="top_M" src="https://github.com/user-attachments/assets/8827ae59-a57f-4ad6-a73e-e9011f4e371a" />
<img width="640" alt="top_q" src="https://github.com/user-attachments/assets/99a04eb9-98e6-43d5-85ef-b4a7e75a8d25" />
<img width="640" alt="top_T" src="https://github.com/user-attachments/assets/ebe9b4dd-9068-430b-ab52-c8fe5e34fc0f" />
<img width="643" alt="top_k" src="https://github.com/user-attachments/assets/1a766eda-cd0b-4020-b556-9cb9aeeee907" />
<img width="637" alt="top_P" src="https://github.com/user-attachments/assets/ecf5d089-d569-40d9-89c9-e79f64fa3e7c" />
<img width="640" alt="top_R" src="https://github.com/user-attachments/assets/9f618c2b-c520-4f4c-b7d9-03b047d6851e" />
<img width="648" alt="top_U" src="https://github.com/user-attachments/assets/54282527-065a-4077-aabb-6b3049a48d02" />
### 2. HTOP
ES una herramienta con el mismo propósito que *top* pero más avanzada. Muestra algo más de información: permite ver los procesos del sistema, el consumo del procesador y la memoria que se está usando. TAmbién permite ver el uso del procesador por el núcleo de CPU.
Al igual que *top* permite ordenar la lista de procesos o uso de procesador, uso de memoria o, tipos de CPU consumidos en orden descendente o ascendente. Ofrece integración con el comando *lsof*.
  - Sintáxis básica: *htop [opciones] opciones*
  - Opciones comunes
      - htop -u <usuario>: Muestra sólo los procesos del usuario especificados.
      - htop --tree: Muestra los proceos en una vista jerárquica (en forma de árbol).
      - htop -p <PID1, PID2>: Filtra y monitorea procesos específicos por sus PID's
      - Atajos de teclados:
          - F2 (Setup)-Configuración
          - F3 (Search)-Búsqueda
          - F4 (Filter)-Filtro
          - F5 (Tree)-Vista en árbol
          - F6 (Sort)-Ordenar
          - F9 (Kill)-Terminar un proceso
### 3. PS
Este comando permite obtener información del estado de los procesos del sistema en el instante que se ejecuta. Posee varias opciones para filtrar los procesos que devuelve y su información de estado.
El comando *ps* proporciona una instantánea de los procesos en ejecución. Es útil para obtener información espedífica sobre procesos.
  - Sintáxis básica: *ps [opciones] opciones comunes*
      - ps a: Muestra todos los procesos asciados a la terminal, incluyendo los de otros usuarios.
      - ps aux: Lista todos los procesos del sistema, incluidos los que no están asociados a ninguna terminal
      - ps -C nano <nombre>: Muestra los procesos que coinciden con un nombre específico en el editor de texto.
### 4. ATOP
Se trata de una herramienta avanzada y versátil para monitorizar no sólo procesos, sino también otros recursos del sistema, como disco, red y memoria. Realiza un monitoreo en tiempo real, registro de datos, visualización flexible y alertas.
  - Síntaxis básica: *atop [opciones]*
      - atop -d <segundos>: Establece el intervalo de actualización en segundos.
      - atop -r <archivo>: Especifica un archivo para registrar datos.
      - atop -w: Activa el modo escritura, reemplazando el archivo de registro existente.
      - atop -D: Desactiva la visualización gráfica y muestra sólo datos en formato ASCII.
      - atop -n <número>: Establece el número de iteraciones antes de finalizar-
      - atop -s <fecha>: Inicia la visualización desde una fecha específica.

### Comparación entre herramientas

| Herramienta | Uso principal | Interfaz | Histórico |
|---|---|---|---|
| ps | Instantánea de procesos | No interactiva | No |
| top | Monitoreo en tiempo real | Interactiva | No |
| htop | Monitoreo en tiempo real | Interactiva y visual | No |
| atop | Monitoreo detallado y registros | Interactiva | Sí |

  
  
   
     
