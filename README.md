# 🌐 Trabajo Práctico Teórico: Programación sobre Redes

**Institución:** IFTS 18  
**Carrera:** Técnico Superior en Desarrollo de Software  
**Profesor:** Lucas Rusatti  
**Grupo:** D  

---

## 👥 Integrantes
* **Diego Murgana** - *Administrador del Proyecto*
* **Leandro Sosa**
* **Agustín Senin**
* **Santiago Padilla**

---

## 📖 Desarrollo del Cuestionario

### 1. ¿Qué es una VLAN?
**Punto clave:** Una **VLAN** (Virtual Local Area Network) es una subdivisión lógica de una red física local que permite agrupar dispositivos como si estuvieran en la misma red, sin importar su ubicación física real[cite: 4].

**Explicación técnica:**
* **Segmentación:** Divide un switch físico en varios virtuales para optimizar el tráfico.
* **Seguridad:** Aísla el tráfico entre diferentes departamentos.
* **Broadcast:** Reduce el tráfico innecesario en la red al limitar el dominio de difusión.

---

### 2. ¿Qué es una VPN?
**Punto clave:** Una **VPN** (Virtual Private Network) es una tecnología que crea un túnel cifrado y seguro sobre una red pública (como Internet) para conectar usuarios de forma privada a una red remota[cite: 5].

**Explicación técnica:**
* **Cifrado:** Protege la integridad y privacidad de los datos durante el transporte.
* **Acceso Remoto:** Permite conectarse a los recursos de la oficina desde cualquier lugar del mundo.
* **Tunelización:** Encapsula los datos para que viajen protegidos por la red pública.

---

### 3. ¿Qué es una SAN?
**Punto clave:** Una **SAN** (Storage Area Network) es una red de alta velocidad diseñada específicamente para conectar servidores a dispositivos de almacenamiento masivo (discos, librerías de cintas, etc.)[cite: 7].


**Explicación técnica:**
* **Red Dedicada:** Funciona de forma independiente a la red de área local (LAN) para no congestionarla con el tráfico de datos pesados.
* **Acceso a Nivel de Bloques:** A diferencia de un NAS, la SAN permite que el sistema operativo vea los discos remotos como si estuvieran conectados localmente.
* **Alta Disponibilidad:** Permite compartir el almacenamiento entre múltiples servidores, facilitando copias de seguridad y redundancia.

---

### 4. Diferencias entre Hub, Repetidor, Router y Switch

**Punto clave:** Estos dispositivos operan en diferentes capas del modelo OSI y tienen distintos niveles de "inteligencia" para manejar los datos en una red.

| Dispositivo | Capa OSI | Función Principal | Inteligencia |
| :--- | :--- | :--- | :--- |
| **Repetidor** | Física (1) | Regenera la señal eléctrica para extender la distancia del cableado. | Nula (solo amplifica). |
| **Hub** | Física (1) | Conecta varios equipos en forma de estrella; todo lo que recibe lo reenvía a todos los puertos (Broadcast). | Baja (genera colisiones). |
| **Switch** | Enlace (2) | Conecta equipos en una LAN y envía los datos solo al destinatario correcto usando direcciones MAC. | Media (aprende rutas). |
| **Router** | Red (3) | Interconecta diferentes redes (ej. tu casa con Internet) y decide el mejor camino usando direcciones IP. | Alta (toma decisiones). |


**Diferencias principales:**
* **Hub vs. Switch:** El Hub es un "difusor" pasivo (envía a todos), mientras que el Switch es "selectivo" (envía solo al destino), lo que lo hace mucho más rápido y seguro.
* **Switch vs. Router:** El Switch une computadoras dentro de una misma red; el Router une esa red con otras redes externas.
* **Repetidor:** Es el más simple de todos, solo sirve para que la señal no se pierda en distancias largas.
