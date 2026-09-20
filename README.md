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

### 💻 Comandos practicados

```bash
nmap -v scanme.nmap.org
nmap -T4 scanme.nmap.org
nmap -sV -T4 scanme.nmap.org
 

### [16/09/2026] - Día 6: Intercepción de Tráfico HTTP con Burp Suite
Hoy integré el uso de proxies locales con los laboratorios avanzados de PortSwigger para manipular datos en tránsito.
- **Herramientas Utilizadas:** Burp Suite (Proxy Interceptor) y PortSwigger Web Academy.
- **Práctica Real:** Desplegué un proxy HTTP local en modo intercepción para capturar, analizar y auditar cabeceras y peticiones en tiempo real (`GET` / `POST`) antes de su recepción en el servidor objetivo.
- **Logro Técnico:** Realicé una manipulación de parámetros en caliente inyectando un carácter especial (`'`) en la carga útil (*payload*). Esto forzó una excepción en la lógica del backend, resultando en un Internal Server Error (500) debido a la falta de sanitización en la consulta SQL.
-
