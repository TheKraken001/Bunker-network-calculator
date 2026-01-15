🦑 The Kraken Networking Suite (NEXUS V24)

The Kraken es una suite de arquitectura de redes Zero-Trust diseñada para ingenieros de ciberseguridad, administradores de red y estudiantes avanzados. No es solo una calculadora VLSM; es un generador de defensa activa.

Genera configuraciones endurecidas (hardened) para equipos Cisco IOS basándose en estándares militares (NIST/CIS), simula tráfico en tiempo real y valida la integridad matemática de la red.

🚀 Características Principales

🧠 Cerebro Matemático (Core VLSM)

Cálculo Real: Algoritmos de ordenamiento automático para evitar el desperdicio de IPs.

Visualización Binaria: Inspección de máscaras a nivel de bit (Matrix Style).

Sanitización de Datos: Validación estricta de entradas para prevenir errores de Capa 8.

🛡️ Perfiles de Misión

Elige tu nivel de paranoia:

🛡️ BUNKER (Zero Trust): Aislamiento total entre VLANs. Bloqueo de tráfico lateral. Port-Security en modo shutdown.

🏢 EMPRESA (Standard): Balance entre seguridad y usabilidad.

🎮 GAMING (QoS): Priorización de tráfico UDP y baja latencia.

⚙️ Adaptabilidad de Hardware

Selector de Router: Genera comandos específicos para interfaces Gi0/0/0 (ISR 4000), Gi0/0 (ISR 2900) o Fa0/0 (Legacy 1841).

Ingeniería de Capa 1: Recomendador inteligente de cableado (Fibra OS2/OM4 vs Cobre Cat6A) según distancia.

🎮 Laboratorio Visual

Topología Viva (SVG): Diagramas que se dibujan en tiempo real.

Simulador de Tráfico: Visualiza paquetes viajando por la red. Comprueba si tus ACLs funcionan antes de desplegar.

Inspector OSI: Referencia interactiva de vulnerabilidades por capa.

📦 Instalación y Uso

The Kraken es una Single Page Application (SPA) de arquitectura monolítica. No requiere servidores, Python, ni Node.js. Es portable y offline.

Descarga el archivo index.html (o v24.html).

Ábrelo con cualquier navegador moderno (Chrome, Edge, Firefox, Brave).

¡Listo para desplegar!

🛠️ Guía Rápida

Define tu Hardware: Selecciona el modelo de router real que usarás.

Elige tu Perfil: ¿Necesitas seguridad militar o velocidad de gaming?

Segmenta: Ingresa tu IP base y añade las VLANs necesarias.

Ejecuta: El sistema calculará subredes, dibujará el mapa y escribirá el código.

Despliega: Copia los scripts generados directamente a tu terminal (Putty/TeraTerm).

📄 Reportes Profesionales

Incluye un motor de generación de reportes en PDF que limpia la interfaz oscura y genera un documento técnico de fondo blanco ("Printer Friendly") con:

Matriz VLSM completa.

Diagrama de topología.

Justificación de seguridad.

Scripts de configuración.
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

⚠️ Disclaimer

Esta herramienta genera configuraciones de seguridad ofensiva/defensiva. El uso de ACLs restrictivas (Modo Bunker) puede cortar el acceso a servicios si no se configura correctamente. Úsalo bajo tu propia responsabilidad.

Desarrollado con obsesión por el detalle y paranoia constructiva.