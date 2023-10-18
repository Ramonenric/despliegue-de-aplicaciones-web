P2: Administración de servidores web
La actividad es individual, pero os podéis ayudar sin copiar.
Comente todo el código para su correcta comprensión. Si quiere destacar algo, puede responder la actividad con los puntos que considere clave o destacables.
Instrucciones de entrega:
Esta entrega se realizará mediante la plataforma Moodle y GitHub.
En el Moodle, habrá que subir un archivo .md con el siguiente nombre: DAW_ DAW_Apellido1_Apellido2_Nombre.md siguiendo el formato Markdown para explicar los diferentes ejercicios.
En GitHub se tendrá que subir en el repositorio de la asignatura. Se puede añadir imágenes y añadirlas en el documento.
 

1.	Instale en una máquina virtual un sistema operativo con base Linux (se recomienda Debian o Ubuntu) e instale apache2.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/e16f7f50-8870-49cb-9802-0fe1813d7e1f)


.
2.	Explique con sus palabras que es una petición GET, POST, PUT y DELETE, remarcando sus diferencias.
La petició GET es una petició que es fa a un servidor per tal d’obtenir información. S’utilitza per recuperar dades especifiques d’un recurs al servidor.

La petició POST es una petició que es fa per enviar les dades d’un servidor i aixi crear un nou recurs en el servidor. S’utilitza per enviar información al servidor.

La petició PUT es una petició que s’utilitza per actualitzar un recurs que ja existeix al servidor. S’utilitza per enviar dades i reemplaçar completament un recurs en el servidor.

Finalment, la peticio DELETE es una petició que s’utilitza per eliminar un recurs que ja existeix en el servidor.

La principal diferencia entre aquestes peticions es el objectiu de cadascuna i la forma en que s’utilitzen les dades.
.
3.	Cambie del puerto 80 al puerto 4444 el servidor apache2. Muestra desde el navegador su funcionamiento adjuntando una captura de pantalla.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/51f620b1-c212-4a28-b7f7-8b2208904847)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/ec38d95c-1dbe-4114-bc03-71df958ed786)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/aca54f34-a5d6-4b90-85d0-ff82ec2a3306)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/6003c336-3969-4aee-bf9d-baf912561215)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/b25c658d-082d-4046-b17a-88c74312857f)

.
4.	Instale un certificado SSL y configure su Apache para servir contenido a través de HTTPS en el puerto 4444. Muestre desde el navegador cómo se muestra el sitio web como "seguro" (aunque sea un certificado autofirmado).
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/75cf1ed1-4be5-48ed-9fc4-3783ee7cac39)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/f2d77dd4-53a2-45bf-83cb-beb1e348c635)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/b04174c6-9f5a-4e48-8f3e-c5c4240f58c1)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/7a98a6b5-e166-4171-bdb2-7b6d6bdea5ae)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/6f4801dd-8dcf-4ad1-81a3-484bdf7c72f7)

.
5.	¿Dónde se encuentran los ficheros de configuración de Apache2?
•	Ubicación principal.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/c7db7a82-c936-4d9c-a488-f7834d4033ea)

•	Explora el archivo apache2.conf. Identifica las secciones principales y describe su propósito.
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/fde15cbf-12e9-4f61-958a-d9ee0111ec32)

 
En la imatge es pot veure la jerarquía on en pot veure que les seccions principals son la configuracio global del servidor(apache2.conf), configuracio de moduls (mods-enable), ajustes de configuracio(conf-enable) i configuracio per a llocs web disponibles(sites-enabled)
•	sites-available y sites-enabled: Explica la diferencia entre estos dos directorios y cómo funcionan juntos.
Sites-available: Aquest directori té arxius de configuracio per a llocs web disponibles, pero no están actius actualmente en el servidor.

Sites-enabled: Aquest directori té enllaços als arxius de configuracio de llocs web actius que es troben a sites-available.

•	mods-available y mods-enabled: Explica la diferencia entre estos dos directorios.
Mods-available: En aquest directori es troben els arxius de configuración de moduls que están disponibles per a ser utilitzats a Apache2.
Mods-enabled: Aquest directori té enllaços  simbolics als arxius de configuracio de moduls que están actius en el servidor.
.
6.	¿Dónde se encuentran los ficheros de ejecución de Apache2?
•	Ubicación principal
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/0e93e101-989b-4ceb-810b-912998026b03)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/4bea936a-9edc-49a6-957a-906826387d65)

 
•	Control del servicio: Utiliza el binario de ejecución para iniciar, detener, recargar y reiniciar el servidor Apache2 explicando la diferencia entre cada uno de los comandos utilizados.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/bf538a65-38d0-437e-b7d1-ce93e529c96b)

