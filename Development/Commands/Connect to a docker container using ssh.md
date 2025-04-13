- Run a docker container

```bash
docker container run -it -d --rm --name prueba-ssh -p 2200:22 ubuntu:20.04
```

- Access the container

```bash
docker exec -it prueba-ssh "/bin/bash"
```

 - install dependencies and install ssh

```bash
apt update
apt install openssh-server vim -y
```

 - Create a new user
```bash
useradd -m ubuntu
```

- Define new user password
```bash
passwd ubuntu
type password:
retype password:
```

 - On the host machine create a ssh key

```bash
ssh-keygen -t rsa -b 4096 -C "Comentario"
```

This key is going to be stored in *~/.ssh/id_rsa*

 - Copy the key from the host machine to the container

```bash
ssh-copy-id -p 2200 <user-name>@localhost

enter host password:
```

- Use ssh to log into the container
```bash
ssh -p 2200 ubuntu@localhost
```

- Install python if necessary
```bash
apt install python3 python3-pip -y
```
