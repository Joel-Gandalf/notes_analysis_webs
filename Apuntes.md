# <span style="color:orange"><center> Spring 0 </span>
## <font color="orange">Funcionamiento de una web</font> <br>

<img src="image.png" alt="respuestas HTTP" style="width: 60%; height: auto; display:block; margin: 15px auto;">

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
  + ``Archivos de código:``construyen la web <br>
  + ``Recursos:`` Materiales(Imágenes,música...) <br>

### Procesos al demandar una dirección web en el navegador

1. El navegador acude al servidor DNS para encontrar la dirección real del servidor donde se aloja el sitio web.

2. El navegador envía un mensaje de petición HTTP al servidor, pidiéndole que envíe una copia de la página web para el cliente. Este mensaje y todos los datos enviados entre el cliente y el servidor, se envían a través de tu conexión a Internet usando TCP/IP.

3. Si el servidor aprueba la solicitud del cliente, enviará al cliente un mensaje ``«200 OK»``, que significa, «¡ Puedes ver ese sitio web! », y comenzará a enviar los archivos de la página web al navegador como una serie de pequeños trozos llamados paquetes de datos.

4. El navegador reúne los pequeños trozos, forma un sitio web completo y te lo muestra.

### Explicación de los DNS

Las direcciones webs reales no son secuencias que tecleas en la barra de direcciones para encontrar tus sitios webs. En realidad, se trata de secuencias de números, algo como 63.245.217.105.(``dirección IP``) y representa un lugar único en la web. Por eso se inventaron los servidores de nombres de dominio(``DNS``). Estos son servidores especiales que hacen coincidir una dirección web tecleada desde tu navegador con la dirección real del sitio web (IP).

Los sitios webs se pueden acceder directamente a través de sus direcciones IP. Puedes encontrar la dirección IP de un sitio web escribiendo su dominio en una herramienta como ``DNS lookup``.

