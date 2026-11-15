
# Ficha de versión · Kubuntu (VM gráfica)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Kubuntu 24.04 LTS (Noble Numbat), lanzada el 25 de abril de 2024. | https://kubuntu.org/ |
| Actualizaciones de seguridad | Soporte oficial de seguridad durante 3 años (hasta abril de 2027). | https://kubuntu.org/ |
| Requisitos y VirtualBox | Compatible con VirtualBox 7.x. Se asignarán **3 GB de RAM** (dentro del rango permitido de 2 a 4 GB), **25 GB de disco** y **2 CPU** para asegurar fluidez del escritorio KDE Plasma y los navegadores sin afectar el equipo anfitrión. | https://kubuntu.org/getkubuntu/ |
| Particionado manual | Sí, el instalador Calamares permite particionado manual para crear `/`, `swap` y `/home`. | https://kubuntu.org/doc/ |
| Guía oficial de Docker Engine | Sí, soporta instalación oficial mediante el repositorio de Ubuntu (`apt`), aunque en el proyecto Docker se instalará en la VM de consola. | https://docs.docker.com/engine/install/ubuntu/ |
| Imagen base en Docker Hub | No aplica (la imagen base asignada al Grupo 01 para el `Dockerfile` es Ubuntu). | https://hub.docker.com/ |

# Ficha de versión · Debian (VM de consola)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Debian 13 (Trixie), rama estable vigente. | https://www.debian.org/releases/ |
| Actualizaciones de seguridad | Soporte estándar de 3 años por el equipo de seguridad de Debian más 2 años adicionales de LTS (5 años en total). | https://www.debian.org/security/ |
| Requisitos y VirtualBox | Compatible con VirtualBox 7.x sin entorno gráfico. Se asignarán **2 GB de RAM** (ampliables a **3 GB** en Sprint 3 para Minikube), **25 GB de disco** y **2 CPU**. | https://www.debian.org/releases/stable/amd64/ch03s04.es.html |
| Particionado manual | Sí, el instalador de Debian permite particionado manual para crear `/`, `/var` (mínimo 10 GB), `swap` y `/home`. | https://www.debian.org/doc/ |
| Guía oficial de Docker Engine | Sí, cuenta con guía oficial paso a paso para instalar Docker Engine desde el repositorio oficial de Docker para Debian. | https://docs.docker.com/engine/install/debian/ |
| Imagen base en Docker Hub | No aplica (la imagen base asignada al Grupo 01 para el `Dockerfile` es Ubuntu). | https://hub.docker.com/ |

# Ficha de versión · Ubuntu (Imagen base Dockerfile)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Ubuntu 24.04 LTS (`ubuntu:24.04`), lanzada el 25 de abril de 2024. | https://ubuntu.com/about/release-cycle |
| Actualizaciones de seguridad | Soporte estándar de seguridad durante 5 años (hasta abril de 2029). | https://ubuntu.com/about/release-cycle |
| Requisitos y VirtualBox | No aplica máquina virtual propia; se emplea únicamente como imagen base ligera de contenedor dentro de Docker. | https://docs.docker.com/build/building/base-images/ |
| Particionado manual | No aplica (los contenedores utilizan el sistema de archivos en capas de Docker sobre el host Debian). | https://docs.docker.com/storage/ |
| Guía oficial de Docker Engine | Sí, Ubuntu cuenta con soporte y repositorio oficial completo en la documentación de Docker Engine. | https://docs.docker.com/engine/install/ubuntu/ |
| Imagen base en Docker Hub | Sí, disponible como *Docker Official Image* bajo el nombre `ubuntu` con etiquetas LTS verificadas. | https://hub.docker.com/_/ubuntu |
