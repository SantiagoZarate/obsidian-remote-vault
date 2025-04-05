**POSTGRES**
su - postgres

**LINUX**
env
consultar variables de entorno

echo $USER

export

Setear una variable de entorno

service --status-all

Consultar servicios activos en el background

service ssh start

Start a service

GROUPS

Consultar los grupos del sistema

```bash
cat /etc/group
```

ROOT

Entrar en modo superuser

```bash
sudo -i
```

SSH

ssh <password>@<ip> -p 2200

ssh root@localhost -p 2200

passwd

setear contraseña para el usuario de linux

passwd root

**WINDOWS**

set

Setear una variabla de entorno

set CONTABILIUM_CLIENT_ID={id}

---

*ECHO*

ECHO %CONTABILIUM_CLIENT_ID%

Leer variable de entorno

***telnet***
consultar si un puerto esta siendo usado
telnet 127.0.0.1 5432

---
**DOCKER**

Correr contenedor en local network en el puerto 8080

*docker container run --name react-local -d -it --rm -p 8080:80 react-app*

---
**Remover un paquete instalado por la CLI**
```
You first check out for the name of the package you want to remove:

`dpkg --list`

Then remove the given package

`sudo apt-get remove package_name`

Purge any related code

`sudo apt-get purge package_name`

Then Autoremove

`sudo apt-get autoremove`

Finally, do a clean so you check everything is correctly removed

`sudo apt-get clean`

You would like to check at the packages list whether the one you wanted to remove is not listed anymore, but it is optional.

Have a nice day,
```

---

Saber que distro esta siendo usada

```
cat /etc/os-release
```

```
hostnamectl
```
---

Crear certificados SSL por 3 meses

**Install certbot cli client**

```bash
sudo install certbot python3-certbot-nginx -y
```

**Generar certificado para el dominio**

```bash
sudo certbot --nginx -d <domain-name>
```
