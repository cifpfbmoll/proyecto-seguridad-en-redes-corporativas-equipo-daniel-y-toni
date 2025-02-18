[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/A04QAW6X)
# El objetivo del sprint1 es aumentar la seguridad del servidor según los estandares cis_level2_server, puntos a tratar:

Auditar según cis_level2_server
Aplicar reglas cis_level2_server
Configuración de arranque GRUB
Establecer permisos de fichero de configuración de arranque
Establecer contraseña de arranque
Obligar al uso de contraseña en el modo single user
Comprobación de usuario administrador
Comprobación de complimiento con recomendaciones sobre actualizaciones de software
Auditoria final del servidor

# Para el sprint 2 queremos introducir un software de copias de seguridad y probar su funcionamiento, se dividirá en:

Instalación de Duplicati
Creación de primera copia de prueba
Pruebas de restauración de la primera copia
Creación de la segunda copia
Pruebas de recuperación de la segunda copia

# En el tercer sprint vamos a asegurarnos de que nuestro servidor apache sea seguro, para ello haremos las siguientes tareas:

Instalación de apache
Configuraciones globales:
  - Ficheros de configuraciones
  - Configuración de usuarios y grupos
  - Ocultación de versiones. 
  - Exposición mínima de módulos.
  - Creación de virtualhost con tu nombre y apellido.
  - Configuración múltiple y de contexto: directiva options.
Investigar ficheros .htaccess.
evitar el hotlinking
Configuración HTTPS mediante OpenSSL. Creacion de certificados para que virtualHost sea seguro, y obligatoriamente los accesos sean por HTTPS
Investigar el módulo mod_security.
Descarga de Kali Linux ataque DoS mediante Metasploit (Slowloris)
Clonar e instalar las reglas recomendadas OWASP. Habilitar mod_security
Reglas para detectar SQLInjection
Realizar de nuevo el ataque DoS y comprueba que el servidor está accesible.

# El cuarto sprint consiste en hardening de SSH, evitaremos accesos indeseados por esta via.

Autenticación SSH siempre basada en clave pública.
Cambio de puerto por defecto.
Comprobación de límite la vinculación IP
Deshabilitar el usuario ROOT para login
Limitar el acceso SSH de los usuarios del sistema. Comprobar la limitación.
Deshabilitar inicio de sesión basado en contraseña.
Deshabilitar contraseñas vacías. 
Limitar intentos de autenticación fallida.
Limitar conexiones simultaneas no autenticadas.
Habilitar un banner de advertencia para los usuarios de SSH.
Configurar el intervalo de tiempo de espera de cierre de sesión inactiva.
Deshabilitar X11forwarding.
Chroot (Bloquear usuarios a sus directorios de inicio).
Investigar como habilitar el doble factor de autenticación en el servicio SSH, configurar y comprobar su correcto funcionamiento.

# El objetivo del sprint 5 es conocer las principales herramientas de reconocimiento de vulnerabilidades, y especialmente familiarizarnos con la herramienta Nmap. Para ello realizaremos una serie de tareas:

- Descarga e importación de la maquina metasploitable2.
- Escaneo utilizando SYN Scan y reconocimiento de los principales servicios de metasplotaible 2 y nuestro servidor. Comparación de resultados.
- Escaneo de los principales puertos UDP abiertos en la máquina metasplotaible2.
- Escaneo lanzando el script vuln sobre metasplotaible 2 y nuestro servidor. Comparación de resultados.
- Escaneo agresivo sobre metasplotaible 2 y nuestro servidor. Comparación de resultados.
- Escaneo únicamente de descubrimiento de equipos en la red domestica.

# El objetivo del sprint 6 es poner en práctica los conocimientos adquiridos sobre seguridad perimetral, y aplicar una arquitectura Screened Subnet (DMZ) que asegure perimetralmente el sistema. Seguiremos unos sencillos pasos:

- Instalación de PfSense y configuración de 3 tarjetas de red.
- Configuración de un equipo empleado.
- Configuración del servidor.
- Comprobaciones pre-reglas.
- Configuración de reglas.

# El objetivo del sprint 7 es poner en práctica los conocimientos adquiridos sobre seguridad perimetral, y configurar el cortafuegos pfSense habilitando el servicio IDS/IPS Suricata y un servidor VPN de manera que permita a los empleados de la empresa conectarse desde redes públicas o teletrabajar de manera segura.

- Instalar IDS/IPS Suricata.
- Aplicar las reglas de la comunidad Snort.
- Antes de habilitar Suricata, realizar un ataque DoS sobre el servidor Web. 
- Habilitar el IDS en modo IPS (Legacy Mode), y repetir el ataque.
- Habilitar el servidor VPN en pfSense.
- Añadir ntopng.

# El objetivo del sprint 8 es poner en práctica los conocimientos sobre balanceo de carga con Apache que hará tarea de proxy inverso y balanceador de carga.

-  Configuración de Apache en modo proxy inverso.
- Configurar Apache en modo Balanceador de carga.
- Realizar una configuración básica para que los equipos de la LAN pasen por el proxy caché.
