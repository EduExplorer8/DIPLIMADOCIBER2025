**DEFENSA EN PROFUNDIDAD**

El modelo de **Defensa en Profundidad** es una estrategia de seguridad que se basa en la implementación de **múltiples capas de protección** para salvaguardar los activos de una organización, especialmente los datos y sistemas informáticos. Su origen se remonta a la terminología militar, donde se utilizan varias líneas defensivas consecutivas para desgastar y ralentizar al enemigo, en lugar de depender de una única y fuerte barrera.

En el ámbito de la ciberseguridad, la idea es que **ninguna capa de seguridad es infalible**. Si un atacante logra superar una defensa (por ejemplo, un firewall), se encontrará con otra capa de seguridad que intentará detenerlo (como un sistema de detección de intrusos, cifrado de datos o controles de acceso).

Este modelo se enfoca en tres aspectos clave:

* **Defensas Físicas:** Incluyen medidas para proteger los equipos y las instalaciones, como guardias de seguridad, cámaras de vigilancia, cerraduras, sistemas biométricos, etc.
* **Defensas Técnicas:** Se refieren a las soluciones tecnológicas implementadas, como firewalls, software antivirus y antimalware, sistemas de prevención de intrusiones (IPS), cifrado de datos, autenticación multifactor, segmentación de red, etc.
* **Defensas Administrativas/Organizativas:** Abarcan las políticas, procedimientos y la capacitación del personal, como la gestión de acceso, planes de respuesta a incidentes, concientización sobre seguridad, auditorías de seguridad, etc.

En resumen, la defensa en profundidad busca crear un **escudo multicapa y redundante** que dificulte el avance de un atacante, le dé tiempo a la organización para detectar y responder a la amenaza, y minimice el impacto en caso de una brecha en alguna de las capas.

---
**Trabajo en Grupo**

Desarrollar y documentar en github el siguiente reto.  

**Nota**
Por cada grupo de trabajo crear una carpeta con un README con la resolución.

---

## Defensa en Profundiadad: Fortaleza Digital de "TechSolutions Corp."


**Contexto:**
TechSolutions Corp. es una empresa global líder en el desarrollo de software y servicios en la nube, con una base de clientes masiva y una vasta cantidad de datos sensibles, incluyendo información financiera, propiedad intelectual y datos personales de clientes. Su infraestructura de TI es compleja, abarcando centros de datos locales, entornos de nube híbrida (AWS y Azure), una red de oficinas distribuidas globalmente y una fuerza laboral remota significativa.

**El Incidente**
Es el 10 de junio de 2025. Su equipo como expertos en ciberseguridadha detectado una serie de actividades anómalas:

* **Fase 1 (Vectores de Ataque Iniciales):**
    * Múltiples empleados han recibido correos electrónicos de *phishing* altamente sofisticados, suplantando a la dirección de TI, solicitando credenciales de acceso a un "nuevo portal de empleados".
    * Se ha identificado un intento de explotación de una vulnerabilidad de día cero en un servidor web público que ejecuta un software de gestión de proyectos obsoleto (versión no parcheada) dentro de la DMZ.
    * Un empleado de reciente contratación descargó accidentalmente un archivo adjunto malicioso desde una red social profesional (LinkedIn) que se hizo pasar por una oferta de capacitación.

* **Fase 2 (Movimiento Lateral y Persistencia):**
    * Parece que el atacante ha logrado comprometer una estación de trabajo de ingeniería de software a través del *phishing* exitoso, utilizando credenciales robadas.
    * Desde esta estación de trabajo, se han observado intentos de escaneo de red interno y de elevación de privilegios.
    * Hay indicios de que el atacante está intentando establecer persistencia mediante la creación de cuentas de usuario ocultas y la modificación de tareas programadas en algunos sistemas comprometidos.

* **Fase 3 (Objetivo Final - Exfiltración/Destrucción):**
    * La actividad principal del atacante parece dirigirse a la base de datos de propiedad intelectual (ubicada en la nube) y a los servidores de desarrollo que contienen el código fuente de los productos estrella de la empresa.
    * Se han detectado grandes volúmenes de tráfico saliente inusual hacia direcciones IP externas no identificadas.
    * En algunos sistemas críticos, se han encontrado archivos con extensiones cifradas y notas de rescate, lo que evidencia una actividad de *ransomware* como un segundo vector de ataque o distracción.

**La Tarea:**
Como equipo de seguridad de TechSolutions Corp., su tarea es desarrollar una estrategia de **defensa en profundidad** integral para mitigar el impacto de este incidente y proteger a la empresa contra futuros ataques. No se trata solo de reaccionar al incidente actual, sino de establecer una arquitectura de seguridad resiliente.

**Instrucciones para los Estudiantes:**

1.  **Análisis de Amenazas y Vulnerabilidades:** Identifiquen las principales amenazas y vulnerabilidades expuestas en la narrativa.
AMENAZAS:
   • Phishing avanzado dirigido a empleados (suplantación de TI).
	• Un empleado de reciente contratación descargó accidentalmente un archivo adjunto malicioso desde una red social profesional (LinkedIn) que se hizo pasar por una oferta de capacitación.
	• Explotación de vulnerabilidades de día cero en servidores expuestos (SOFTWARE DESACTUALIZADO).
	• Descarga de malware por ingeniería social (archivo malicioso desde LinkedIn).
	• Parece que el atacante ha logrado comprometer una estación de trabajo de ingeniería de software a través del phishing exitoso, utilizando credenciales robadas.
		○ tras compromiso de credenciales (escalada de privilegios y escaneo interno).
	• Persistencia mediante cuentas ocultas y tareas programadas.
	• Exfiltración de información sensible (base de datos en la nube, código fuente).
   • Ransomware (cifrado de archivos y notas de rescate)