### Explicación de los paquetes

 ``Paquetes``: formato en que los datos se envían desde el servidor al cliente. Los datos se envían a través de la web como miles de trozos pequeños, permitiendo que muchos usuarios pueden descargar la misma página web al mismo tiempo. Si los sitios web fueran enviados como grandes trozos, sólo un usuario podría descargarlos a la vez, lo que volvería a la web muy ineficiente.

 Webgrafía: [developer.mozilla.org](https://developer.mozilla.org/es/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works)

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
cada ordenador en una red está conectado a una pequeña computadora especial llamada enrutador(``router``).  
El router se encarga de asegurar que el mensaje enviado desde un ordenador emisor llegue al destino correcto.

ordenador -> A router -> ordenador B  

### Red de redes

Conectando ordenadores a enrutadores y luego enrutadores entre sí, podemos escalar infinitamente.
La infraestructura telefónica conecta tu casa con cualquier persona en el mundo, así que conectamos nuestra red a la infraestructura telefónica, mediante un equipo especial llamado ``modem``que convierte la información de nuestra red en información manejable por la infraestructura telefónica y viceversa.

A su vez conectaremos el modem a un proveedor de servicios de internet (``ISP`` de sus siglas en inglés ``Internet Service Provider``). Un ISP es una empresa que gestiona algunos enrutadores especiales interconectados, que también pueden acceder a enrutadores de otros ISP. Así, el mensaje de nuestra red es llevada a través de la red de redes de ISP, hasta la red de destino. Internet consiste en toda esta infraestructura de redes.

Ordenadores <-> router <-> modem <-> ISP <-> ISP <-> modem <-> router <-> Ordenadores

### Identificación de ordenadores

``Dirección IP``(Internet Protocol, o Protocolo de Internet): dirección única que identifica a un ordenador compuesta por una serie de cuatro números separados por puntos (192.168.2.10). 

Para enviar un mensaje a una computadora, se debe especificar a cuál. Por ello todo ordenador conectado a una red cuenta con una IP.

Para convertir esta serie numérica en algo que podamos asociar con mayor facilidad se utilizan los ``nombres de dominio``.

### Internet y la web

Internet es una infraestructura técnica que permite que miles de millones de ordenadores estén conectadas entre sí. Algunos de estos ordenadores, llamados servidores web son capaces de enviar mensajes inteligibles a los navegadores.  
Internet es una infraestructura, mientras que la Web es un servicio construido sobre dicha infraestructura.  
Existen otros servicios soportados por Internet, como el correo electrónico e IRC.

Webgrafía: [developer.mozilla.org](https://developer.mozilla.org/es/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work)

## <font color="orange"> Front end vs Back end</font>

El front end es aquello que ven los usuarios e incluye elementos visuales, como botones, casillas de verificación, gráficos y mensajes de texto. Permite a los usuarios interactuar con la aplicación. El back-end son los datos y la infraestructura que permiten que la aplicación funcione. Almacena y procesa los datos de las aplicaciones para los usuarios.

### Funcionamiento del front end en una aplicación

El Front end hace referencia a la interfaz gráfica de usuario (``GUI``) con la que los usuarios pueden interactuar de forma directa, (menús de navegación, los elementos de diseño, los botones, las imágenes y los gráficos).  
Una página o pantalla que el usuario ve con varios componentes de la interfaz de usuario se denomina ``modelo de objetos del documento (DOM)``.

Hay tres lenguajes de computación principales que afectan a la forma en que los usuarios interactúan con el front end:

+ El lenguaje ``HTML`` define la estructura del front end y los diferentes elementos del DOM
+ Las hojas de estilo en cascada (``CSS``) definen el estilo de una aplicación web, incluido el diseño, las fuentes, los colores y el estilo visual
+ ``JavaScript`` agrega una capa de funcionalidad dinámica mediante la manipulación del DOM

JavaScript puede activar cambios en una página y mostrar información nueva.  
Esto significa que el front end puede gestionar las interacciones (o solicitudes) fundamentales de los usuarios y transmite las solicitudes más complejas al back end.

### Funcionamiento del backend en una aplicación

A veces denominado servidor, el back end de la aplicación administra la funcionalidad general de la aplicación web. Cuando el usuario interactúa con el front end, la interacción envía una solicitud al back end en formato HTTP. El backend procesa la solicitud y devuelve una respuesta.

Cuando el backend procesa una solicitud, normalmente interactúa con los siguiente elementos:

+ ``Servidores de bases de datos`` para recuperar o modificar datos relevantes
+ ``Microservicios`` que realizan un subconjunto de las tareas solicitadas por el usuario
+ ``API de terceros`` para recopilar información adicional o realizar funciones adicionales

El backend:  
 + Utiliza varios protocolos y tecnologías de comunicación para completar una solicitud.  
 + Gestiona miles de solicitudes distintas de forma simultánea.  
 + Combina técnicas de concurrencia y paralelismo, como la distribución de solicitudes en muchos servidores, el almacenamiento en caché y la duplicación de datos.

el front end y el back end de la aplicación deben diseñarse de forma coherente para obtener los mejores resultados.

### Diferencias entre back end y front end 

__Objetivos de desarrollo:__

``full stack``: crear aplicaciones con buena capacidad de respuesta, eficientes y funcionales

``Front end``: desarrollar interfaces de usuario(GUI) con una interacción sencilla para el usuario, optimizar la aplicación en cuanto a accesibilidad y rendimiento, y crear diseños con capacidad de respuesta en diferentes plataformas y dispositivos.

``Back end``: crear y mantener las operaciones del lado del servidor de una aplicación con una arquitectura fiable y eficiente, cumpliendo con los requisitos de los usuarios, seguridad y costos.

__Tecnologías:__  

``Front end``: HTML, CSS, JavaScript, TypeScript y Marcos de trabajo (Frameworks).
``Back end``: Java, Python, Ruby, PHP y tecnologías de almacenamiento y de API.

__Simultaniedad:__

O ``concurrencia``: capacidad de una aplicación para ejecutar varias tareas de manera simultánea.

``Front end``: cada usuario tiene su propia copia de la aplicación en el navegador así que no hay problemas de concurrencia.  
``Back end``: es usual que se gestionen muchas peticiones de forma simultánea, por ello se usan diversas _estratégias_:
+ Subprocesos múltiples (gestión del procesamiento de tareas, CPU).
+ Programación asíncrona (devolución de llamadas y promesas).
+ Programación basada en eventos (escuchas de eventos y ejecuciónes de controladores de eventos de forma simultánea).
+ Bloqueo y sincronización (acceso sin inconsistencias al mismo recurso para varios usuarios de forma simultánea).

__Almacenamiento en Caché:__

Mejora el rendimiento y el tiempo de carga de una aplicación.

``Front end``: Los navegadores o las aplicaciones cliente almacenan en caché los archivos de la aplicación y los utilizan para mejorar el rendimiento.  
``Back end``: almacenamiento en caché en diferentes servidores o en una CDN (red de entrega de contenido) de diferentes contenidos para reducir la carga en el servidor.

__Seguridad:__  

``Front end``: validación de entradas en formularios, scripts en la parte del cliente y autentificación de usuario.  
``Back end``: protección de bases de datos, servicios de back end y la aplicación. (Mediante el uso de cifrado, sistemas de autenticación seguros y prácticas de codificación segura).

Webgrafía: [aws.amazon.com](https://aws.amazon.com/es/compare/the-difference-between-frontend-and-backend/#:~:text=El%20front%20end%20es%20aquello,permiten%20que%20la%20aplicaci%C3%B3n%20funcione)

## <font color="orange"> Generalidades del protocolo HTTP</font>

Hypertext Transfer Protocol: protocolo que permite hacer peticiones de datos y recursos.

Es la base de cualquier intercambio de datos en la Web, y un protocolo de estructura cliente-servidor.

Clientes y servidores se comunican intercambiando mensajes individuales (no flujos continuos de datos).

Tipos de mensaje:

+ ``Peticiones``  mensajes que envía el cliente, normalmente un navegador Web.
+ ``Respuestas`` mensajes enviados por el servidor.

Se conoce como un protocolo de la capa de aplicación, y se transmite sobre el protocolo ``TCP/IP``, o el protocolo encriptado ``TLS``, teóricamente podría usarse cualquier otro protocolo fiable. Es un protocolo __ampliable__.

Se usa para:
+ Transmitir documentos de hipertexto (HTML).
+ Transmitir imágenes o vídeos.
+ Enviar datos o contenido a los servidores, como en el caso de los formularios de datos.
+ Transmitir partes de documentos, y actualizar páginas Web en el acto.

![alt text](image-1.png)

### Arquitectura de los sistemas basados en HTTP

Arquitectura en capas de la Web basado en el principio de cliente-servidor.

+ El cliente envía una petición mediante el ``agente del usuario``(normalmente un navegador web, también puede ser otro programa que explore la web).

+ Cada petición individual se envía a un ``proxy``(a demás de otros agentes intermedios como routers, modems o ISP).

+ Los proxies envian las peticiones a los ``servidores`` correspondientes para que estos las gestionen y respondan.

__Proceso para mostrar una página Web__:   
El navegador envía una petición de documento HTML al servidor, procesa este documento y envía más peticiones para solicitar scripts, hojas de estilo (CSS), y otros datos que necesite (vídeos, imágenes...). El navegador, une todos estos documentos y datos, y compone la página Web.

__Proxies__:  
Existen distintos dispositivos que gestionan los mensajes HTTP.La mayoria solamente gestionan estos mensajes en los niveles de protocolo inferiores: capa de transporte, capa de red o capa física.  
Los proxies, en canvío, son dispositivos que operan procesando la capa de aplicación.

### HTTP y conexiones

HTTP _no necesita_ que el protocolo que lo sustenta mantenga una _conexión continua_ entre los participantes en la comunicación, solamente necesita que sea un protocolo fiable o que no pierda mensajes, un protocolo que sea capaz de detectar que se ha pedido un mensaje y reporte un error.

De los dos protocolos más comunes en Internet, TCP es fiable, UDP no lo es. Por lo tanto HTTP, se apoya en el uso del protocolo TCP.

### ¿Qué se puede controlar con HTTP?

Elementos que se pueden controlar con el protocolo HTTP:

+ ``Cache``: El como se almacenan los documentos en la caché. El servidor puede indicar a los proxies y clientes que almacenar y durante cuanto tiempo.

+ ``Flexibilidad del requisito de origen`` entre cliente y servidor: Para dar facilidades al servidor, ya que los navegadores Web sólo permiten compartir datos a páginas del mismo origen para proteger la privacidad de los usuarios. 
+ ``Autentificación``: HTTP provee de servicios básicos de autentificación. Para dar acceso sólo a usuarios autorizados.
+ ``Proxies y tunneling``: Servidores y/o clientes pueden usar intranets para esconder su dirección IP. Las peticiones HTTP utilizan los proxies para acceder a ellos.

### Flujo de HTTP

__Pasos:__

1. Abre una conexión TCP.
2. Hacer una petición HTTP.
3. Leer la respuesta enviada por el servidor.
4. Cierre o reuso de la conexión para futuras peticiones.

### Mensajes HTTP

__Peticiones__:

  <img src="http-request.svg" alt="peticiones HTTP" style="width: 50%; height: auto; display:block; margin: 15px auto;">

+ Un ``método HTTP``, normalmente un verbo, como: GET, POST o un nombre como: OPTIONS o HEAD, que defina la operación que el cliente quiera realizar. El cliente suele hacer una petición de recursos, usando GET, o presentar un valor de un formulario HTML, usando POST. También se pueden hacer otros tipos de peticiones.
+ La ``versión`` del protocolo HTTP.
+ La ``dirección del recurso pedido``; la URL del recurso, sin los elementos obvios por el contexto, como pueden ser: sin el protocolo (http://), el dominio (aquí developer.mozilla.org), o el puerto TCP (aquí el 80).
+ ``Cabeceras HTTP`` opcionales, que pueden aportar información adicional a los servidores.
+ O un ``cuerpo de mensaje``, en algún método, como puede ser POST, en el cual envía la información para el servidor.

__Respuestas:__

<img src="http-response.svg" alt="respuestas HTTP" style="width: 60%; height: auto; display:block; margin: 15px auto;">

+ La ``versión`` del protocolo HTTP que están usando.
+ Un ``código de estado``, indicando si la petición ha sido exitosa, o no, y debido a que.
+ Un ``mensaje de estado``, una breve descripción del código de estado.
+ ``Cabeceras HTTP``, como las de las peticiones.
+ Opcionalmente, el ``recurso que se ha pedido``.  

Webgrafía: [developer.mozilla.org](https://developer.mozilla.org/es/docs/Web/HTTP/Guides/Overview)

## <font color="orange"> Renderización en la Web</font>

La renderización web es el proceso técnico mediante el cual el navegador interpreta y traduce el código de una página(HTML, CSS y JavaScript) en la representación visual e interactiva que el usuario ve en pantalla. 

Webgrafía: [arimetrics.com](https://www.arimetrics.com/glosario-digital/renderizado-web#:~:text=Definici%C3%B3n:,cliente%20como%20el%20c%C3%B3digo%20JavaScript.)

### Fases clave del proceso de renderizado:

+ ``Análisis HTML``: Obtención y conversión del código HTML en el DOM (Modelo de Objetos del Documento), estructura. En él, cada etiqueta HTML genera identificadores de apertura y cierre (tokens) y los transforma en objetos nodo (node).
+ ``Análisis CSS``: Obtención y conversión del código CSS en el CSSOM (estilos) que se construye mediante las etiquetas CSS, las cuales se dividen en tokens y nodos. Como resultado se obtienen reglas de estilo estructuradas en forma de árbol.
+ Creación del ``Render Tree``: Unión de DOM y CSSOM para determinar qué se muestra.
+ ``Diseño`` (Layout): Cálculo de la posición y tamaño de cada elemento.
+ ``Pintura`` (Painting): Relleno de píxeles, colores, imágenes y textos en pantalla. 

Webgrafía: [publisuites.com](https://www.publisuites.com/blog/que-es-el-renderizado-de-paginas-web/)

### Tipos principales de renderización:

__Renderización del servidor (SSR):__
Renderizar una app en el servidor para enviar HTML, en lugar de JavaScript, al cliente.

__Renderización del cliente (CSR):__
Renderizar una app en un navegador con JavaScript para modificar el DOM y construir el contenido.

__Renderización previa:__
Ejecutar una aplicación del cliente en el momento de la compilación para capturar su estado inicial como HTML estático. la "renderización previa" es diferente de la _renderización previa del navegador de navegaciones futuras_.

__Hidratación:__
Ejecutar secuencias de comandos del cliente para agregar estado de la aplicación e interactividad al HTML renderizado por el servidor. La hidratación supone que el DOM no cambia.

__Rehidratación:__
A veces se utiliza como sinónimo de la hidratación. Implica actualizar el DOM con regularidad con el estado más reciente, incluso después de la hidratación inicial.

### Términos relativos al Rendimiento 

__Time to First Byte (TTFB):__
Es el tiempo que transcurre entre hacer clic en un vínculo y la carga del primer byte de contenido en la página nueva.

__First Contentful Paint (FCP):__
Es el momento en que el contenido solicitado (cuerpo del artículo, etcétera) se vuelve visible.

__Interaction to Next Paint (INP):__
Es una métrica representativa que evalúa si una página responde de forma coherente y rápida a las entradas del usuario.

__Total Blocking Time (TBT):__
Es una métrica proxy para INP que calcula cuánto tiempo se bloqueó el subproceso principal durante la carga de la página.

Webgrafía: [web.dev](https://web.dev/articles/rendering-on-the-web?hl=es-419)

## <font color="orange">Introducción a los frameworks del lado del cliente</font>

Un framework es una biblioteca que ofrece pautas sobre cómo se construye el software.

### Principales Frameworks:

+ Ember
+ Angular
+ Vue
+ React

El objetivo los frameworks de JavaScript es facilitar una ``mejor experiencia`` al desarrollador. No aportan nuevas funcionalidades a JavaScript, sino que facilitan el acceso a sus capacidades para que se puedan desarrollar aplicaciones web para el futuro.

Ofrecen una forma de escribir interfaces de usuario de manera ``más declarativa``. Es decir, permiten escribir código que describe mejor cómo debería verse la interfaz de usuario, y el framework se encarga de que esto suceda en el DOM de forma transparente.

Es posible hacer algo similar con JavaScript puro. Las ``plantillas literales`` facilitan la escritura de cadenas HTML que representan el aspecto final del elemento. Pueden ser útiles para tareas simples, pero no son viables para aplicaciones grandes.

### Qué ofrecen los frameworks?

+ Conjunto de herramientas(``tooling``): Estas facilitan la incorporación de funcionalidades como pruebas (para que la aplicación funcione correctamente) o análisis estático de código (busquedas de errores).
+ Compartimentación(``Compartmentalization``): facilitan a los desarrolladores la separación de las distintas partes de sus interfaces de usuario en componentes (fragmentos de código reutilizables y fáciles de mantener que pueden comunicarse entre sí).
+ Enrutamiento(``Routing``): Es posible crear un enrutador utilizando las capacidades nativas de JavaScript y del navegador, pero los frameworks cuentan con bibliotecas complementarias que hacen que el enrutamiento sea una parte más intuitiva del proceso de desarrollo.

Hay que tener en cuenta que un uso excesivo de estos puede aumentar el tamaño y el coste computacional del proyecto final, afectando al rendimiento de la página web o app.

Si las prioridades de los desarrolladores no son el rendimiento y la accesibilidad, los frameworks amplificarán la fragilidad, la sobrecarga y la inaccesibilidad.

Todos los frameworks mencionados admiten tanto la renderización del lado del servidor como la del lado del cliente.

### Alternativas

+ CMS: herramientas que permiten crear contenido web sin necesidad de escribir código.
+ Renderizado del lado del servidor.
+ Generadores de sitios estáticos: Utilización de plantillas

Webgrafía: [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Frameworks_libraries/Introduction)

## <font color="orange"> ¿Qué es una aplicación web progresiva?</font>

``PWA``(Progressive Web App): aplicación creada con tecnologías de plataforma web, que ofrece una experiencia de usuario similar a la de una aplicación específica de la plataforma.

### Aplicaciones específicas de la plataforma (Platform-specific apps)

Las aplicaciones específicas de plataforma se desarrollan para un sistema operativo (SO) o un tipo de dispositivo concreto, como iOS o Android.

Se descargan, instalan, y posteriormente se perciben como una función adicional permanente del dispositivo.

__Ventajas:__

+ ``Fácil acceso`` para los usuarios : Tienen su propio icono en el dispositivo, fácil de encontrar y abrir para los usuarios.
+ ``Funcionamiento sin conexión y en segundo plano`` : pueden operar incluso cuando el usuario no interactúa con ellas y el dispositivo está sin conexión. Esto permite que un chat reciba mensajes aunque la app no esté abierta y muestre una notificación al usuario. También permite que una aplicación se actualice en segundo plano para mostrar contenido nuevo incluso sin conexión.
+ ``Interfaz de usuario personalizada`` : Pueden implementar su propia interfaz de usuario distintiva e inmersiva.
+ ``Integración con el sistema operativo`` : Se pueden integrar en el sistema operativo anfitrión; una aplicación de mensajería puede registrarse como destino para compartir, permitiendo a los usuarios seleccionar una imagen en la aplicación de fotos y enviarla. También pueden acceder a funciones del dispositivo como la cámara, el GPS o el acelerómetro.
+ ``Integración con la App Store`` : Se distribuyen a través de la tienda de aplicaciones, ofreciendo a los usuarios un único lugar donde encontrarlas y la forma de decidir si quieren instalarlas.

### Sitios web tradicionales

Un sitio web: no tiene presencia en el dispositivo del usuario cuando este no accede a él, solo se puede acceder a él abriendo el navegador y navegando hasta el sitio, y depende en gran medida de la conectividad de red.

__Ventajas:__

+ ``Código base único`` : Dado que la web es inherentemente multiplataforma, un sitio web puede ejecutarse en diferentes sistemas operativos y clases de dispositivos a partir de un único código base.
+ ``Distribución a través de la web`` : La web es una excelente plataforma de distribución. Los motores de búsqueda indexan los sitios web, que se pueden compartir y acceder simplemente mediante URL. Un sitio web se puede distribuir sin necesidad de registrarse en la tienda de aplicaciones de ningún proveedor.

### Aplicaciones web progresivas

Las aplicaciones web progresivas combinan las mejores características de los sitios web tradicionales y las aplicaciones específicas de plataforma.

__Ventajas(web):__

+ Las PWA se desarrollan utilizando tecnologías estándar de plataformas web, por lo que ``pueden ejecutarse en múltiples sistemas operativos y clases de dispositivos`` a partir de un único código base.
+ Se puede acceder a las PWA directamente desde la web.

__Ventajas(app):__

+ Las PWA se pueden ``instalar en el dispositivo``.

  + Se pueden instalar desde la tienda de aplicaciones de la plataforma o directamente desde la web.
  + Permiten personalizar el proceso de instalación.
  + Una vez instalada, la PWA obtiene un icono de aplicación en el dispositivo, junto con las aplicaciones específicas de la plataforma.
  + Una vez instalada, la PWA se puede ejecutar como una aplicación independiente, en lugar de como un sitio web en un navegador.

+ Las PWA pueden ``funcionar en segundo plano y sin conexión``: un sitio web típico solo está activo mientras la página está cargada en el navegador. Una PWA puede:

  + Funcionar incluso cuando el dispositivo no tiene conexión a la red.
  + Actualizar el contenido en segundo plano.
  + Responder a los mensajes push del servidor.
  + Mostrar notificaciones mediante el sistema de notificaciones del sistema operativo.

+ Las PWA pueden ``usar toda la pantalla``, en lugar de ejecutarse en la interfaz de usuario del navegador.

+ Las PWA se pueden ``integrar en el dispositivo``, registrándose como destinos y fuentes para compartir contenido, y accediendo a las funciones del dispositivo.

### Las PWA y el navegador

Al visitar un sitio web en el navegador, este se ejecuta en él. La interfaz de usuario del navegador muestra un marco alrededor del sitio web, incluyendo elementos como botones de retroceso/avance y el título de la página. _Las API web que utiliza tu sitio web son implementadas por el motor del navegador._

Las PWA suelen tener la apariencia de aplicaciones específicas de la plataforma, pero desde un punto de vista tecnológico, siguen siendo sitios web. ``Necesitan un motor de navegador``, como los de Chrome o Firefox, ``para su gestión y ejecución``. 

En una aplicación específica de la plataforma, el sistema operativo gestiona la aplicación, proporcionando el entorno en el que se ejecuta.

En una PWA, el motor del navegador gestiona la aplicación en segundo plano, al igual que en los sitios web convencionales, proporcionando el entorno en el que se ejecuta.

### Características técnicas

Las PWA son sitios web y poseen las mismas características básicas:

+ Al menos una ``página HTML``, que probablemente carga CSS y JavaScript.
+ El JavaScript cargado por la página tiene ``un Window`` (objeto global) y puede acceder a todas las API web disponibles a través de dicho objeto.

__Características adicionales:__

+ Un ``archivo de manifiesto de la aplicación web``: como mínimo, proporciona la información que el navegador necesita para instalar la PWA, como el nombre y el icono de la aplicación.  

  También puede definir la apariencia de la PWA (color del tema y del fondo) y su comportamiento, incluyendo su capacidad para actuar como destino para compartir datos de otras aplicaciones o para manejar tipos de archivos específicos .

+ Opcionalmente, se puede contratar un sevice worker (trabajador de servicios) para ofrecer una experiencia ``sin conexión a internet``.

  Las páginas de la aplicación implementan la interfaz de usuario y el service worker implementa un backend que permite el funcionamiento sin conexión y en segundo plano.

### PWA y SPA (aplicaciones de una sola página)

Las PWA suelen implementarse como SPA.

En una aplicación de una sola página (SPA), el sitio consta de una única página HTML, cuando el usuario hace clic en enlaces internos, JavaScript se encarga de obtener el nuevo contenido del servidor y actualizar las partes relevantes de la página.

_Sólo se actualizan las partes relevantes a medida que interactúa con la aplicación._

_No todas las PWA son SPA._

### Mejora progresiva

Es una estrategia de diseño web que se enfoca en proporcionar una experiencia funcional básica a todos los usuarios (independientemente del navegador o dispositivo). Si el dispositivo y el navegador lo permiten añade capas de funcionalidades más avanzadas (como notificaciones push o funcionamiento offline) usando la detección de características para las API avanzadas.

Webgrafía: [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Guides/What_is_a_progressive_web_app#traditional_websites)

## <font color="orange">Tipologías de página web (Conclusiones)</font>

Las páginas estáticas muestran contenido fijo, son rápidas y seguras, ideales para sitios informativos simples. Las dinámicas generan contenido en tiempo real mediante bases de datos, permitiendo interacción (ej. redes sociales, e-commerce). Las PWA (Progressive Web Apps) combinan lo mejor de la web y aplicaciones nativas: funcionan sin conexión, cargan al instante y se instalan en el móvil.

Las SPA cargan una única página HTML inicial y actualiza dinámicamente el contenido mediante JavaScript, sin recargar el navegador. Ofrece una experiencia de usuario fluida y rápida, similar a una aplicación de escritorio.

### Diferencias clave:
__Páginas Web Estáticas:__

+ Funcionamiento: Archivos HTML/CSS y JS predefinidos servidos tal cual al navegador.
+ Contenido: Fijo. El mismo para todos los usuarios.
+ Actualización: Manual(desarrollador), editando el código de cada página.
+ Ventajas: Carga muy rápida, coste de desarrollo bajo, alta seguridad.
+ Uso: Portafolios, páginas de aterrizaje (landing pages), sitios corporativos informativos.

__Páginas Web Dinámicas:__

+ Funcionamiento: El contenido se genera en el servidor en tiempo real utilizando lenguajes como PHP, Python o Node.js y consultas a bases de datos para generar contenido al momento.
+ Contenido: Personalizado e interactivo. Cambia según el usuario (cookies, comportamiento).
+ Actualización: Automática a través de un gestor de contenidos (CMS) como WordPress.
+ Ventajas: Funcionalidades complejas (registros, carritos de compra, búsquedas).
+ Uso: Tiendas online (Amazon), redes sociales, blogs, sitios con alta interacción.

__PWA (Progressive Web Apps):__

+ Funcionamiento: Sitios web modernos que usan Service Workers para funcionar como apps.
+ Contenido: Dinámico, rápido y con capacidad de caché (funciona sin conexión o con baja conectividad).
+ Características: Instalables en el escritorio/móvil, envían notificaciones push y acceden a hardware (cámara, geolocalización).
+ Ventajas: Experiencia nativa, no requieren descarga desde la tienda de apps, menor costo de desarrollo que una app nativa.
+ Uso: Aplicaciones que requieren alta experiencia de usuario (ej. Twitter Lite, Pinterest).  

__Páginas web SPA__ (Single-Page Application o Aplicación de Una Sola Página):

+ Funcionamiento: Carga una única página HTML al inicio. Cuando el usuario interactúa, JavaScript actualiza solo la parte necesaria de la pantalla (DOM) utilizando tecnologías como AJAX; sin recargar todo el navegador.
+ Contenido: El contenido no viaja "pre-armado" desde el servidor. Lo que viaja son datos puros (normalmente en formato JSON) a través de APIs. La SPA toma esos datos y los "dibuja" en el navegador del usuario en tiempo real.
+ Actualización: reactiva; si cambias un dato, solo se actualiza ese componente o sección específica de la interfaz de forma invisible para el usuario.
+ Tecnologías comunes: Se suelen desarrollar con frameworks y librerías de JavaScript como React, Angular, Vue.js o EmberJS.
+ Ventajas: Navegación extremadamente rápida, excelente experiencia de usuario y menor consumo de ancho de banda tras la carga inicial. Reutilización: Al separar los datos del diseño, puedes usar la misma API para una web y una App móvil.
+ Desventajas: El SEO (posicionamiento en buscadores) es más complejo de optimizar, el tiempo de carga inicial puede ser mayor y depende del rendimiento del navegador del cliente. 
+ Uso: aplicaciones interactivas donde la velocidad y la experiencia de usuario son primordiales (Gmail, Facebook, Twitter, Netflix o Spotify).

__Resumen comparativo__

| Característica | Estática |	Dinámica	| SPA | PWA |  
| :--- | :---: | :---: | :---: | :---: | 
| Contenido | Fijo | Variable/Personalizado | Reactivo (JSON/APIs) | Dinámico/Interactivo |
| Interactividad |	Muy baja	| Alta | Muy alta |	Muy alta |
| Velocidad |	Muy rápida |	Media (depende del servidor)	| Inicial lenta Después Muy alta | Muy rápida (offline)
| Actualización |	Manual (código) |	CMS/Base de datos | Se actualiza por secciones	| Automática/En tiempo real Segundo Plano|
| Instalable |	No |	No | No |	Sí (añadir a pantalla inicio) |
| Uso Offline |	No |	No	| Limitado | Sí |
<br><br>
Webgrafía:

[mytaskpanel.com](https://www.mytaskpanel.com/paginas-web-estaticas-y-dinamicas/#:~:text=%C2%BFQu%C3%A9%20es%20una%20p%C3%A1gina%20web%20din%C3%A1mica?,de%20tr%C3%A1fico%20y%20datos%20din%C3%A1micos.)

[openWebinars.net](https://openwebinars.net/blog/paginas-web-estaticas-vs-paginas-web-dinamicas/)

[incentro.com](https://www.incentro.com/es-ES/blog/que-es-web-simple-page-applications)

[omatech.com](https://www.omatech.com/blog/2022/08/31/que-es-una-web-spa/)

[arsys.es](https://www.arsys.es/blog/spa-unica-pagina)


## <font color="orange"> Accessibilidad(WCAG) y SEO </font>

La accesibilidad (a11y) consiste en programar con estándares de calidad que permiten que cualquier persona (con ceguera, movilidad reducida o daltónica) use tu web.

### Puntos esenciales:

__Semántica HTML:__ Usar las etiquetas para lo que son. Un `<button>` es para acciones y un `<a>` para navegar. No uses un `<div>` con un onClick si puedes usar un botón, ya que los lectores de pantalla no sabrán que se puede pulsar.

__Contraste de color:__ El texto debe resaltar claramente sobre el fondo. La norma (WCAG) pide una relación mínima de 4.5:1. Puedes usar herramientas como Adobe Color para comprobarlo.

__Atributos alt en imágenes:__ Todas las imágenes deben tener una descripción breve. Si la imagen es puramente decorativa, deja el atributo vacío (alt=""), pero no lo omitas, para que el lector de pantalla sepa que debe saltársela.

__Navegación por teclado:__ Un usuario debería poder navegar por toda tu web solo usando la tecla Tab. Asegúrate de que el "foco" (el borde que rodea al elemento seleccionado) sea siempre visible y no lo quites con CSS (outline: none).

__Jerarquía de encabezados:__ Usa los `<h1>` a `<h6>` en orden lógico. No elijas un `<h3>` solo porque el tamaño de la letra te gusta más; úsalo porque es un subapartado de un `<h2>`. Los lectores de pantalla lo usan como un índice.

__Formularios etiquetados:__ Cada `<input>` debe tener su etiqueta <label> asociada mediante el atributo for. Esto permite que al clicar en el texto, el cursor salte al cuadro de escritura.

__Responsive y Zoom:__ La web no debe romperse si el usuario aumenta el tamaño de la fuente hasta un 200%. El diseño debe ser fluido.

## <font color="orange"> SEO </font>

__SEO (Search Engine Optimization):__ Preparar la estructura técnica para que los robots de Google (crawlers) entiendan y clasifiquen tu web correctamente.

### Puntos esenciales:

__Etiquetas de Título y Meta-descripción:__ Son lo primero que ve el usuario en Google. El `<title>` debe ser único por página y la `<meta name="description">` debe resumir el contenido para atraer el clic.

__Encabezados Semánticos (H1-H6):__ Solo debe haber un solo `<h1>` por página (el título principal). El resto (`<h2>`, `<h3>`) deben seguir un orden jerárquico, como el índice de un libro, para organizar los temas.

__Atributos ALT en Imágenes:__ Los buscadores no "ven" las imágenes. El texto alt les explica qué aparece en la foto, lo que te permite posicionar también en Google Imágenes.

__URLs Amigables:__ Evitar URLs con números raros (ej: page?id=123). Es mucho mejor usar "slugs" descriptivos como ://misitio.com.

__Velocidad de Carga (Core Web Vitals):__ Google penaliza las webs lentas. Como dev, debes optimizar el tamaño de las imágenes, minificar el código CSS/JS y usar técnicas como el Lazy Loading.

__Diseño Responsive (Mobile-First):__ Google indexa primero la versión móvil de tu web. Si no se ve bien en un smartphone o los botones están muy juntos, tu posicionamiento caerá.

__Enlazado Interno:__ Usa enlaces dentro de tu texto para conectar unas páginas con otras. Esto ayuda a Google a descubrir todo tu sitio y a entender qué páginas son las más importantes.

__Sitemap y Robots.txt:__ El archivo sitemap.xml es un mapa de todas tus páginas para el buscador, y el robots.txt le dice qué partes de la web NO debe rastrear (como el panel de administración).


## <font color="orange"> Conceptos </font>

### API

API (Application Programming Interface): Imagina que es el camarero de un restaurante. Tú (el cliente/frontend) le pides un plato (datos) de la carta; el camarero lleva el pedido a la cocina (el servidor) y te trae la comida de vuelta. Es el "puente" que permite que tu web hable con otros servicios para obtener información (como el tiempo, tweets o productos).

Una API es un conjunto de reglas, protocolos y definiciones que permite que dos aplicaciones de software se comuniquen entre sí. Actúa como una "interfaz" (un punto de conexión) donde el servidor expone ciertos puntos de acceso (Endpoints) y el cliente sabe exactamente qué datos enviar y qué formato de respuesta esperar.

__Flujo:__

+ Request (Petición): El Frontend realiza una llamada HTTP (usando fetch o axios) a una URL específica. Esta petición incluye un Método (GET para leer, POST para crear, PUT para actualizar, DELETE para borrar) y, a veces, cabeceras (headers) de autenticación.
+ Procesamiento: El servidor recibe la petición, consulta la base de datos o ejecuta una lógica de negocio.
+ Response (Respuesta): El servidor devuelve un código de estado (como el famoso 200 OK o el 404 Not Found) y, generalmente, un cuerpo de datos en formato JSON.

__Abstracción y Encapsulamiento:__
La API permite la abstracción. Como desarrollador frontend, no necesitas saber en qué lenguaje está escrito el backend (puede ser Python, Java o Go) ni cómo está organizada su base de datos. Solo necesitas conocer la documentación de la API para consumir los datos. Esto permite que el equipo de Backend cambie toda su estructura interna sin que tu código de Frontend se rompa, siempre que la interfaz de la API se mantenga igual.

### DOM

DOM (Document Object Model): Es la estructura de árbol que crea el navegador cuando carga tu código HTML. Al convertir las etiquetas (`<div>`, `<h1>`, etc.) en objetos de JavaScript, el DOM te permite "engañar" a la página: puedes usar código para cambiar un texto, borrar una imagen o mover un botón sin tener que editar el archivo HTML original.

### CMS

CMS (Content Management System): Es una herramienta de gestión para personas que no saben programar. En lugar de escribir código HTML para cada noticia de un blog, usan un panel visual (como WordPress) para escribir y subir fotos. El CMS guarda todo eso en una base de datos y lo muestra automáticamente en la web siguiendo una plantilla.

## <font color="orange"> Componentes principales que forman la arquitectura de un navegador</font>


1. __La Interfaz de Usuario (User Interface):__ 
Es todo lo que ves "fuera" de la ventana donde se carga la web. Incluye la barra de direcciones, el botón de atrás/adelante, el menú de marcadores y las pestañas. Es la única parte que no renderiza la web directamente. 

2. __El Motor del Navegador (Browser Engine):__
Es el "director de orquesta". Se encarga de gestionar las interacciones entre la Interfaz de Usuario y el Motor de Renderizado. Si le das a "Refrescar", él le dice al motor de renderizado que empiece de nuevo. 

3. __El Motor de Renderizado (Rendering Engine):__
Es la pieza más importante para un desarrollador Frontend. Su trabajo es "dibujar" la web.
Lee el HTML y el CSS.
Construye el DOM (árbol de elementos).
Calcula el diseño (Layout) y pinta los píxeles en la pantalla.
Ejemplos: Blink (Chrome, Edge), Gecko (Firefox) y WebKit (Safari). 

4. __El Motor de JavaScript (JS Engine):__
Como el HTML es estático, necesitamos un intérprete que entienda y ejecute tu código JavaScript. 
Transforma tu código JS en algo que el procesador del ordenador pueda entender rápidamente (compilación Just-In-Time).
Ejemplos: V8 (Chrome/Edge/Node.js), SpiderMonkey (Firefox).

5. __Backend de Red (Networking):__
Es el componente que se encarga de las comunicaciones por internet. Gestiona las peticiones HTTP/HTTPS, las DNS y la seguridad (certificados SSL). Es quien "va a buscar" los archivos al servidor.

6. __Almacenamiento de Datos (Data Storage):__
El navegador necesita guardar cosas en tu disco duro para no pedirlas siempre al servidor. Aquí se gestionan: 
    + Cookies.
    + LocalStorage y SessionStorage.
    + IndexedDB (bases de datos locales).
    + Caché de archivos. 

7. Capa de Interfaz con el Sistema Operativo (UI Backend)
Es una capa interna que usa los métodos del sistema operativo (Windows, macOS, Linux) para dibujar ventanas básicas, menús desplegables o cuadros de selección de archivos. 

__Al poner una URL y dar a Enter:__

+ La Red descarga el archivo.
+ El Motor de Renderizado lee el HTML y crea el DOM.
+ El Motor de JS ejecuta los scripts.
+ El Motor de Navegador coordina que todo aparezca en la Interfaz.

## <font color="orange"> Seguridad básica </font>

### HTTPS, Cross-Site Scripting (XSS) 
### Cross-Origin Resource Sharing (CORS)



## <font color="orange"><center>Análisis de aplicaciones</font>

### Amazon :

| Criterio | Descripción |
|:---|:---|
| Tipología| 	Dinàmica/híbrida (Multi-Page Application - MPA) con fragmentos de comportamiento SPA y PWA|
| URL | https://www.amazon.es/ |
| Evidencias técnicas | <ul><li>No es una SPA pura porque cada sección principal (Home, Producto, Checkout) implica una carga de documento nuevo, aunque usa AJAX para actualizar estados internos como el filtrado de productos o el despliegue de reseñas.</li><li>Manifiesto de Aplicación (manifest.json): Aunque Amazon tiene archivos de configuración, no siempre expone el banner de "Instalar en pantalla de inicio" que caracteriza a las PWA. Su estrategia de negocio es empujarte a la App Nativa.</li> <li>Service Workers: Amazon los usa masivamente para el almacenamiento en caché de recursos críticos y para que la página cargue rápido, pero no ofrece una experiencia offline completa (no puedes comprar sin internet), Por ello no se considera una PWA.</li> <li> SSR (Server Side Rendering): El HTML inicial llega renderizado desde el servidor para optimizar SEO y LCP (no es un div vacío como en un React básico).</li> <li>Arquitectura de Micro-frontends: Diferentes secciones (carrito, buscador...) son servicios independientes integrados en la interfaz, si uno falla, el otro sigue funcionando.</li> <li>Imágenes de próxima generación: Uso de formatos .webp y lazy-loading nativo.</li></ul> |
| Comportamiento de navegación | 	Navegación hibrida. El flujo principal es síncrono (recarga de página), pero las interacciones de filtrado, paginación de reseñas y el "Añadir a la cesta" son asíncronas (AJAX/Fetch), manteniendo el estado sin refrescar la ventana.|
| Tiempo de carga |276 requests 13.9 MB transferred 19.6 MB resources Finish: 1.2 min DOMContentLoaded: 1.72 s Load: 3.10 s|
| Interacción con el servidor | APIs y CDNs |

### Blog personal de WordPress :

| Criterio | Descripción |
|:---|:---|
| Tipología| 	Dinàmica / CMS (Content Management System) tradicional. |
| URL | https://humanidadymedio.wordpress.com/ |
| Evidencias técnicas| <ul><li>Estructura clásica donde el servidor (PHP) genera el HTML en cada solicitud.</li> <li>Contenido personalizado e interactivo. Cambia según el comportamiento del usuario</li> <li>Actualización automática a través de un gestor de contenidos (CMS), WordPress</li> <li>WordPress: Rutas /wp-content/ y generador WordPress.com.</li> <li>Jetpack: Plugins integrados para estadísticas/seguridad.</li> <li>Temas predefinidos: Clases CSS estándar (.site-header, .entry-content).</li></ul> |
| Comportamiento de navegación | Navegació Síncrona (MPA, Multi-Page Application Clàssica). Recarga la página completa en cada navegación; sin transiciones suaves de JS. |
| Tiempo de carga |36 requests 728 kB transferred 1.4 MB resources Finish: 1.58 s DOMContentLoaded: 1.05 s Load: 1.49 s|
| Interacción con el servidor | 	PHP / MySQL via Servidor Remot. El servidor monta el HTML con PHP y lo envía; sin API moderna separada. |

### Portafolio estático :

| Criterio | Descripción |
|:---|:---|
| Tipología|  Estática, Static Site Generator (SSG)/ SPA  |
| URL | https://www.shcherban.com/ |
| Evidencias técnicas| <ul><li>Al entrar en DevTools > Network y hacer clic en un enlace de su menú, no se descarga un archivo html, sino un pequeño archivo de datos (JSON) o un fragmento de JavaScript.</li> <li>Es Estática porque el contenido no cambia según quién lo mire (no hay login, ni nada personalizado). El contenido es el mismo para todos y está pre-calculado.<li>Es SPA en su comportamiento porque utiliza un "Router" de JavaScript para cambiar lo que se ve en pantalla sin que la pestaña del navegador haga amago de recarga.</li> <li>Tecnología moderna: Está construida con Next.js o Gatsby (se nota por el pre-fetching de enlaces).</li> <li>Imágenes optimizadas: Usa componentes de imagen avanzados que cargan versiones pequeñas primero (blur-up effect).</li> <li>Gestión de estado: Si inspeccionas el código, verás que el contenido está inyectado mediante JavaScript hidratado sobre un HTML base.</li></ul> |
| Comportamiento de navegación | Navegació Instantània (Client-side routing). Al hacer clic en un proyecto, no hay petición de una nueva página HTML al servidor; JavaScript captura el clic y cambia el componente visual. Da una experiencia fluida. |
| Tiempo de carga | 21 requests 1.4 MB transferred 1.6 MB resources Finish: 1.11 s DOMContentLoaded: 702 ms Load: 983 ms |
| Interacción con el servidor | Mínima / Pre-renderizada. El servidor no "piensa". Todo el trabajo duro se hizo cuando el desarrollador pulsó "build". Durante la navegación, el cliente (navegador) solo descarga pequeños archivos JSON con la información de cada sección. |

### Airbnb :

| Criterio | Descripción |
|:---|:---|
| Tipología| 	Dinàmica / SPA (Single Page Application). Una de las implementaciones de React más avanzadas, priorizando la experiencia fluida de "app nativa" sobre la navegación tradicional. |
| URL | https://www.airbnb.es/ |
| Evidencias técnicas| <ul><li>React & TypeScript: Uso masivo de componentes reutilizables.</li> <li>Client-side Rendering (CSR): Navegación sin recargar la página tras la carga inicial.</li> <li>PWA: Service Workers para carga rápida y funcionamiento en conexiones débiles.</li> <li>Skeleton Screens: Visualización de componentes mientras cargan los datos.</li></ul> |
| Comportamiento de navegación | Navegació Instantània i Líquida. Actualización en milisegundos de filtros y mapas sin parpadeos de página. Descarga progresiva de imágenes a medida que el usuario hace scroll. |
| Tiempo de carga | 267 requests 4.1 MB transferred 12.3 MB resources Finish: 25.15 s DOMContentLoaded: 2.08 s Load: 11.62 s|
| Interacción con el servidor | APIs GraphQL / REST. Intercambio constante de datos (JSON) con uso de CDN para una rápida respuesta global. |

Airbnb utiliza una arquitectura SPA (Single Page Application) avanzada basada en React, TypeScript y Next.js para ofrecer una experiencia de usuario fluida, caracterizada por la carga dinámica de componentes y la gestión eficiente de datos. La plataforma optimiza el rendimiento mediante lazy loading de imágenes y el uso de service workers (PWA) para garantizar interactividad instantánea sin recargas de página.

### Twitter :

| Criterio | Descripción |
|:---|:---|
| Tipología| SPA/PWA |
| URL | https://x.com/?lang=es |
| Evidencias técnicas|  <ul><li>Es una aplicación de una sola página cargada con JavaScript. Cumple todos los requisitos de una PWA (Progressive Web App): es instalable, tiene notificaciones push y funciona casi como una app nativa.</li> <li>React.js: Toda la interfaz se basa en componentes React (puedes verlo en el código con clases que empiezan por css-).</li> <li>Service Workers activos: Si abres DevTools > Application, verás que hay procesos en segundo plano para manejar caché y notificaciones.</li> <li>Infinite Scroll: Implementación técnica donde el DOM se recicla para no saturar la memoria mientras bajas por el feed.</li></ul> |
| Comportamiento de navegación | Asíncrona Total. Al moverte entre "Inicio", "Explorar" o tu "Perfil", la página nunca se recarga. El navegador solo pide los datos (tweets) al servidor y React redibuja la pantalla. La sensación es de fluidez absoluta. Carga por fases (App Shell). Primero carga el "esqueleto" y luego van apareciendo los tweets. Usa Streaming SSR para que el contenido llegue lo antes posible al usuario.|
| Tiempo de carga | 116 requests 4.9 MB transferred 17.7 MB resources Finish: 27.21 s DOMContentLoaded: 2.45 s Load: 2.77 s |
| Interacción con el servidor | WebSocket / Real-time APIs. A diferencia de un blog, X necesita saber si tienes un nuevo "like" o tweet al segundo. Usa conexiones persistentes para recibir datos en tiempo real sin que tú tengas que refrescar nada. |

Diferencia con Amazon:

Instalable: Si entras desde el móvil o Chrome, te aparecerá un icono en la barra de direcciones para "Instalar X". Una vez hecho, se abre en una ventana sin barras de navegador.
Offline (parcial): Sin conexión, puedes seguir viendo los tweets que ya se habían cargado porque el Service Worker los guardó en el almacenamiento local de tu navegador.
App Shell: El diseño de la interfaz se queda guardado en tu dispositivo; solo se descargan los datos nuevos (los tweets).


### Página de documentación de MDN :

| Criterio | Descripción |
|:---|:---|
| Tipología|	Dinàmica / Jamstack (Yari)|
| URL | https://developer.mozilla.org/es/docs/Web/HTTP/Guides/Overview |
| Evidencias técnicas| <ul><li>Aunque parece una web tradicional, utiliza una arquitectura moderna llamada Yari. Es un sitio generado estáticamente (SSG) pero con una capa dinámica de React para la búsqueda y la interactividad.</li> <li>React: Se utiliza para gestionar la navegación entre artículos y el buscador.</li> <li> GitHub-backed Content: El contenido no está en una base de datos SQL típica, sino en archivos Markdown en GitHub.</li> <li>Hydration: El HTML llega listo del servidor (para SEO) y luego JavaScript "toma el control" para permitir búsquedas rápidas.</li></ul> |
| Comportamiento de navegación | Híbrid (SPA-like). Con clic en enlaces laterales la página no se recarga totalmente de forma brusca; usa un sistema de rutas (Client-side routing) para que la transición sea suave, pero manteniendo URLs únicas para cada documento. |
| Tiempo de carga | 99 requests 894 kB transferred 1.8 MB resources Finish: 2.37 s DOMContentLoaded: 407 ms Load: 1.03 s |
| Interacción con el servidor | APIs de Busqueda y Contribución. El servidor apenas trabaja para servir el contenido (son archivos estáticos), pero se comunica con APIs para el autocompletado del buscador y para mostrar el estado de las traducciones. |



