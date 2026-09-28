Ruta-Ciberseguridad-SENATI
# Mi Ruta de Aprendizaje en Ciberseguridad 🚀
Repositorio creado para documentar mi preparación técnica antes y durante mis estudios en SENATI.

## 🗓️ Bitácora Diario

### [11/09/2026] - Día 1: Infraestructura y Fundamentos de la CLI
Hoy inicié mi preparación desde cero con un enfoque híbrido (PC + Celular), logrando los siguientes hitos:

- **Portafolio:** Configuración de este repositorio en GitHub para registrar mi constancia y progreso diario.
- **Laboratorio Local:** Instalación exitosa de VirtualBox 7.2.16 y despliegue operativo de la máquina virtual Kali Linux en mi PC.
- **Fundamentos Web:** Comprensión del protocolo HTTP, métodos de petición (GET/POST) y manejo de códigos de estado como el Error 404 Not Found.
- **Plataformas de Estudio:** Desbloqueo del módulo 'Linux Fundamentals' en Hack The Box Academy utilizando cubos gratuitos de la plataforma.
- **Práctica Técnica (CLI de Linux):** Dominé el uso de la terminal negra para administrar el sistema operativo sin usar el mouse mediante los comandos:
  - `pwd` (Identificar ruta actual)
  - `ls` (Listar contenido de directorios)
  - `mkdir` (Crear carpetas de auditoría)
  - `cd` (Navegar y entrar a directorios)
  - `echo >` (Redirigir e inyectar texto para crear reportes en archivos .txt)
  - `cat` (Lectura y visualización rápida del contenido de archivos)
- **Troubleshooting:** Aprendí a leer los errores de sintaxis del sistema (mayúsculas y comas erróneas) para corregir los comandos en caliente hasta lograr la ejecución exitosa.
 VirtualBox instalado y máquina Kali Linux operativa en el primer intento.
 
### [12/09/2026] - Día 2
: Conquista Total de Linux Fundamentals
Hoy cerré de golpe todo el bloque interactivo en la nube de Hack The Box Academy, completando las 30 secciones técnicas del examen y obteniendo mi primera insignia profesional.

- **Secciones Dominadas:**
  - Administración de archivos, directorios y descriptores de redirección.
  - Búsqueda avanzada y filtrado de contenidos masivos (`grep`, comandos de flujo).
  - Gestión de usuarios, políticas de bloqueo, control de servicios (`systemctl`) y manejo de particiones de disco.
- **Hito Técnico:** Finalización

### [13/09/2026] - Día 3: Regularización de HTB y Auditoría Web Manual (PortSwigger)
Hoy consolidé mi conocimiento de sistemas y di mis primeros pasos en el hackeo de aplicaciones web.
- **Consolidación Técnica:** Repetí de forma manual los laboratorios de Hack The Box en mi consola local para asegurar el conocimiento real de comandos base.
- **Laboratorio PortSwigger (SQL Injection):** Accedí a mi primer entorno controlado. Manipulé los parámetros de la URL de forma manual introduciendo caracteres especiales (`'`) para alterar la lógica de la base de datos del servidor y analizar fallas en la infraestructura web.

### [14/09/2026] - Día 4: Clonación de Herramientas y Automatización CLI en Kali
Hoy pasé a la acción real descargando y ejecutando scripts externos en mi laboratorio local de Kali Linux.
- **Comandos Practicados:**
  - `sudo apt update` (Actualización y sincronización de las listas de repositorios del sistema).
  - `git clone [URL]` (Descarga directa de herramientas de hacking desde GitHub a la terminal).
 
  ## [15/09/2026] - Día 5: Reconocimiento de redes con Nmap

Hoy comencé a practicar reconocimiento de redes utilizando Nmap sobre `scanme.nmap.org`, un objetivo destinado a prácticas.

### 🧪 Práctica realizada

- Ejecuté un escaneo básico con `nmap`.
- Practiqué el ajuste de velocidad mediante `-T4`.
- Utilicé `-sV` para identificar servicios y versiones.
- Analicé puertos abiertos y comprendí su relación con los servicios.

### 🔎 Conceptos aprendidos

