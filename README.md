# 🌐 Trabajo Práctico Teórico — Programación sobre Redes

<br></br>
<div align="center">

<img src="img/logo-ifts18.png" width="180px">
<br></br>

## Instituto de Formación Técnica Superior N°18

</div>

**Institución:** IFTS 18  
**Carrera:** Técnico Superior en Desarrollo de Software  
**Profesor:** Lucas Rusatti  
**Grupo:** D

</div>


<div align="center">
  
## 👥 Integrantes

</div>

* **Diego Murgana** 
* **Leandro Sosa**
* **Agustín Senin**
* **Santiago Padilla**  


<br></br>

## 📍 Índice de Contenidos

| N° | Pregunta | N° | Pregunta | N° | Pregunta |
|:---:|:---|:---:|:---|:---:|:---|
| 1 | [¿Qué es una VLAN?](#1-qué-es-una-vlan) | 12 | [Tecnologías Wireless](#12-tecnologías-wireless-y-sus-estándares) | 23 | [Microsoft Teams](#23-explique-la-solución-de-microsoft-teams) |
| 2 | [¿Qué es una VPN?](#2-qué-es-una-vpn) | 13 | [¿Qué es un Proxy?](#13-qué-es-un-proxy) | 24 | [Calidad en enlace MPLS](#24-qué-significa-aplicar-calidad-en-un-enlace-mpls) |
| 3 | [¿Qué es una SAN?](#3-qué-es-una-san) | 14 | [Protocolo Spanning Tree](#14-protocolo-spanning-tree) | 25 | [Coaxial, UTP y Fibra](#25-diferencias-entre-coaxial-utp-y-fibra) |
| 4 | [Hub, Repetidor, Router y Switch](#4-diferencias-entre-un-hub-repetidor-router-y-switch) | 15 | [Protocolo OSPF](#15-protocolo-de-comunicaciones-ospf) | 26 | [Certificaciones Cisco](#26-según-cisco-qué-significa-ccent-ccna-y-ccnp) |
| 5 | [Protocolo de Comunicaciones](#5-qué-es-un-protocolo-de-comunicaciones) | 16 | [Protocolo ARP](#16-protocolo-arp) | 27 | [Modelo OSI](#27-explique-el-modelo-osi) |
| 6 | [TCP/IP y NetBios](#6-explique-tcpip-y-netbios-resuma-sus-diferencias) | 17 | [¿Qué es un Firewall?](#17-qué-es-un-firewall) | 28 | [Estándar IEEE 802.3](#28-estándar-ieee-8023) |
| 7 | [Paquete TCP/IP y Flags](#7-cómo-está-formado-un-paquete-de-datos-en-tcpip-qué-es-un-flag) | 18 | [¿Qué es una DMZ?](#18-qué-es-una-dmz) | 29 | [Estándar IEEE 802.4](#29-estándar-ieee-8024) |
| 8 | [Red según Geografía](#8-defina-la-red-según-su-geografía-explicar-distintas-variantes) | 19 | [¿Qué es un Gateway?](#19-qué-es-un-gateway) | 30 | [Protocolos de correo](#30-protocolos-para-enviar-y-recibir-correo) |
| 9 | [Red según Topología](#9-defina-una-red-según-su-topología-explicar-distintas-variantes) | 20 | [¿Qué significa NBL?](#20-según-microsoft-qué-significa-nbl) | 31 | [Protocolo para leer correo](#31-protocolo-para-leer-correo-recibido) |
| 10 | [Servicio DHCP](#10-explicar-el-servicio-de-dhcp) | 21 | [Tipos de enlace](#21-tipos-de-enlace-mpls-lan-to-lan-microonda-vsat) | 32 | [IPv4 vs IPv6](#32-diferencias-entre-ipv4-e-ipv6) |
| 11 | [Servicio DNS](#11-explicar-el-servicio-de-dns) | 22 | [Tecnología LTE](#22-describir-la-tecnología-lte) | 33 | [Experiencia Personal](#33-experiencia-en-redes-por-integrante) |


<br></br>

<div align="center">

# 📖 Desarrollo del Cuestionario

</div>


## 1. ¿Qué es una VLAN?

<img src="img/p1-vlan.png" alt="Ejemplo de VLAN por departamentos" width="40%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

Una **VLAN** (Virtual Local Area Network) es una tecnología que nos permite dividir un único switch físico en varias redes lógicas independientes. En lugar de tener que comprar un equipo para cada sector de una empresa, usamos el software del switch para segmentar y organizar el tráfico de datos de manera inteligente.

Como podemos observar en la imagen, el mismo switch físico está repartiendo la conexión para distintos departamentos. Gracias a esta configuración, la **VLAN 10 (Finanzas)** se mantiene totalmente aislada de la **VLAN 30 (Ventas)**. Esto significa que, aunque todos los cables lleguen al mismo aparato, los datos de un grupo no se "ven" ni se mezclan con los del otro.

Según la bibliografía de **Cisco**, esta separación optimiza el rendimiento y la seguridad de la red por tres motivos principales:

* **Seguridad:** Un usuario en la red de Ventas no puede acceder a los servidores de Finanzas si no hay un permiso de ruteo explícito.
* **Orden y Rendimiento:** Si un sector está saturando la red con archivos pesados, ese tráfico no afecta la velocidad de los demás sectores.
* **Flexibilidad:** Si un empleado se muda de oficina, simplemente se cambia la configuración de su boca de red en el switch sin necesidad de tirar cables nuevos.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 2. ¿Qué es una VPN?

Una **VPN** (Virtual Private Network o Red Privada Virtual) es una tecnología que permite extender una red privada sobre una red pública como Internet. Su función principal es crear un canal de comunicación seguro, permitiendo que los datos viajen protegidos como si estuviéramos conectados físicamente a la red de nuestra propia oficina, sin importar la distancia geográfica.

Para entenderlo de forma sencilla, si Internet es una autopista pública, una VPN funciona como un **túnel privado y blindado** construido dentro de esa autopista. Solo los dispositivos autorizados pueden entrar en ese túnel, y todo lo que pasa por dentro viaja cifrado (oculto) para que nadie desde afuera pueda interceptar o leer la información privada de la empresa.
<br></br>

<p align="center">
  <img src="img/VPN.png" alt="Esquema de túnel VPN" width="100%">
  <br>
  <i>Diagrama de una conexión remota segura a través de un túnel VPN.</i>
</p>
<br></br>

Según la bibliografía de **Cisco**, una VPN garantiza la operatividad y seguridad mediante dos pilares fundamentales:

* **Cifrado de Datos:** La información se codifica mediante algoritmos matemáticos antes de salir del dispositivo, volviéndose ilegible para cualquier atacante en la red pública.
* **Acceso Remoto Transparente:** Permite que un empleado trabaje desde su casa o cualquier sitio remoto accediendo a los recursos internos (servidores de archivos, bases de datos o sistemas de gestión) de manera privada y confiable.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 3. ¿Qué es una SAN?

<img src="img/SAN.png" alt="Arquitectura de red SAN" width="40%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

Una **SAN** (Storage Area Network o Red de Área de Almacenamiento) es una red de alta velocidad diseñada exclusivamente para conectar servidores con dispositivos de almacenamiento, como sistemas de discos o librerías de cintas. A diferencia de conectar un disco rígido directamente a una computadora, la SAN crea un entorno donde el almacenamiento es un recurso compartido y centralizado que funciona de forma independiente a la red de los usuarios.

Como se observa en el diagrama, la SAN actúa como una "nube de discos" privada. Según la bibliografía de **Cisco**, esto permite que los servidores vean estos discos remotos como si estuvieran físicamente instalados dentro de ellos (almacenamiento a nivel de bloque). Es la solución preferida en entornos profesionales porque el tráfico pesado de datos viaja por cables propios, sin saturar la red local (LAN) de la empresa.
<br></br>

**Las principales ventajas de implementar una SAN en una infraestructura son:**

* **Alta Disponibilidad:** Si un servidor falla, los datos permanecen intactos en la SAN y pueden ser conectados a otro servidor en segundos.
* **Consolidación y Eficiencia:** En lugar de tener gigas desperdiciados en distintos servidores, todo el espacio se administra desde un solo equipo (Storage), repartiéndolo según la necesidad.
* **Escalabilidad:** Permite agregar discos masivamente sin tener que apagar los servidores ni desarmar los equipos existentes.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 4. Diferencias entre un Hub, Repetidor, Router y Switch

Para comprender cómo se estructura una red, es fundamental distinguir la inteligencia y la función de cada dispositivo. Como se observa en el gráfico, existen diversos componentes que trabajan en conjunto para permitir la comunicación:

* **Repetidor:** Es el dispositivo más sencillo. Su única función es recibir una señal débil y regenerarla para extender su alcance físico, sin analizar el contenido de los datos.
* **Hub (Concentrador):** Funciona como un punto de conexión central, pero carece de inteligencia. Todo lo que recibe por un puerto lo reenvía a todos los demás, lo que suele generar "colisiones" y saturar la red innecesariamente.
* **Switch (Conmutador):** Es la evolución del Hub. Según la guía de **Cisco**, el switch identifica las direcciones físicas (MAC) de cada equipo conectado. De esta forma, entrega los datos solo al destinatario correcto, permitiendo que varios equipos hablen a la vez sin interferencias.
* **Router (Enrutador):** Es el "cerebro" que conecta diferentes redes entre sí (como nuestra LAN con Internet). Decide cuál es el mejor camino para que la información llegue a su destino.

<p align="center">
  <img src="img/dispositivos.png" alt="Dispositivos de red" width="100%">
  <br>
  <i>Dispositivos de Red.</i>
</p>
<br></br>

Además, en el esquema podemos ver otros componentes vitales como el **Firewall**, que actúa como una barrera de seguridad contra amenazas externas, el **Access Point** para brindar conectividad inalámbrica, y el **Módem**, que es el encargado de traducir las señales de nuestro proveedor de internet (ISP) para que el Router pueda distribuirlas.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 5. ¿Qué es un protocolo de comunicaciones?

<img src="img/p5-protocolo.png" alt="Concepto de protocolo de comunicaciones" width="45%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

En el mundo de las redes, un **protocolo de comunicaciones** es un conjunto de reglas y normas que permiten que dos o más dispositivos se entiendan y compartan información. Si comparamos una red con una charla entre personas, el protocolo sería el idioma y las reglas de cortesía: no importa qué tan buenos sean los teléfonos (el hardware), si no se utiliza el mismo idioma y no se respetan los turnos para hablar, la comunicación fracasará.

Como se ilustra en el esquema, el protocolo actúa como el medio que garantiza que el mensaje llegue correctamente del emisor al receptor. Según explica **Tanenbaum**, este acuerdo define tres aspectos fundamentales:

* **Sintaxis:** Cómo se estructuran los datos (el formato del paquete).
* **Semántica:** Qué significa cada sección de la información enviada.
* **Temporización:** A qué velocidad se deben enviar los datos y cómo se sincronizan ambos equipos.

En resumen, los protocolos son el "reglamento" que garantiza que el flujo de datos sea ordenado, seguro y universal, permitiendo que equipos de diferentes marcas en todo el mundo se conecten entre sí sin problemas.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 6. Explique TCP/IP y NetBios, resuma sus diferencias

<img src="img/Suite_de_Protocolos.jpg" alt="Suite de protocolos TCP/IP" width="45%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

Para entender las redes modernas y las antiguas, debemos diferenciar entre el estándar global **TCP/IP** y el sistema de nombres **NetBIOS**:

* **TCP/IP (Transmission Control Protocol/Internet Protocol):** Es el lenguaje universal de Internet. Como se observa en la imagen de la **Suite de Protocolos**, no es un solo protocolo sino una arquitectura de capas. Según **Cisco**, su gran ventaja es que es "enrutable": permite que los datos viajen a través de múltiples routers hasta llegar a cualquier parte del mundo usando direcciones numéricas (IP). Es robusto, escala a redes gigantescas y garantiza que la información llegue sin errores.

* **NetBIOS (Network Basic Input/Output System):** Es un protocolo mucho más antiguo, desarrollado originalmente para redes locales (LAN) pequeñas. A diferencia de TCP/IP, NetBIOS no usa números, sino **nombres de hasta 15 caracteres** para identificar a las computadoras (ejemplo: `PC-CONTABILIDAD`). Su limitación principal es que no es enrutable; es decir, los mensajes de NetBIOS no pueden salir de la oficina hacia Internet por sí solos.

**Diferencia fundamental:**
Mientras que TCP/IP es el motor que mueve los datos por todo el planeta, NetBIOS es un sistema de nombres simplificado. Hoy en día, NetBIOS casi no se usa solo, sino que corre "encapsulado" dentro de TCP/IP (NetBIOS sobre TCP/IP) para que podamos seguir viendo los nombres de los equipos en Windows pero usando la potencia y el alcance de Internet.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 7. ¿Cómo está formado un paquete de datos en TCP/IP? ¿Qué es un Flag?

En el modelo TCP/IP, la información no viaja como un bloque único, sino fragmentada en unidades llamadas **paquetes** (o segmentos en la capa de transporte). Un paquete está formado principalmente por dos secciones: el **Encabezado (Header)**, que contiene las instrucciones de manejo, y los **Datos (Payload)**, que es la información real que queremos transmitir.

<p align="center">
  <img src="img/p7-encabezado-tcp.png" alt="Estructura del encabezado TCP en español" width="100%">
  <br>
  <i>Estructura técnica de un encabezado TCP agrupados por colores.</i>
</p>

Como se puede observar en la tabla técnica superior, el encabezado contiene datos críticos para que la comunicación sea exitosa, representados por colores:
* **Azul:** Contiene los **Puertos**, que identifican la aplicación que envía y la que recibe.
* **Verde:** Incluye los **Números de Secuencia**, fundamentales para reordenar los datos al llegar.
* **Amarillo:** Es la sección de Control y Gestión, donde **residen los Flags** y el Tamaño de Ventana para coordinar el flujo de la comunicación.
* **Naranja:** Tiene la **Suma de Verificación (Checksum)**, que asegura que el paquete no se dañó.

#### ¿Qué es un Flag?
Dentro del encabezado, específicamente en la sección **amarilla** (donde se ven las siglas CWR, ECE, URG, ACK, PSH, RST, SYN, FIN), encontramos los **Flags** (banderas). Según la bibliografía de **Cisco**, los Flags son indicadores de un solo bit que funcionan como "señales de control" entre los dispositivos.

Funcionan como un lenguaje de señas para gestionar la conexión. Los más importantes son:
* **SYN (Synchronize):** "Hola, ¿querés iniciar una conexión?".
* **ACK (Acknowledgment):** "Recibido, confirmo que me llegó el paquete".
* **FIN (Finish):** "Ya no tengo más nada para enviar, cerremos la conexión".

En resumen, si el paquete es un sobre, el encabezado es la etiqueta con la dirección y los **Flags** son marcas especiales que indican si el envío es urgente o si requiere un acuse de recibo obligatorio.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

## 8. Defina la red según su geografía. Explicar distintas variantes.

<img src="img/clasificacion_de_redes.png" alt="Clasificación geográfica de redes" width="45%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

La clasificación geográfica de las redes determina el alcance físico y las tecnologías necesarias para establecer la comunicación. Según la bibliografía de **Tanenbaum**, las redes se categorizan principalmente por la distancia que cubren:

* **PAN (Personal Area Network):** Como se observa en la base del gráfico, son redes de muy corto alcance (menos de 10 metros). El ejemplo más común es el **Bluetooth** (estándar IEEE 802.15) que conecta dispositivos personales.
* **LAN (Local Area Network):** Cubre áreas pequeñas como una casa o una oficina. Suelen usar tecnologías **Wi-Fi** (IEEE 802.11) o cables Ethernet, con un alcance típico de hasta 150 metros.
* **MAN (Metropolitan Area Network):** Diseñada para conectar diversas LAN en una ciudad o municipio, con un alcance de hasta 50 km. Utiliza tecnologías como WiMAX fijo para cubrir grandes áreas urbanas.
* **WAN (Wide Area Network):** Es la red de área amplia que conecta países o continentes. Internet es el ejemplo máximo. Utiliza infraestructuras complejas, satélites y cables submarinos para cubrir distancias superiores a los 150 km.

**Dato clave:** A medida que la red crece en geografía, la administración se vuelve más compleja y suele requerir de proveedores externos (ISP) para mantener la infraestructura de conexión.


<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 9. Defina una red según su topología. Explicar distintas variantes.

<img src="img/p9-topologia.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 10. Explicar el servicio de DHCP

<img src="img/p10-dhcp.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 11. Explicar el servicio de DNS

<img src="img/p11-dns.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 12. Tecnologías Wireless y sus estándares

<img src="img/p12-wireless.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 13. ¿Qué es un Proxy?

<img src="img/p13-proxy.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 14. Protocolo Spanning Tree

<img src="img/p14-spanning-tree.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 15. Protocolo de comunicaciones OSPF

<img src="img/p15-ospf.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 16. Protocolo ARP

<img src="img/p16-arp.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 17. ¿Qué es un Firewall?

<img src="img/p17-firewall.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 18. ¿Qué es una DMZ?

<img src="img/p18-dmz.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 19. ¿Qué es un Gateway?

<img src="img/p19-gateway.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 20. Según Microsoft, ¿qué significa NBL?

<img src="img/p20-nbl.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 21. Tipos de enlace: MPLS, LAN to LAN, Microonda, VSAT

<img src="img/p21-enlaces.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 22. Describir la tecnología LTE

<img src="img/p22-lte.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 23. Explique la solución de Microsoft Teams

<img src="img/p23-teams.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 24. ¿Qué significa aplicar calidad en un enlace MPLS?

<img src="img/p24-qos-mpls.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 25. Diferencias entre Coaxial, UTP y Fibra

<img src="img/p25-cables.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 26. Según Cisco, ¿qué significa CCENT, CCNA y CCNP?

<img src="img/p26-cisco-cert.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 27. Explique el modelo OSI

<img src="img/p27-modelo-osi.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 28. Estándar IEEE 802.3

<img src="img/p28-ieee8023.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 29. Estándar IEEE 802.4

<img src="img/p29-ieee8024.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 30. Protocolos para enviar y recibir correo

<img src="img/p30-email-protocolos.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 31. Protocolo para leer correo recibido

<img src="img/p31-imap-pop3.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 32. Diferencias entre IPv4 e IPv6

<img src="img/p32-ipv4-ipv6.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 33. Experiencia en redes por integrante

**Punto clave:** Cada integrante describe su experiencia personal y/o profesional en redes informáticas.

**Diego Murgana:** *Completar aquí...*

**Leandro Sosa:** *Completar aquí...*

**Agustín Senin:** *Completar aquí...*

**Santiago Padilla:** *Completar aquí...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

*Trabajo Práctico — Programación sobre Redes | IFTS 18 | Grupo D*
