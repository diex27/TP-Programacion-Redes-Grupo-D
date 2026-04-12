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


### 1. ¿Qué es una VLAN?

<img src="img/p1-vlan.png" alt="Ejemplo de VLAN por departamentos" width="40%" align="right" style="margin-left: 20px; margin-bottom: 20px;">

Una **VLAN** (Virtual Local Area Network) es una tecnología que nos permite dividir un único switch físico en varias redes lógicas independientes. En lugar de tener que comprar un equipo para cada sector de una empresa, usamos el software del switch para segmentar y organizar el tráfico de datos de manera inteligente.

Como podemos observar en la imagen, el mismo switch físico está repartiendo la conexión para distintos departamentos. Gracias a esta configuración, la **VLAN 10 (Finanzas)** se mantiene totalmente aislada de la **VLAN 30 (Ventas)**. Esto significa que, aunque todos los cables lleguen al mismo aparato, los datos de un grupo no se "ven" ni se mezclan con los del otro.

Según la bibliografía de **Cisco**, esta separación optimiza el rendimiento y la seguridad de la red por tres motivos principales:

* **Seguridad:** Un usuario en la red de Ventas no puede acceder a los servidores de Finanzas si no hay un permiso de ruteo explícito.
* **Orden y Rendimiento:** Si un sector está saturando la red con archivos pesados, ese tráfico no afecta la velocidad de los demás sectores.
* **Flexibilidad:** Si un empleado se muda de oficina, simplemente se cambia la configuración de su boca de red en el switch sin necesidad de tirar cables nuevos.



<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 2. ¿Qué es una VPN?

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

### 3. ¿Qué es una SAN?

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

### 4. Diferencias entre un Hub, Repetidor, Router y Switch

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

### 5. ¿Qué es un protocolo de comunicaciones?

<img src="img/p5-protocolo.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 6. Explique TCP/IP y NetBios, resuma sus diferencias

<img src="img/p6-tcpip-netbios.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 7. ¿Cómo está formado un paquete de datos en TCP/IP? ¿Qué es un Flag?

<img src="img/p7-paquete-tcp.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

<p align="right"><a href="#-índice-de-contenidos">⬆ Volver al Índice</a></p>

---

### 8. Defina la red según su geografía. Explicar distintas variantes.

<img src="img/p8-geografia-redes.png" width="35%" align="right" style="margin-left: 15px;">

**Punto clave:** *Contenido en desarrollo...*

**Explicación técnica:** *Contenido en desarrollo...*

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
