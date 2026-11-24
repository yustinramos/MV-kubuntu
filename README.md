# Proyecto Final · Sistemas Operativos (750001C)

**Universidad del Valle** · Tecnología en Desarrollo de Software · Semestre 3-2026  
**Docente:** Mg. José Alexander Castañeda Muñoz  
**Grupo:** Grupo 01  
**Repositorio:** [yustinramos/MV-kubuntu](https://github.com/yustinramos/MV-kubuntu)

---

## 1. Descripción del Proyecto

Este sitio documenta el diseño, instalación, administración y despliegue de una infraestructura virtualizada compuesta por dos máquinas virtuales en **VirtualBox**: una estación cliente con entorno gráfico (**Kubuntu**, `g01-grafica`) y un servidor administrado en modo consola (**Debian 13**, `g01-consola`). A lo largo de tres sprints se implementaron particionado manual, conectividad en red, seguridad mediante llaves SSH y firewall, automatización con scripts, gestión de procesos y despliegue de contenedores con Docker y Kubernetes.

### Integrantes del Grupo 01

| Integrante | Usuario de GitHub | Rol / Aporte Principal |
| --- | --- | --- |
| Yustin Ramos | `@yustinramos` | Administración del repositorio, montaje de máquinas virtuales y configuración de red |
| Mariana Mejía | `@mejiamariana-desig` | Configuración de Kubuntu (`g01-grafica`) y Debian 13 (`g01-consola`), particionado manual, SSH y firewall |
| Yeraldin Rivera | `@riverayeraldin44-source` | Scripts de automatización, gestión de procesos, contenedores con Docker y despliegue en Kubernetes |

---

## 2. Documentación por Sprints

- [Sprint 1: Montaje, Particionado y Red](sprint-1.md) — Instalación de Kubuntu (`g01-grafica`) y Debian 13 (`g01-consola`), particionado manual, red, acceso SSH e instantáneas.
- [Sprint 2: Servicios, Llaves SSH y Firewall](sprint-2.md) — Configuración de OpenSSH, autenticación sin contraseña con llaves criptográficas y reglas UFW.
- [Sprint 3: Scripts, Procesos, Docker y Kubernetes](sprint-3.md) — Scripts `.sh` y `.desktop`, simulación de proceso zombi, imagen en Docker Hub y clúster en Minikube.

---

## 3. Distribuciones Utilizadas y Ficha Técnica

### 3.1. Máquina Cliente (`g01-grafica`) · Kubuntu

| Característica | Especificación |
| --- | --- |
| **Distribución y versión** | Kubuntu 24.04 LTS (Noble Numbat) |
| **Arquitectura** | `amd64` (x86_64) |
| **Entorno de escritorio** | KDE Plasma (modo gráfico) |
| **Rol en el proyecto** | Estación cliente para administración remota por SSH, pruebas de red y entorno gráfico |
| **Almacenamiento** | Disco virtual dinámico (`VDI`) con sistema de archivos `ext4` |

### 3.2. Máquina Servidor (`g01-consola`) · Debian 13

| Característica | Especificación |
| --- | --- |
| **Distribución y versión** | Debian GNU/Linux 13.7.0 (*Trixie*) · NETINST |
| **Arquitectura** | `amd64` (x86_64) |
| **Modo de arranque** | Consola pura (`multi-user.target`, sin entorno gráfico) |
| **Rol en el proyecto** | Servidor de servicios SSH, firewall UFW, ejecución de procesos y contenedores |
| **Disco y particionado (`/dev/sda` · 26.8 GB)** | `/` (`12.0 GB`, `ext4`), `/var` (`4.0 GB`, `ext4`), `swap` (`2.0 GB`), `/home` (`8.8 GB`, `ext4`) |

---

## 4. Cuadro Comparativo del Instalador

| Criterio | Instalador de Kubuntu (Calamares) | Instalador de Debian 13 (NETINST Modo Texto) |
| --- | --- | --- |
| **Interfaz de usuario** | Gráfica, asistida con ratón y ventanas visuales | Basada en menús numerados en consola (sin interfaz gráfica) |
| **Consumo de recursos durante instalación** | Mayor uso de memoria RAM por cargar el entorno Live KDE | Mínimo consumo de RAM y CPU; ideal para servidores |
| **Particionado de disco** | Visual mediante barras gráficas y asistentes automáticos | Manual y granular por sectores/tamaños exactos y puntos de montaje |
| **Selección de paquetes (`tasksel`)** | Instala suite completa de escritorio y aplicaciones ofimáticas | Permite elegir únicamente utilidades estándar del sistema y servidor SSH |
| **Dependencia de red** | Instala el sistema base desde la imagen ISO local sin conexión obligatoria | Descarga los paquetes actualizados directamente desde réplicas (`deb.debian.org`) |
| **Perfil recomendado** | Usuarios finales, estaciones de trabajo y entornos de escritorio | Servidores de producción, infraestructura cloud y administración remota |

---

## 5. Conclusiones por Integrante

### Yustin Ramos (`@yustinramos`)
> *Conclusión pendiente por redactar en el cierre del Sprint 3 sobre el montaje de máquinas virtuales, gestión de repositorios con GitHub Pages y administración de redes.*

### Mariana Mejía (`@mejiamariana-desig`)
> *Conclusión pendiente por redactar en el cierre del Sprint 3 sobre la configuración de Kubuntu (`g01-grafica`), el particionado manual en Debian 13 (`g01-consola`) y la seguridad con llaves SSH y firewall.*

### Yeraldin Rivera (`@riverayeraldin44-source`)
> *Conclusión pendiente por redactar en el cierre del Sprint 3 sobre la automatización con scripts en Bash, el manejo de procesos en Linux y el despliegue con Docker y Kubernetes.*

---

## 6. Declaración de Uso de Inteligencia Artificial (IA)

Para el desarrollo y documentación de este proyecto se utilizaron herramientas de Inteligencia Artificial generativa como apoyo técnico y de redacción, bajo supervisión y verificación directa de los integrantes del grupo:

- **Herramienta utilizada:** Google Gemini.
- **Propósito de uso:** Apoyo en la estructuración de las páginas en formato Markdown, verificación de sintaxis para GitHub Pages, resolución de dudas durante el particionado manual de Debian 13 y revisión de comandos de administración en Linux.
- **Validación humana:** Todos los comandos, configuraciones de red, reglas de firewall, scripts, capturas de pantalla y videos de sustentación fueron ejecutados, comprobados y documentados directamente por los integrantes del Grupo 01 en sus propias máquinas virtuales.
