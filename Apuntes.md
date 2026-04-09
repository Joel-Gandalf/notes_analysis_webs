# <span style="color:orange"><center> Spring 0 </span>
## <font color="orange">Funcionamiento de una web</font> <br>

![alt text](image.png) <br>

### Clientes <br>
Dispositivos de los usuarios conectados a internet con el software necesario para ello(navegador).<br>

### Servidores <br>
Computadores que almacenan páginas web, aplicaciones o sitios. <br>
Cuando el cliente accede a una página web se está descargando una copia de la página que visualiza mediante el navegador.<br>

### Agentes necesarios para la comunicación entre ``clientes y servidores:``<br>

+ __Conexión a Internet:__ permite enviar y recibir datos en la web. <br>

+ __TCP/IP(Protocolo de Control de Transmisión / Protocolo de Internet):__ Protocolos de comunicación que definen cómo deben viajar los datos. <br>

+ __DNS(Sistema de Nombres de Dominio):__ libreta de direcciones de sitios web. Direcciones de la página web buscada por el navegador que describen el servidor en el que se encuentra y su lugar en este para que el navegador pueda enviar los mensajes HTTP al lugar correcto. <br>

+ __HTTP(Protocolo de Transferencia de Hipertexto):__ Protocolo de Aplicación para definir un lenguage de comunicación entre Servidor y cliente. <br>

+ __Archivos componentes:__ Archivos que componen una web.  
  + ``` Archivos de código: ```construyen la web <br>
  + ``` Recursos: ``` Materiales(Imágenes,música...) <br>

### Procesos al demandar una dirección web en el navegador

1. El navegador acude al servidor DNS para encontrar la dirección real del servidor donde se aloja el sitio web.

2. El navegador envía un mensaje de petición HTTP al servidor, pidiéndole que envíe una copia de la página web para el cliente. Este mensaje y todos los datos enviados entre el cliente y el servidor, se envían a través de tu conexión a Internet usando TCP/IP.

3. Si el servidor aprueba la solicitud del cliente, enviará al cliente un mensaje ```«200 OK»```, que significa, «¡ Puedes ver ese sitio web! », y comenzará a enviar los archivos de la página web al navegador como una serie de pequeños trozos llamados paquetes de datos.

4. El navegador reúne los pequeños trozos, forma un sitio web completo y te lo muestra.

### Explicación de los DNS

Las direcciones webs reales no son secuencias que tecleas en la barra de direcciones para encontrar tus sitios webs. En realidad, se trata de secuencias de números, algo como 63.245.217.105.(```dirección IP```) y representa un lugar único en la web. Por eso se inventaron los servidores de nombres de dominio(```DNS```). Estos son servidores especiales que hacen coincidir una dirección web tecleada desde tu navegador con la dirección real del sitio web (IP).

Los sitios webs se pueden acceder directamente a través de sus direcciones IP. Puedes encontrar la dirección IP de un sitio web escribiendo su dominio en una herramienta como ```DNS lookup```.

### Explicación de los paquetes

 ```Paquetes```: formato en que los datos se envían desde el servidor al cliente. Los datos se envían a través de la web como miles de trozos pequeños, permitiendo que muchos usuarios pueden descargar la misma página web al mismo tiempo. Si los sitios web fueran enviados como grandes trozos, sólo un usuario podría descargarlos a la vez, lo que volvería a la web muy ineficiente.

 ## <font color="orange">¿Cómo funciona Internet?</font>

 Internet es la infraestructura técnica que hace posible la Web, mediante una gran red de computadoras que se comunican simultáneamente.

Comenzó en la década de 1960 como un proyecto de investigación financiado por el ejercito de los EE.UU, y luego se convirtió en una infraestructura pública en la década de 1980 con el apoyo de muchas universidades públicas y empresas privadas.

Internet es una forma de conectar las computadoras entre sí y asegurar que, pase lo que pase, encuentren una manera de mantenerse conectadas.

### La red

Vinculaciones para la comunicación entre ordenadores:
+ físicamente (por lo general con un cable de Ethernet)
+ inalámbrica (por ejemplo por WiFi o sistema de Bluetooth).

Una red no se limita a dos ordenadores, se pueden conectar tantos como se desee.  
La conexión por cable de todos ellos se volvería muy compleja. Por ello 
cada ordenador en una red está conectado a una pequeña computadora especial llamada enrutador(```router```).  
El router se encarga de asegurar que el mensaje enviado desde un ordenador emisor llegue al destino correcto.

ordenador -> A router -> ordenador B  

### Red de redes

Conectando ordenadores a enrutadores y luego enrutadores entre sí, podemos escalar infinitamente.
La infraestructura telefónica conecta tu casa con cualquier persona en el mundo, así que conectamos nuestra red a la infraestructura telefónica, mediante un equipo especial llamado ```modem```que convierte la información de nuestra red en información manejable por la infraestructura telefónica y viceversa.