- Una **IP** identifica un equipo dentro de una red.
- Un **puerto** es un punto de comunicación utilizado por los servicios.
- `open` indica que Nmap detectó un servicio aceptando conexiones.
- `closed` indica que el puerto es accesible, pero no hay un servicio escuchando.
- `filtered` significa que un firewall o filtro impide determinar claramente el estado.
- `-sV` permite intentar identificar el servicio y su versión.
- `-T4` modifica la temporización para realizar el escaneo más rápidamente.



### [16/09/2026] - Día 6: Intercepción de Tráfico HTTP con Burp Suite
Hoy integré el uso de proxies locales con los laboratorios avanzados de PortSwigger para manipular datos en tránsito.
- **Herramientas Utilizadas:** Burp Suite (Proxy Interceptor) y PortSwigger Web Academy.
- **Práctica Real:** Desplegué un proxy HTTP local en modo intercepción para capturar, analizar y auditar cabeceras y peticiones en tiempo real (`GET` / `POST`) antes de su recepción en el servidor objetivo.
- **Logro Técnico:** Realicé una manipulación de parámetros en caliente inyectando un carácter especial (`'`) en la carga útil (*payload*). Esto forzó una excepción en la lógica del backend, resultando en un Internal Server Error (500) debido a la falta de sanitización en la consulta SQL.

### [17/09/2026] - Día 7: Automatización de Ataques de Fuerza Bruta con Burp Intruder
Hoy completé con éxito el laboratorio avanzado de enumeración y evasión de mecanismos de autenticación.
- **Herramientas Utilizadas:** Burp Suite (Intruder Module) y PortSwigger Web Academy.
- **Práctica Real:** Intercepté un flujo de login defectuoso y configuré vectores de ataque dirigidos (*Sniper mode*) cargando diccionarios dinámicos en los parámetros de autenticación.
- **Logro Técnico:** Exploté la vulnerabilidad analizando las sutiles variaciones en las respuestas del servidor web (*Response Length* y redirecciones *302*), logrando extraer el usuario y la contraseña correctos para comprometer la cuenta objetivo. ¡Laboratorio marcado como SOLVED!
-
### [18/09/2026] - Día 8: Explotación de Vulnerabilidades de Lógica de Negocio con Burp Repeater
Hoy audité flujos transaccionales web para identificar fallas en la validación de parámetros críticos del lado del servidor.
- **Herramientas Utilizadas:** Burp Suite (Repeater Module) y PortSwigger Web Academy.
- **Práctica Real:** Intercepté solicitudes de canje de productos (`POST /cart`) y las trasladé al módulo Repeater para realizar pruebas de manipulación de datos repetitivas sin alterar la sesión del navegador.
- **Logro Técnico:** Identifiqué una vulnerabilidad de confianza excesiva en controles del lado del cliente (*Excessive trust in client-side controls*). Al modificar el parámetro de precio en tránsito antes de su procesamiento en el backend, demostré la falta de validación de integridad en el servidor, adquiriendo un artículo de alto valor por una fracción de su costo original y marcando el laboratorio como SOLVED.

### [18/09/2026] - Día 9: Rompiendo Contraseñas de Red mediante Fuerza Bruta Local con Hydra
Hoy ejecuté pruebas de robustez de autenticación sobre servicios de administración remota directamente en un entorno local seguro.
- **Herramientas Utilizadas:** Hydra (Network Logon Cracker) y Kali Linux CLI.
- **Práctica Real:** Configuré un vector de ataque por diccionario dirigido contra el servicio SSH de la máquina virtual para evaluar la resistencia del sistema ante ataques de diccionario masivos.
- **Logro Técnico:** Desplegué un análisis de fuerza bruta automatizado utilizando diccionarios criptográficos, identificando con éxito las credenciales válidas del usuario local en pocos segundos y consolidando el conocimiento práctico sobre la velocidad de procesamiento de Hydra.

#### 🛠️ Comandos y Payloads Utilizados:
- `sudo systemctl start ssh`
  - **¿Para qué servía?** Abre el puerto de administración remota (SSH) en tu propia computadora Linux para simular que eres un servidor web real en producción listo para recibir conexiones o auditorías.
- `sudo gunzip /usr/share/wordlists/rockyou.txt.gz`
  - **¿Para qué servía?** Descomprime el famoso diccionario `rockyou.txt` que viene archivado de fábrica en Kali Linux. Este archivo contiene millones de contraseñas reales filtradas en internet y se necesita tener suelto para que las herramientas de hacking puedan leerlo.
