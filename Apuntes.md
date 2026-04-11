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

