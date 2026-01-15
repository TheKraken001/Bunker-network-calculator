📘 Manual de Operaciones: The Kraken Networking

1. Introducción

Bienvenido al sistema The Kraken. Este manual te guiará a través del proceso de diseño, cálculo y aseguramiento de una infraestructura de red utilizando la suite.

El objetivo de esta herramienta es eliminar el error humano en cálculos de subredes y automatizar la aplicación de mejores prácticas de seguridad (Hardening) en equipos Cisco.

2. Interfaz de Mando

La interfaz se divide en 3 columnas estratégicas:

Izquierda (Input): Configuración de parámetros, hardware y VLANs.

Centro (Visual): Topología, Matriz VLSM y Simulador.

Derecha (Output): Código generado y referencias.

3. Flujo de Trabajo Paso a Paso

Paso 1: Definición de Hardware y Perfil

En la columna izquierda:

Router Modelo: Selecciona el equipo físico que tienes.

Cisco ISR 4000: Usa interfaces de 3 dígitos (Gi0/0/0).

Cisco 1841: Usa interfaces FastEthernet (Fa0/0).

Nota: Esto asegura que al copiar el código, no te dé error de "Interface not found".

Perfil de Misión:

Usa BUNKER si la seguridad es crítica (Bancos, Gobierno). Bloqueará pings entre VLANs.

Usa EMPRESA para oficinas estándar.

Ingeniería Física: Selecciona la distancia de tus enlaces para recibir recomendaciones de cableado (Fibra vs Cobre).

Paso 2: Segmentación (VLSM)

Red Base: Ingresa la dirección IP principal (ej: 192.168.0.0/24 o 10.0.0.0/8).

Añadir VLANs:

Haz clic en + VLAN.

Asigna un Nombre (ej: Ventas), Hosts (cantidad de equipos) e ID (número de VLAN).

Ejecutar: Presiona el botón rojo EJECUTAR.

El sistema ordenará automáticamente las VLANs de mayor a menor para optimizar el espacio.

Paso 3: Validación Visual (Centro)

Una vez ejecutado:

Topología: Verifica que el diagrama SVG muestre tu router, switch y las VLANs conectadas.

Matriz VLSM: Revisa la tabla. Observa la columna "Binario" para entender cómo se han asignado los bits de red (Cian) y host (Gris).

Inspector OSI: Pasa el mouse sobre las capas para recordar vulnerabilidades comunes.

Paso 4: Simulación de Tráfico (Test de Fuego)

Antes de copiar el código, prueba la lógica:

Ve al panel 9. SIMULADOR DE TRÁFICO.

Selecciona una VLAN de Origen y una de Destino.

Elige ICMP (Ping).

Dale a ▶ TEST.

Si estás en modo BUNKER y tratas de conectar dos VLANs diferentes, deberías ver un fallo (❌) debido a las ACLs Zero-Trust.

Si estás en modo EMPRESA, debería ser exitoso (✅).

Paso 5: Despliegue (Derecha)

Ve a la columna derecha 7. CÓDIGO GENERADO.

Usa las pestañas RT (Router) y SW (Switch) para ver los scripts.

Presiona COPY para llevarlo al portapapeles.

Pega la configuración en tu emulador (Packet Tracer/GNS3) o equipo real.

4. Generación de Reportes

Para entregar documentación a un cliente o superior:

Haz clic en el botón verde 🖨️ IMPRIMIR REPORTE en la cabecera.

Se abrirá una ventana limpia, con fondo blanco y diseño profesional.

Guárdalo como PDF.

5. Solución de Problemas (Troubleshooting)

Problema: "Me dice Error Crítico de Capacidad".

Causa: Estás pidiendo más IPs de las que caben en tu red base (ej: 300 hosts en una red /24).

Solución: Aumenta la red base (ej: cambia /24 a /23 o /16).

Problema: "El código del router da error en la interfaz".

Causa: Probablemente seleccionaste el modelo incorrecto en el paso 1.

Solución: Verifica qué modelo estás usando y selecciónalo en el menú desplegable.

Problema: "No tengo internet en las VLANs".

Causa: El script configura NAT, pero necesitas que la interfaz WAN (Gi0/0) reciba IP por DHCP de tu ISP.

Solución: Verifica que el cable WAN esté conectado a internet.

🛠️ Tecnologías Utilizadas
HTML5 - Estructura y semántica

CSS3 - Estilos y diseño responsivo

JavaScript ES6+ - Lógica y cálculos

SVG - Diagramas de topología

OWASP Best Practices - Seguridad web

🌐 Compatibilidad
✅ Chrome 80+

✅ Firefox 75+

✅ Edge 80+

✅ Safari 13+

✅ Opera 67+

🙏 Agradecimientos
Cisco Systems - Por los estándares de networking

OWASP - Por las mejores prácticas de seguridad

NIST - Por el framework Zero-Trust

Comunidad de networking - Por el feedback continuo

Fin del Manual.
The Kraken Suite - Arquitectura de Redes Avanzada.