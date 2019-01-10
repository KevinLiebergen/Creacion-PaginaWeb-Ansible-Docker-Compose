# Creación página web con wordpress conectado a una base de datos 

Página web montada con Wordpress 4.7.2-apache sobre base de datos mariadb 10.0.29

Instalación de servidor web sobre maquina virtual Ubuntu 18.04 Bionic


## Requisitos

- Máquina virtual Ubuntu 18.04 Bionic con openssh-server instalado
- Descarga e instalación de ansible
- Configuración sobre la dirección de maquinas virtuales a actuar ansible en /etc/ansible/hosts

## Descarga 

$ git clone https://github.com/KevinLiebergen/Creacion-PaginaWeb-Ansible-Docker-Compose.git

## Instalación

### Iniciar aplicación
$ cd Creacion-PaginaWeb-Ansible-Docker-Compose

-  Modificar por sus rutas absolutas en las 2 últimas tareas de webserver.yml donde se tenga el fichero docker-compose.yml

$ ansible-playbook webserver.yml -K

### Parar aplicación

-  Cambiar la ruta hacia donde tenga su fichero docker-compose.yml

$ ansible-playbook pararWebserver.yml -K