•	Comprobación de sintaxis: Usa el binario de Apache para verificar la sintaxis de tu configuración. Esto es útil para asegurarse de que no haya errores antes de reiniciar el servidor.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/1412c48b-8449-4a8e-a78a-7e8df6a1eac7)

.
7.	¿Dónde se encuentran los ficheros de monitorización de Apache2?
•	Ubicación principal
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/5c7a16eb-2645-4d6c-899e-d36e6ab058e9)

 
•	error.log y access.log: Explica la diferencia entre estos dos archivos. Abre y revisa las entradas recientes en cada uno de ellos.
error.log: Aquest arxiu registra els errors que passen durant el funcionament de Apache2.
acces.log: Aquest arxiu registra les solicituds de acces al servidos, inclos els detalls cm la direccio Ip del client etc.
 ![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/2b2f8a5a-9e39-4700-b2a6-1b171918c2ed)


•	Rotación de logs: Investiga cómo funciona la rotación de logs en Apache2.
¿Por qué es importante? ¿Cómo se configura?

La rotacio de logs es important per mantener la integritat i el rendiment del sistema al evitar que els arxius del log creixin descontroladament i ocupin tot el espai del disc.

La configuracio de rotacio de logs es realitza en el arxiu de configuracio de logrotate, generalment ubicat en /etc/logrotate.d/. pots crear o modificar configuracions per Apache2 específicament en un arxiu, per exemple, /etc/logrotate.d/apache2.


•	Monitorización en tiempo real: Utiliza herramientas como tail -f para monitorear en tiempo real los accesos a tu servidor web y posibles errores
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/540ea318-3349-4d07-92bd-b9dd068e65a7)

 .
•	Análisis de logs: Instala y usa herramientas como goaccess para analizar y obtener estadísticas visuales a partir de tus logs de Apache2.
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/33e5af23-48ff-41a5-8014-9c7c38a4d15b)

.  
8.	¿Qué es un Firewall? ¿Para qué sirve? ¿Por qué es necesario? Instale y configure un Firewall en la máquina virtual para que solo permita tráfico HTTP y HTTPS. Bloquee todo el resto de los puertos y demuestre su funcionamiento.
Un firewall es una barrera de seguretat que controla i filtra el trafic de red que entra i surt d’una red informática o una maquina individual. La seva funcio principal es protetgir la red i els sistemes contra accesos no autoritzats i posibles amenaçes externes.
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/b8c966b9-20c0-415a-9f3a-65c2f54d6ef4)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/16668466-29cb-44fb-9494-6cb1bbff1e0e)
![image](https://github.com/Ramonenric/despliegue-de-aplicaciones-web/assets/95300566/b4675e89-6cbb-4276-9851-9f38480a3d01)

 
 
 
.
9.	Explica con tus palabras las diferentes partes de una URL.
Una URL esta formada per tres parts obligatories les quals son esquema, nom de domini, ruta. El esquema es la part inicial de la URL que especifica el protocol utilitzat per accedir al recurs. El nom de domini es la dirección web que representa la ubicació especifica d’internet on es esta guardat el recurs. La ruta es la part que segueix al domini i representa la ubicació especifica dins del lloc web on esta guardat el recurs. Per altra banda, hi han tres parts que son opcionals les cuals son subdomini, parametres i fragment.
.
10.	Explica el funcionamiento del protocolo HTTP con tus palabras.

El funcionament del protocol HTTP estableix una comunicación entre un client i un servidor, on el client solicita un recurs i el servidor respon proporcionant les dades corresponents. Això permet la navegació i el acces a continguts en la web d’una manera eficient i estructurada.
.





11.	¿Qué es un archivo .htaccess? Proporcione un ejemplo de cómo se puede utilizar para reescribir URL o restringir el acceso a ciertas partes de su sitio web.
Un arxiu .htaccess es un arxiu de configuracio utilitzat en servidors web Apache per controlar i modificar la configuracio del servidor en un directori especific i els seus subdirectoris. Permet definir normes i directives que afecten com es manipulen les solicitud i s’accedeixen a diferents parts d’un lloc web.,

1.	Reescritura de URLs:
	RewriteEngine On
RewriteRule ^producto/([^/]+)/?$ producto?id=$1 [L]

2.	Restriccion de acceso:
Order Deny,Allow
Deny from all
Allow from 192.168.1.1
