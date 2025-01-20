# Monitorización de la red
La monitorización de red es el uso de software de monitorización de red para monitorizar el estado y la fiabilidad de una red informática. Los sistemas de monitorización del rendimiento de la red (NPM) suelen generar mapas de topología e información práctica basada en los datos de rendimiento recopilados y analizados.
Como resultado de esta asignación de red, los equipos de TI obtienen una visibilidad completa de los componentes de la red, la monitorización del rendimiento de las aplicaciones y la infraestructura de TI relacionada. Esta visibilidad les permite realizar un seguimiento del estado general de la red, detectar señales de alerta y optimizar el flujo de datos.
Un sistema de monitorización de red vigila los dispositivos de red que funcionan mal y los recursos sobrecargados. El sistema hace esto independientemente de si los recursos de red están en las instalaciones, en un centro de datos, alojados por un proveedor de servicios en la nube o forman parte de un ecosistema híbrido. Por ejemplo, puede encontrar CPU sobrecargadas en servidores, altas tasas de error en conmutadores y enrutadores, o picos repentinos en el tráfico de red. Una característica clave del software NPM es alertar a los administradores de red cuando se detecta un problema de rendimiento.           
Los sistemas de monitorización de red también recopilan datos para analizar el flujo de tráfico y medir el rendimiento y la disponibilidad. Una forma de monitorizar los problemas de rendimiento y los cuellos de botella es configurar umbrales, de modo que reciba alertas inmediatas cuando se supere un umbral. Algunos umbrales son simples umbrales estáticos. Sin embargo, los sistemas NPM modernos utilizan el machine learning (ML) para determinar el rendimiento normal en todas las métricas de una red en función de la hora del día y el día de la semana. Los sistemas NPM con estas líneas de base basadas en ML crean alertas que, por lo general, son más procesables.
¿Por qué es necesaria?
Los fallos de red pueden provocar interrupciones en el negocio, lo que puede significar una pérdida de clientes, productividad de los empleados y dinero. De hecho, el 91 % de las empresas medianas y grandes afirman que una sola hora de tiempo de inactividad de TI les cuesta al menos 300 000 dólares por hora.
La monitorización de la infraestructura le permite saber con precisión dónde se produce un problema de red, lo que permite solucionarlo antes de que la situación provoque una interrupción. La identificación temprana y la resolución de la causa raíz de un problema pueden reducir el tiempo de respuesta, mejorar la satisfacción del cliente, ahorrar dinero y proteger la reputación de una empresa.

### Algunas herramientas básicas son:

[### 1. TCPTRACK -i nombreRed]()

Comando poco conocido, nos muestra todos los datos del consumo de nuestra conexión. Se trata de un comando de monitorización de la red y de los paquetes que se envíen y reciban que, además, permite realizar pruebas de velocidad en internet. Se utiliza para monitorear conexiones TCP en tiempo real, mostrando estadísticas como dirección IP, puerto, estado de la conexión y el ancho de banda utilizado.

  - Sintáxis básica: *tcptrack -i [nombreRed] [opción]*
  - Opciones comunes:
    
      [-tcptrack -i nombreRed -c: ]() Desactiva los colores en la salida.
        
      [-tcptrack -i nombreRed -a: ]() Muestra todas las conexiones, incluidas cerradas o en espera.
        
      [-tcptrack -i nombreRed -n: ]() No resuelve nombres de host, mostrando sólo direcciones IP.
        
      [-tcptrack -i nombreRed -t: ]() Ajusta el intervalo de actualización en segundos (por defecto es 1 segundo).
        
      [-tcptrack -i nombreRed--p: ]() Proporciona detalles adicionales sobre las conexiones activas.
        
      [-tcptrack -i nombreRed -l: ]() Ajusta la longitud de la ventana de salida.

[### 2. NETSTAT](https://github.com/user-attachments/assets/debfb1dd-0da0-4201-8448-35f49b9347f0)

Este comando permite ver cuáles son las conexiones de red establecidas por los procesos del sistema y su estado. Se utiliza para mostrar estadísticas de red, conexiones activas, tablas de enrutamiento, interfaces de red y más. Es una herramienta común para diagnosticar problemas de red y monitorear actividad.

  - sintáxis básicas: *netstat [opciones]*
  - Opciones comunes:
    
      [-netstat -a: ](https://github.com/user-attachments/assets/5edaf04f-51a6-4f3f-8ffc-fd77b0309b5f) Muestra todas las conexiones y puertos en encucha (listening).
        
      [-netstat -t: ](https://github.com/user-attachments/assets/c8c76203-45fc-44d7-a98b-4da882a8c585) Muestra únicamente las conexiones TCP activas.
        
      [-netstat -u: ](https://github.com/user-attachments/assets/bd82339f-a4b2-4a6b-9b6d-1e015b05a9a6) Muestra únicamente las conexiones UDP activas.
        
      [-netstat -n: ](https://github.com/user-attachments/assets/05bb5622-eacb-4a69-8b24-7a75a9f3dff7) Muestra direcciones y puertos en formato numérico en lugar de resolver nombres.
        
      [-netstat -l: ](https://github.com/user-attachments/assets/7b710c13-c382-4dc3-a81a-752d3458ed42) Muestra sólo los puertos de escucha.
        
      [-netstat -p: ](https://github.com/user-attachments/assets/5b5c4e86-f407-48bf-9f65-a5ff66736d22) Muestra el PID y el nombre del programa asociado a cada conexión.
        
      [-netstat -r: ](https://github.com/user-attachments/assets/15ef214e-434e-4bfc-a377-9b6108e0895c) Muestra la tabla de enrutamiento del kernel.
        
      [-netstat -i: ](https://github.com/user-attachments/assets/963d2499-a609-4c16-a27b-1c7fccf32b3b) Muestra estadísticas de las interfaces de red.
        
      [-netstat -s: ](https://github.com/user-attachments/assets/d766ee4a-07dc-4d78-8202-5e8ddcd794c0) Muestra estadísticas detalladas de protocolos, como TCP, UDP e ICMP.
        
      [-netstat -c: ](https://github.com/user-attachments/assets/eeb83549-15d3-4fa5-8636-46bc666c0884) Actualiza la salida de manera continua en intervalos.
        
[### 3. IPTRAF](https://github.com/user-attachments/assets/f7d04140-4d67-4bb9-a1d7-9da40fd44167)

Se trata de una herramienta muy interesante y útil para monitorizar las redes IP y donde se puede usar para monitorizar la carga en la red. Iptraf intercepta paquetes en la red y muestra información sobre el tráfico. Se trata de una herramienta interactiva para monitorear el tráfico de red en tiempo real. Proporciona estadísticas detalladas de conexiones, ancho de banda y uso de interfaces.
  - Sintáxis básica: *iptraf [opciones]*
  - Opciones comunes:
    
      [-iptraf -i <interfaz>: ](https://github.com/user-attachments/assets/0f15a519-788d-4dc0-9dd9-731acbce981b) Monitorea el tráfico en una interfaz específica.
        
      [-iptraf -d <interfaz>: ]() Muestra un resumen detallado de las estadísticas de tráico por una interfaz.
        
      [-iptraf -s: ]() Muestra un resumen general del sistema, incluyendo tráfico en todas las interfaces.
        
      [-iptraf -l: ]() Inicia un monitoreo en modo log, almacenando los resultados en un archivo de registro.

[### 4. TCPDUMP]()

El comando tcpdump permite capturar el tráfico de red de una interfaz de red, para un puerto de red o para un nombre de host como origen o destino específico. Se trata de una herramienta muy poderosa para capturar y analizar el tráfico de red. Es muy utilizado para depuración de redes y monitoreo en tiempo real.

  - Sintáxis básica: *tcpdump [opciones] [filtro]*
  - Opciones comunes:
    
      [-tcpdump -i <interfaz>: ]() Especifica la interfaz de red en la que se realizará la captura.
        
      [-tcpdump -n: ]() Evita resolver nombres de host y mustra direcciones IP en formato numérico.
        
      [-tcpdump -c <número>: ]() Captura un número específico de paquetes.
        
      [-tcpdump -w <archivo>: ]() Guarda los paquetes capturados en un archivo.
        
      [-tcpdump -r <archivo>: ]() Analiza un archivo de captura existente.
        
      [-tcpdump -v, -vv, -vvv: ]() Aumenta el nivel de detalle en la salida.
