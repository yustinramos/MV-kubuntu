# Sprint 3: Scripts, Procesos, Docker y Kubernetes

[⬅ Volver a la portada](README.md)

## 1. Desarrollo y Despliegue
En este tercer sprint se desarrollaron herramientas de automatización en consola y entorno gráfico, se analizó el ciclo de vida de los procesos en Linux y se empaquetó y orquestó una aplicación mediante contenedores:

- **Automatización mediante scripts:** Creación de script de consola en Bash (`.sh`) y lanzador de aplicación gráfica (`.desktop`).
- **Gestión y simulación de procesos:** Ejecución controlada de `zombi.py` para observar procesos en estado zombi (`Z`) en la tabla de procesos del kernel.
- **Contenerización con Docker:** Construcción, etiquetado y publicación de una imagen personalizada en Docker Hub.
- **Orquestación con Minikube / Kubernetes:** Despliegue de pods y exposición del servicio en un clúster local de Kubernetes.

---

## 2. Comandos Utilizados
| Comando | Para qué sirve |
| :--- | :--- |
| `chmod +x script.sh` | Otorgar permisos de ejecución al script de consola |
| `python3 zombi.py &` | Ejecutar en segundo plano el script generador del proceso zombi |
| `ps aux \| grep Z` | Filtrar y verificar los procesos en estado zombi (`Z`) y su PID padre |
| `docker build -t usuario/imagen:v1 .` | Construir la imagen de contenedor a partir del `Dockerfile` |
| `docker push usuario/imagen:v1` | Subir la imagen generada al repositorio remoto en Docker Hub |
| `minikube start` | Iniciar el clúster local de Kubernetes |
| `kubectl apply -f deployment.yaml` | Aplicar el manifiesto de despliegue de pods y servicios en Kubernetes |
| `kubectl get pods` | Verificar que los pods desplegados estén en estado `Running` |

---

## 3. Evidencias Gráficas

### 3.1. Ejecución de script de consola y lanzador `.desktop`
![Scripts de consola y gráfico](img/scripts-consola-desktop.png)

### 3.2. Simulación y verificación de proceso zombi (`zombi.py`)
![Simulación de proceso zombi](img/proceso-zombi.png)

### 3.3. Construcción y publicación de imagen en Docker
![Construcción y push en Docker](img/docker-build-push.png)

### 3.4. Despliegue y estado de pods en Minikube / Kubernetes
![Despliegue en Kubernetes](img/kubernetes-pods.png)

---

## 4. Video de Sustentación

<iframe width="560" height="315" src="https://www.youtube.com/embed/ID_DEL_VIDEO" title="Sustentación Sprint 3 - Grupo 01" frameborder="0" allowfullscreen></iframe>