- `hydra -l kali -P /usr/share/wordlists/rockyou.txt -t 1 -w 3 ssh://127.0.0.1`
  - **¿Para qué servía?** Activa a la herramienta Hydra (el robot abrepuertas automático). El parámetro `-l` define el usuario objetivo (`kali`), `-P` carga el diccionario de claves descompreso, `-t 1` le dice que intente una sola contraseña a la vez y `-w 3` mete una pausa de 3 segundos entre intentos para engañar los sistemas de seguridad locales, atacando a la dirección IP universal de pruebas `127.0.0.1`.

 ### [19/09/2026] - Día 10: Inyección de Código del Lado del Cliente mediante Reflected XSS
Hoy ejecuté auditorías de seguridad web enfocadas en la sanitización y validación de entradas de usuario para mitigar fallas de Cross-Site Scripting.
- **Herramientas Utilizadas:** Burp Suite (Navegador Integrado) y PortSwigger Web Academy.
- **Práctica Real:** Analicé el comportamiento de los parámetros de búsqueda en el backend (`GET /?search=`) para evaluar si los datos de entrada se reflejaban de manera directa en el código fuente HTML sin pasar por filtros de codificación.
- **Logro Técnico:** Exploté con éxito una vulnerabilidad de XSS Reflejado en contexto HTML, forzando al navegador web a interpretar código arbitrario en el contexto de la sesión y marcando el laboratorio como SOLVED.

#### 🛠️ Comandos y Payloads Utilizados:
- `<script>alert(1)</script>`
  - **¿Para qué servía?** Es una carga útil (*payload*) escrita en JavaScript. Le ordena al navegador web de la víctima romper la lectura normal de la página y forzar de forma agresiva la apertura de una ventana flotante de alerta con el número 1 en medio de la pantalla. Sirve para demostrar visualmente que un atacante puede inyectar virus o scripts maliciosos en la web debido a que el programador olvidó limpiar o sanitizar el cuadro de búsqueda.

### [21/09/2026] - Día 11: Escalada de Privilegios Local (Sudo Misconfiguration)
Hoy practiqué la fase de post-explotación para elevar mis privilegios de usuario común a Administrador (Root) directamente en un entorno local controlado.
- **Herramientas Utilizadas:** Linux CLI (Bash/Bdash) y Kali Linux Virtual Environment.
- **Práctica Real:** Audité las directivas de seguridad locales para entender el funcionamiento del archivo *sudoers* y simular la explotación de permisos excesivos en sistemas operativos basados en Linux.
- **Logro Técnico:** Ejecuté un análisis de privilegios mediante la consola y forcé un escape de entorno (*breakout*), logrando obtener una shell interactiva con el rol de superusuario (`#`) a costo cero y de forma autónoma.

#### 🛠️ Comandos y Payloads Utilizados:
- `sudo -l`
  - **¿Para qué servía?** Es el comando de reconocimiento interno más importante en seguridad Linux. Le pide al sistema operativo que te muestre una lista detallada con todos los programas que tu usuario actual tiene permitido ejecutar con permisos de administrador ("superpoderes"). Sirve para que los auditores encuentren fallas de configuración (*misconfigurations*) en los servidores de las empresas.
- `sudo bdash` (o `sudo bash`)
  - **¿Para qué servía?** Es el comando de explotación y elevación. Aprovecha los permisos del intérprete de comandos para romper la jaula del usuario básico y regalarte una consola avanzada con el símbolo `#`. Te convierte instantáneamente en el usuario supremo `root`, dándote el poder absoluto de borrar, editar o crear carpetas en cualquier disco de la computadora.

### [22/09/2026] - Día 12: Descubrimiento de Paneles Ocultos mediante Fuga de Información en Robots.txt
Hoy audité un sitio web en PortSwigger utilizando técnicas de reconocimiento pasivo en la URL para evadir la seguridad sin necesidad de interceptar tráfico.
- **Herramientas Utilizadas:** Navegador Web y PortSwigger Web Academy.
- **Práctica Real:** Inspeccioné los archivos de configuración públicos del servidor indexados para motores de búsqueda con el fin de rastrear directorios ocultos o privados de la empresa.
- **Logro Técnico:** Identifiqué una ruta administrativa crítica expuesta de forma insegura, lo que me permitió ingresar directamente al panel de control central y marcar el laboratorio como SOLVED.