VULNERABILIDADES:
	• Falta de parches y actualización en servidores críticos.
	• Ausencia de segmentación de red y controles de acceso internos.
	• Deficiente concienciación y capacitación del personal, socialización e interiorización de la cultura de seguridad.
	• Deficiente proceso de induccion y reinduccion para la socializacion de las politicas y procedimientos de seguridad.
	• Insuficientes controles de monitoreo y detección de anomalías.
   • Políticas débiles de gestión de identidades y privilegios.

2.  **Principios de Defensa en Profundidad:** Expliquen cómo aplicarían los principios de defensa en profundidad (capas de seguridad) en este escenario.
  Se plantea que la defensa profunda sea un tema de cultura organizacional, y que vaya evolucionando y desarrollandose, al interior de la organizaicon, que sea resiliente y en constante desarrollo, partiendo desde los directivos y a la vez en los operarios o partes mas bajas de la organizacion, y que de esta manera ir permeando a todos los miembros de la organizacion. Posteriormente, a hacer llegar a la necesidad a la organizacion, se relizaran la implementacion de las capas como se propone a continuacion

   
3.  **Capas de Defensa Propuestas:** Diseñen una estrategia detallada de defensa en profundidad, especificando las medidas de seguridad y tecnologías clave en cada una de las siguientes capas:
    * **Capa 1: Perímetro/Red Externa** :
   • Firewalls de nueva generación (NGFW) configurados con reglas estrictas y listas negras de IPs maliciosas.
	• Sistemas de prevención y detección de intrusos para identificar ataques conocidos y comportamientos anómalos.
	• WAF (Web Application Firewall) para proteger aplicaciones web públicas.
	• Segmentación y actualización obligatoria de software expuesto.
   • Filtrado de correo electrónico para bloquear phishing y adjuntos maliciosos.

    * **Capa 2: Red Interna/Segmentación**
   • Segmentación de la red para aislar servidores críticos, bases de datos y estaciones de trabajo sensibles.
	• Control de accesos para validar dispositivos antes de permitir acceso.
   • Monitoreo de tráfico interno y alertas ante escaneos o movimientos laterales.

    * **Capa 3: Endpoint/Dispositivos**
   • Soluciones para detectar y responder a comportamientos anómalos en las terminales.
	• Antivirus y antimalware actualizados.
	• Aplicación automática de parches y actualizaciones.
   • Restricción de privilegios en estaciones de trabajo (principio de mínimo privilegio)

    * **Capa 4: Aplicaciones**
   • Desarrollo seguro y revisión de código.
	• Pruebas periódicas de vulnerabilidades.
	• Control de versiones y acceso restringido al código fuente.
   • Seguridad autenticación robusta en aplicaciones internas y externas.

    * **Capa 5: Datos**
   • Cifrado de datos en reposo y en tránsito.
	• Particionar y encriptar los datos, para evitar fuga de información.
	• Backups automáticos, cifrados y con almacenamiento offline.
   • Control de acceso basado en roles y monitoreo de accesos a bases de datos sensibles de acuerdo a cada departamento.

    * **Capa 6: Identidad y Acceso**
   • Autenticación multifactor obligatoria para todos los accesos críticos y remotos.
	• Gestión centralizada de identidades y revisiones periódicas de privilegios.
	• Políticas de contraseñas robustas y rotación frecuente.
   • Monitoreo de cuentas privilegiadas y detección de creación de cuentas sospechosas.

    * **Capa 7: Operaciones y Concienciación**
    • Programas de capacitación y simulacros de phishing regulares para empleados.
	• Políticas y procedimientos claros de respuesta a incidentes.
	• Auditorías de seguridad periódicas y revisión.
   • Cultura de reporte de incidentes y recompensas por identificación de amenazas internas.


    
4.  **Respuesta al Incidente:** Describan los pasos iniciales que tomarían para contener y erradicar el incidente actual basándose en su estrategia de defensa en profundidad.

Pasos iniciales:
	• Identificación: De la amenaza, recoleccion de la informacion y revision del ataque, que alcance tuvo el ataque.
	• Contención: Aislar estaciones y servidores comprometidos, bloquear comunicación con IPs externas sospechosas.
	• Erradicación: Eliminar malware, cuentas ocultas y tareas programadas maliciosas.
	• Recuperación: Restaurar sistemas desde backups limpios y actualizados.
	• Comunicación: Informar a la dirección y, si aplica, a clientes y autoridades según normativas.
	• Análisis forense: Determinar el alcance y vector de ataque para evitar recurrencia.


   
8.  **Monitoreo y Mejora Continua:** ¿Cómo garantizarían que su estrategia de defensa en profundidad se mantenga efectiva a lo largo del tiempo?

	• Implementar un sistema para correlación y análisis de eventos de seguridad en tiempo real.
	• Realizar auditorías de seguridad al menos dos veces al semestre.
	• Actualizar políticas y controles según nuevas amenazas e incidentes detectados.
	• Medir KPIs de ciberseguridad (tiempo de detección, respuesta, número de incidentes reportados, etc.).
   • Mantener un ciclo de retroalimentación para mejorar la estrategia de defensa en profundidad y la cultura de seguridad empresarial![image](https://github.com/user-

