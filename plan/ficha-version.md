# Ficha de versión · Kubuntu (VM gráfica)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Kubuntu 26.10 ("Stonking Stingray"), versión interina lanzada el 15 de octubre de 2026. | https://kubuntu.org/news/kubuntu-26-10-release-notes/ |
| Actualizaciones de seguridad | Soporte de actualizaciones de seguridad y correcciones críticas durante 9 meses (hasta julio de 2027), por ser versión interina. | https://kubuntu.org/news/kubuntu-26-10-release-notes/ |
| Requisitos de hardware y VirtualBox | Requisitos oficiales de la línea Ubuntu 26.x: CPU dual-core 2 GHz, 6 GB de RAM recomendados (4 GB mínimo no obligatorio), 25 GB de disco. Es compatible con VirtualBox 7.x; el proyecto fija el rango de la VM gráfica en 2-4 GB, así que asignaremos **3 GB de RAM**, 25 GB de disco y 2 CPU, dentro de lo permitido por la guía del curso. | https://www.omgubuntu.co.uk/2026/04/ubuntu-2604-system-requriments/embed |
| Particionado manual | Sí, el instalador Calamares permite particionado manual para crear `/`, `swap` y `/home`. | https://kubuntu.org/doc/ |
| Guía oficial de Docker Engine | Sí, mediante el repositorio oficial de Ubuntu (`apt`); en el proyecto, Docker se instala en la VM de consola, no en esta. | https://docs.docker.com/engine/install/ubuntu/ |
| Imagen base en Docker Hub | No aplica a esta VM (la imagen base asignada al Grupo 1 para el `Dockerfile` es Ubuntu). | https://hub.docker.com/ |

# Ficha de versión · Debian (VM de consola)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Debian 13 ("Trixie"), rama estable vigente, lanzada inicialmente el 9 de agosto de 2025. | https://www.debian.org/releases/trixie/ |
| Actualizaciones de seguridad | Soporte estándar del equipo de seguridad de Debian hasta aproximadamente agosto de 2028 (~3 años desde el lanzamiento), seguido de LTS hasta el 30 de junio de 2030. | https://www.debian.org/security/ |
| Requisitos de hardware y VirtualBox | Compatible con VirtualBox 7.x sin entorno gráfico. El proyecto asigna **2 GB de RAM** (ampliables a 3 GB en el Sprint 3 para Minikube), 25 GB de disco y 2 CPU. | https://www.debian.org/releases/stable/amd64/ch03s04.es.html |
| Particionado manual | Sí, el instalador de Debian permite particionado manual para crear `/`, `/var` (mínimo 10 GB), `swap` y `/home`. | https://www.debian.org/doc/ |
| Guía oficial de Docker Engine | Sí, guía oficial paso a paso para instalar Docker Engine desde el repositorio oficial de Docker para Debian. | https://docs.docker.com/engine/install/debian/ |
| Imagen base en Docker Hub | No aplica a esta VM (la imagen base asignada al Grupo 1 para el `Dockerfile` es Ubuntu). | https://hub.docker.com/ |

# Ficha de versión · Ubuntu (imagen base del Dockerfile)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Ubuntu 26.04 LTS (`ubuntu:26.04`), versión de soporte extendido más reciente, lanzada el 23 de abril de 2026. | https://ubuntu.com/about/release-cycle |
| Actualizaciones de seguridad | Soporte estándar de seguridad durante 5 años (hasta abril de 2031). | https://ubuntu.com/about/release-cycle |
| Requisitos de hardware y VirtualBox | No aplica máquina virtual propia; se usa solo como imagen base ligera de contenedor dentro de Docker, sobre el host Debian. | https://docs.docker.com/build/building/base-images/ |
| Particionado manual | No aplica (los contenedores usan el sistema de archivos en capas de Docker). | https://docs.docker.com/storage/ |
| Guía oficial de Docker Engine | Sí, Ubuntu cuenta con soporte y repositorio oficial completo en la documentación de Docker Engine. | https://docs.docker.com/engine/install/ubuntu/ |
| Imagen base en Docker Hub | Sí, disponible como *Docker Official Image* bajo el nombre `ubuntu` con etiqueta LTS verificada (`ubuntu:26.04`). | https://hub.docker.com/_/ubuntu |
