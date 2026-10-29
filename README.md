## Problemática: En el entorno académico actual, se presenta una dificultad recurrente al intentar reportar fallos en los activos debido a que el personal encargado de su supervisión pertenece a la empresa colaboradora y no se encuentra fácilmente localizable para el alumnado. Ante esta falta de un canal directo provoca retrasos en la atención de los reportes y agrava el deterioro de los equipos. Para resolver esta problemática, se busca implementar un sistema integrado en Microsoft Teams que permita a los alumnos reportar fallas de manera directa e intuitiva, vinculando automáticamente los datos y antecedentes del activo afectado con el equipo encargado en la empresa.

## Objetivo general: Desarrollar e integrar un sistema de gestión de incidencias en Microsoft Teams vinculado a la base de datos de activos de la universidad, para optimizar el canal de reporte entre los alumnos y el personal de la empresa encargada, reduciendo los tiempos de respuesta y evitando el deterioro mayor de los equipos.

## Alcance: (Que funciones tendrá,que tecnologías se usarán)

* **Registro e inicio de sesión con dos roles:**  alumno y personal de la empresa encargada.
* **Registro de reportes deactivos en la base de datos:** (identificador, nombre, tipo y ubicación), capturados por los activos.
* **Creación de reportes:**  el alumno selecciona el material afectado y describe la falla.
* **Sumarse a un reporte existente:**  si ya hay un reporte del mismo material y tipo de falla, el alumno puede unirse en lugar de crear uno nuevo, lo que evita duplicados de reportes.
* **Prioridad automática:**  la prioridad del reporte aumenta según el número de reportes que se suman (por ejemplo: baja, media y alta).

* **Seguimiento del estado de un reporte:**  cada reporte pasará por los estados Pendiente, Revisado, En solución y Resuelto, para que el alumno sepa en qué punto está su reporte.

* **Panel para el personal de la escuela:**  lista de reportes ordenada por prioridad, con la opción de cambiar el estado de cada uno.
* **Historial de reportes:**  sección “Mis reportes” para el alumno e historial de reportes por activo.

## Responsabilidades: los integrantes se organizaron dividiendo los roles de trabajo 
de la siguiente manera para garantizar una cobertura eficiente de todas las etapas 
del desarrollo 
*  **Backend:** Jadiel Ernesto es el encargado del desarrollo del servidor y el 
hosteo, implementara edpoints para el registro de usuarios, creación y 
actualización de reportes de activos y es el encargado de la seguridad, 
autenticación de usuarios y control de accesos según los roles definidos y 
gestionar la comunicación con APIs externas 
* **Frontend:** Yuseff Farah es el encargado de diseñar la interfaz del usuario el 
cual debe de hacer un diseño responsivo y amigable para el usuario y dar 
una conexión de las interfaces con el Backend para mostrar la información 
en tiempo real 
* **Base de datos** y Hosteo amairani es la encargada de la creación, diseño y 
estructuración de la base de datos, además de gestionar el despliegue e 
infraestructura en la nube. ella se encarga de definir los esquemas de 
datos, asegurar la integridad de la información de los usuarios y activos y 
mantener el servidor de base de datos en línea. Para gestionar la base de 
datos se usará MySQL o MongoDB, o Supabase.