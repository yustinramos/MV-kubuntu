# Plan de trabajo · Grupo 01 (Sede Santander Carvajal)

| Integrante | Rol | Qué hace |
|---|---|---|
| Yustin Ramos | Coordinación, repositorio y usuarios | Crea y administra el repositorio público en GitHub, sube el enlace al campus, gestiona usuarios/permisos (`/srv/proyecto`, `sudo`) y redacta documentación. |
| Mariana Mejía | Máquinas virtuales, red y sitio web | Instala Kubuntu (`g01-grafica`) y Debian (`g01-consola`), configura la red entre las VMs, SSH, llaves SSH y firewall, y construye el sitio web en GitHub Pages con las evidencias y videos de cada entrega. |
| Yeraldin Rivera | Scripts, procesos, Docker y Kubernetes | Desarrolla el script de consola, el script gráfico (`.desktop`) y `zombi.py`, instala Docker Engine, publica la imagen de Ubuntu en Docker Hub y despliega en Minikube/Kubernetes. |

## Cronograma y acuerdos de equipo · Sede Santander Carvajal

| Entrega | Fecha límite (Santander) | Responsable principal | Entregables clave |
|---|---|---|---|
| Sprint 0 · Arranque | Jueves 19 de noviembre | Todo el grupo (coordina Yustin) | Repositorio público, `plan/plan-de-trabajo.md` y `plan/ficha-version.md`. |
| Sprint 1 · Montaje | Jueves 26 de noviembre | Mariana y Yustin (apoya Yeraldin) | Instalación de VMs `g01-grafica` (Kubuntu) y `g01-consola` (Debian), red, SSH e instantánea `instalacion-limpia` por Mariana; documentación en repositorio por Yustin. |
| Sprint 2 · Servicios | Jueves 10 de diciembre | Todo el grupo | Usuarios, `/srv/proyecto` y `sudo` (Yustin); firewall y llaves SSH (Mariana); scripts `.sh`/`.desktop`, `zombi.py` y Docker Engine en Debian (Yeraldin). |
| Sprint 3 · Cierre | Jueves 17 de diciembre | Yeraldin y Mariana (apoya Yustin) | `Dockerfile` (base Ubuntu) en Docker Hub, despliegue en Minikube/Kubernetes y sitio web completo en GitHub Pages. |
| Sustentación final | Viernes 18 de diciembre | Todo el grupo | Exposición grupal de 6 minutos con sitio web y prueba individual de 2 minutos con las dos VMs encendidas. |

**Regla de colaboración:** Cada integrante realiza al menos 2 commits propios por sprint desde su cuenta de GitHub en los archivos de su rol, avisa antes de editar archivos de otra persona y participa en el video explicando su aporte.