#### 🛠️ Comandos y Payloads Utilizados:
- `/robots.txt`
  - **¿Para qué servía?** Es un archivo de texto público que los creadores de páginas web ponen en el servidor para decirle a los buscadores (como Google) qué carpetas tienen permitido revisar y cuáles deben ignorar. Al escribirlo al final de la URL, obligué al servidor a enseñarme su lista de exclusiones, donde el programador cometió el grave error de confesar la ubicación exacta de la carpeta secreta de administración.
- `/administrator-panel` (o la ruta exacta que te dio el archivo)
  - **¿Para qué servía?** Es el enlace directo al panel del jefe que descubrí gracias al archivo anterior. Al pegarlo en la barra de direcciones de la URL, salté directamente al centro de control sin que la página me pidiera contraseña, demostrando que el sitio web sufre de una falla crítica de control de acceso.

### [23/09/2026] - Día 13: Ataque CSRF Manual (Cross-Site Request Forgery)

Hoy exploté una vulnerabilidad CSRF en PortSwigger, obligando al navegador de una víctima a cambiar su correo sin que ella hiciera clic en nada.

- **Herramientas Utilizadas:** Navegador Web, PortSwigger Academy y creación manual de HTML.
- **Práctica Real:** Identifiqué que la petición de cambio de correo no tenía token anti-CSRF y construí un formulario HTML malicioso para alojarlo en el servidor de exploits.
- **Logro Técnico:** Al enviar el exploit, el navegador de la víctima usó su propia cookie de sesión para autorizar el cambio de correo. Laboratorio **SOLVED**.

#### 🛠️ Comandos y Payloads Utilizados:
- `<form action="URL/my-account/change-email" method="POST">`
  - **¿Para qué servía?** Estructura el formulario malicioso apuntando directamente a la función vulnerable del servidor.
- `<script>document.forms[0].submit();</script>`
  - **¿Para qué servía?** Obliga al navegador de la víctima a enviar el formulario automáticamente al cargar la página, usando su sesión activa.
    
  ### [24/09/2026] - Día 14: SSRF (Server-Side Request Forgery) para acceder a la red interna
Hoy exploté una vulnerabilidad SSRF en PortSwigger, obligando al servidor web a realizar peticiones a su propia red interna para acceder a un panel de administración oculto.

Herramientas Utilizadas: Navegador Web, Burp Suite Community y PortSwigger Academy.

Práctica Real: Identifiqué que la función "Check stock" realizaba peticiones a una URL controlable. Al interceptar el tráfico, cambié la URL original por http://localhost/admin para forzar al servidor a mostrarme su panel interno.

Logro Técnico: Accedí al panel de administración interno y ejecuté la eliminación del usuario carlos a través del propio servidor. Laboratorio SOLVED.

🛠️ Comandos y Payloads Utilizados:
stockApi=http://localhost/admin

¿Para qué servía? Engaña al servidor para que se haga una petición a sí mismo en el puerto local (localhost), saltándose el firewall perimetral y mostrando el panel de administración que solo debería ser visible internamente.

stockApi=http://localhost/admin/delete?username=carlos

¿Para qué servía? Ejecuta una acción administrativa (borrar al usuario carlos) usando la confianza que el servidor tiene en sí mismo, demostrando el impacto crítico del SSRF.

### [25/09/2026] - Día 15: Ejecución Remota de Comandos (RCE) mediante File Upload

Hoy exploté una vulnerabilidad de subida de archivos en PortSwigger, logrando leer archivos internos del servidor (RCE) y obteniendo el control total de la máquina.

- Herramientas Utilizadas: Navegador Web, Burp Suite Community y PortSwigger Academy.
- Práctica Real: Intercepté la petición de subida de avatar con Burp Suite y modifiqué el contenido del archivo a código PHP malicioso. El servidor no validó correctamente el tipo de archivo.
- Logro Técnico: Subí el archivo `myexploit.php` al servidor, accedí a él vía URL y logré leer el archivo `/etc/passwd` (para verificar la vulnerabilidad) y el archivo secreto de Carlos (`/home/carlos/secret`). Laboratorio **SOLVED**.

