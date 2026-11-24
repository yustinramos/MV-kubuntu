# Sprint 2: Servicios, SSH, Llaves SSH y Firewall

[⬅ Volver a la portada](README.md)

## 1. Configuración de Servicios y Seguridad
En este segundo sprint se configuró y aseguró la comunicación remota entre la máquina cliente **Kubuntu (`g01-grafica`)** y el servidor **Debian 13 (`g01-consola`)**, implementando:

- **Servicio OpenSSH (`sshd`):** Habilitación de administración remota segura en el servidor.
- **Autenticación por llaves SSH:** Generación de par de llaves criptográficas en el cliente y autorización en el servidor para iniciar sesión sin contraseña.
- **Firewall (`ufw`):** Filtrado de tráfico entrante permitiendo únicamente el acceso por el puerto SSH (`22/tcp`).

---

## 2. Comandos Utilizados
| Comando | Para qué sirve |
| :--- | :--- |
| `sudo systemctl status ssh` | Verificar que el servicio servidor OpenSSH esté activo y en ejecución |
| `ssh-keygen -t ed25519` | Generar el par de llaves pública y privada en `g01-grafica` |
| `ssh-copy-id usuario@<IP>` | Copiar la llave pública al archivo `authorized_keys` de `g01-consola` |
| `ssh usuario@<IP>` | Comprobar el inicio de sesión remoto sin solicitar contraseña |
| `sudo ufw allow ssh` | Crear la regla del firewall para permitir conexiones entrantes por SSH |
| `sudo ufw enable` | Activar el cortafuegos UFW en el sistema |
| `sudo ufw status verbose` | Consultar el estado activo y las reglas aplicadas en el firewall |

---

## 3. Evidencias Gráficas

### 3.1. Estado del servicio SSH y conexión inicial (`g01-consola`)
![Servicio y Conexión SSH](img/ssh-conexion.png)

### 3.2. Generación de llaves SSH y acceso sin contraseña
![Llaves SSH y acceso sin contraseña](img/llaves-ssh.png)

### 3.3. Reglas y estado activo del firewall (`ufw`)
![Estado Firewall UFW](img/firewall-ufw.png)

---

## 4. Video de Sustentación

<iframe width="560" height="315" src="https://www.youtube.com/embed/ID_DEL_VIDEO" title="Sustentación Sprint 2 - Grupo 01" frameborder="0" allowfullscreen></iframe>
