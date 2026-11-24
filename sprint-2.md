# Sprint 2 · SSH, Llaves SSH y Firewall

[⬅ Volver a la portada](README.md)

## 1. Configuración de Servicios y Seguridad
Configuración de acceso remoto por **SSH**, autenticación sin contraseña mediante **llaves SSH** y reglas de **firewall** entre `g01-grafica` y `g01-consola`[cite: 2].

## 2. Comandos utilizados
| Comando | Para qué sirve |
| :--- | :--- |
| `ssh-keygen` | Generar el par de llaves pública y privada |
| `ssh-copy-id usuario@IP` | Copiar la llave pública al servidor destino |
| `sudo ufw status` | Verificar el estado y las reglas del firewall |
| `sudo ufw allow ssh` | Permitir conexiones entrantes por el puerto SSH |

## 3. Evidencias
![Conexión SSH](img/ssh-conexion.png)

![Estado Firewall](img/firewall-ufw.png)

## 4. Video de sustentación
<iframe width="560" height="315" src="https://www.youtube.com/embed/ID_DEL_VIDEO" title="Sprint 2" frameborder="0" allowfullscreen></iframe>