A su vez conectaremos el modem a un proveedor de servicios de internet (```ISP``` de sus siglas en inglés ```Internet Service Provider```). Un ISP es una empresa que gestiona algunos enrutadores especiales interconectados, que también pueden acceder a enrutadores de otros ISP. Así, el mensaje de nuestra red es llevada a través de la red de redes de ISP, hasta la red de destino. Internet consiste en toda esta infraestructura de redes.

Ordenadores <-> router <-> modem <-> ISP <-> ISP <-> modem <-> router <-> Ordenadores

### Identificación de ordenadores

```Dirección IP```(Internet Protocol, o Protocolo de Internet): dirección única que identifica a un ordenador compuesta por una serie de cuatro números separados por puntos (192.168.2.10). 

Para enviar un mensaje a una computadora, se debe especificar a cuál. Por ello todo ordenador conectado a una red cuenta con una IP.

Para convertir esta serie numérica en algo que podamos asociar con mayor facilidad se utilizan los ```nombres de dominio```.

### Internet y la web

Internet es una infraestructura técnica que permite que miles de millones de ordenadores estén conectadas entre sí. Algunos de estos ordenadores, llamados servidores web son capaces de enviar mensajes inteligibles a los navegadores.  
Internet es una infraestructura, mientras que la Web es un servicio construido sobre dicha infraestructura.  
Existen otros servicios soportados por Internet, como el correo electrónico e IRC.

## <font color="orange"> Front end vs Back end</font>

El front end es aquello que ven los usuarios e incluye elementos visuales, como botones, casillas de verificación, gráficos y mensajes de texto. Permite a los usuarios interactuar con la aplicación. El back-end son los datos y la infraestructura que permiten que la aplicación funcione. Almacena y procesa los datos de las aplicaciones para los usuarios.

### Funcionamiento del front end en una aplicación

El Front end hace referencia a la interfaz gráfica de usuario (```GUI```) con la que los usuarios pueden interactuar de forma directa, (menús de navegación, los elementos de diseño, los botones, las imágenes y los gráficos).  
Una página o pantalla que el usuario ve con varios componentes de la interfaz de usuario se denomina ```modelo de objetos del documento (DOM)```.

Hay tres lenguajes de computación principales que afectan a la forma en que los usuarios interactúan con el front end:

+ El lenguaje ```HTML``` define la estructura del front end y los diferentes elementos del DOM
+ Las hojas de estilo en cascada (```CSS```) definen el estilo de una aplicación web, incluido el diseño, las fuentes, los colores y el estilo visual
+ ```JavaScript``` agrega una capa de funcionalidad dinámica mediante la manipulación del DOM

JavaScript puede activar cambios en una página y mostrar información nueva.  
Esto significa que el front end puede gestionar las interacciones (o solicitudes) fundamentales de los usuarios y transmite las solicitudes más complejas al back end.

### Funcionamiento del backend en una aplicación

A veces denominado servidor, el back end de la aplicación administra la funcionalidad general de la aplicación web. Cuando el usuario interactúa con el front end, la interacción envía una solicitud al back end en formato HTTP. El backend procesa la solicitud y devuelve una respuesta.

Cuando el backend procesa una solicitud, normalmente interactúa con los siguiente elementos:

+ ```Servidores de bases de datos``` para recuperar o modificar datos relevantes
+ ```Microservicios``` que realizan un subconjunto de las tareas solicitadas por el usuario
+ ```API de terceros``` para recopilar información adicional o realizar funciones adicionales

El backend:  
 + Utiliza varios protocolos y tecnologías de comunicación para completar una solicitud.  
 + Gestiona miles de solicitudes distintas de forma simultánea.  
 + Combina técnicas de concurrencia y paralelismo, como la distribución de solicitudes en muchos servidores, el almacenamiento en caché y la duplicación de datos.

el front end y el back end de la aplicación deben diseñarse de forma coherente para obtener los mejores resultados.

### Diferencias entre back end y front end 

__Objetivos de desarrollo:__

```full stack```: crear aplicaciones con buena capacidad de respuesta, eficientes y funcionales

```Front end```: desarrollar interfaces de usuario(GUI) con una interacción sencilla para el usuario, optimizar la aplicación en cuanto a accesibilidad y rendimiento, y crear diseños con capacidad de respuesta en diferentes plataformas y dispositivos.

```Back end```: crear y mantener las operaciones del lado del servidor de una aplicación con una arquitectura fiable y eficiente, cumpliendo con los requisitos de los usuarios, seguridad y costos.

__Tecnologías:__  

```Front end```: Marcos de trabajo(Frameworks)
```Back end```:
















