Se identificó una campaña activa de phishing denominada VENOMOUS#HELPER, observada desde abril de 2025, que utiliza herramientas legítimas de administración remota como SimpleHelp y ConnectWise ScreenConnect para establecer acceso persistente en equipos comprometidos.

La actividad ha impactado a más de 80 organizaciones, principalmente en Estados Unidos, y presenta características consistentes con operaciones de Initial Access Brokers (IAB) o fases iniciales de despliegue de ransomware.

El ataque inicia con un correo que suplanta a la Social Security Administration (SSA) e induce a la víctima a descargar un supuesto documento oficial. El archivo descargado instala una versión modificada de SimpleHelp, configurada para persistencia avanzada, evasión de detección y monitoreo de controles de seguridad.

Posteriormente, los actores elevan privilegios a nivel SYSTEM, obteniendo capacidad para:

- Control remoto completo del sistema
- Visualización e interacción con la sesión del usuario
- Transferencia bidireccional de archivos
- Ejecución silenciosa de comandos
- Movimiento lateral dentro de la red

Como mecanismo de redundancia, también despliegan ScreenConnect, permitiendo mantener acceso incluso si uno de los canales remotos es detectado o bloqueado.

El uso de software firmado y legítimo dificulta significativamente la detección mediante controles tradicionales basados en firmas.

Referencia: https://thehackernews.com/2026/05/phishing-campaign-hits-80-orgs-using.html