#### 🛠️ Comandos y Payloads Utilizados:

1. `myexploit.php`
   - **¿Para qué servía?** Simula una imagen para engañar al servidor, pero en realidad es un script en PHP listo para ser ejecutado.

2. `<?php echo file_get_contents('/etc/passwd'); ?>`
   - **¿Para qué servía?** Payload inyectado en el archivo PHP. Le ordena al servidor leer el archivo de usuarios del sistema y mostrarlo en pantalla, confirmando la ejecución remota de código.

3. `<?php echo file_get_contents('/home/carlos/secret'); ?>`
   - **¿Para qué servía?** Payload final. En lugar de ejecutar comandos, le dice al servidor que lea directamente el archivo secreto de Carlos y nos lo muestre en el navegador para resolver el reto.
  
     ### [26/09/2026] - Día 16: Transición a Hack The Box (HTB) y Compromiso de la Máquina "Meow"

Hoy di el salto de los laboratorios web guiados a la explotación de máquinas completas en Hack The Box, utilizando el entorno Pwnbox y comprometiendo mi primer sistema objetivo.

- **Herramientas Utilizadas:** HTB Pwnbox (Kali Linux), Nmap y Telnet.
- **Práctica Real:** Desplegué la máquina "Meow" en HTB y realicé un escaneo de puertos para identificar servicios expuestos.
- **Logro Técnico:** Descubrí el puerto 23 (Telnet) abierto, accedí al sistema como usuario root (sin contraseña) y capturé la flag para completar la máquina con éxito.

#### 🛠️ Comandos y Payloads Utilizados:

1. `nmap -sV 10.129.250.69`
   - **¿Para qué servía?** Realiza un escaneo de puertos y servicios para descubrir que el puerto 23 (Telnet) estaba abierto en la máquina víctima.

2. `telnet 10.129.250.69`
   - **¿Para qué servía?** Se conecta al servicio Telnet de la máquina víctima. Al no tener contraseña el usuario root, permite el acceso directo al sistema operativo.

3. `cat flag.txt`
   - **¿Para qué servía?** Lee el archivo que contiene la flag (la "bandera" del reto) para demostrar que hemos comprometido la máquina y poder subirla a la plataforma.
   ### [27/09/2026] - Día 17: Compromiso de la Máquina "Fawn" en Hack The Box (HTB)

Hoy continué con el Starting Point de HTB, comprometiendo la máquina "Fawn" mediante la explotación de un servidor FTP con acceso anónimo mal configurado.

- **Herramientas Utilizadas:** HTB Pwnbox, Nmap y cliente FTP.
- **Práctica Real:** Desplegué la máquina "Fawn", realicé un escaneo de puertos y detecté el servicio FTP (puerto 21) activo. Intenté el acceso anónimo estándar, pero el servidor lo rechazó. Realicé pruebas de troubleshooting y logré autenticarme usando el usuario "ftp" sin contraseña.
- **Logro Técnico:** Accedí al servidor FTP, listé los archivos disponibles, descargué el archivo `flag.txt` alojado en el servidor, lo leí y completé la máquina con éxito.

#### 🛠️ Comandos y Payloads Utilizados:

1. `nmap -sV <IP_DE_FAWN>`
   - **¿Para qué servía?** Escaneo de puertos para identificar que el puerto 21 (FTP) estaba abierto y aceptaba conexiones.

2. `ftp <IP_DE_FAWN>`
   - **¿Para qué servía?** Establece la conexión con el servidor FTP vulnerable.

3. `ftp` (Usuario) + Enter (Contraseña)
   - **¿Para qué servía?** Inicia sesión en el servidor FTP. Tras fallar con "anonymous", el usuario "ftp" sin contraseña permitió el acceso exitoso (230 Login successful).

4. `ls`
   - **¿Para qué servía?** Lista los archivos y directorios dentro del servidor FTP remoto. Permitió descubrir el archivo exacto llamado `flag.txt` antes de descargarlo.

5. `get flag.txt`
   - **¿Para qué servía?** Descarga el archivo que contiene la flag desde el servidor víctima a mi máquina local para poder leerlo.

6. `cat flag.txt`
   - **¿Para qué servía?** Lee el contenido del archivo descargado en la terminal para obtener la flag final.
