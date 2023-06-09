# dockercompose-equipo3

correr el servicio de moodle, configurarlo, crear cursos y usuarios con sus diversos roles especificos

paso 1 - clonar el github para ejecutar el docker-compose.yml

git clone https://github.com/PabloLandaverde/dockercompose-equipo3

![WhatsApp Image 2023-06-09 at 3 48 00 AM](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/d47ec6ec-7478-4085-8c8f-c0fa6a508c01)




paso 2- entrar a la carpeta del directorio clonado

$cd dockercompose-equipo3

paso 3 - correr el docker compose con el siguiente comando:

 $docker compose up

paso 4 - se presentan erroreshay,  que detener los contenedores y configurar con superusuario el grupo y usuario 

$ sudo chgrp docker mariadb_data/

se utiliza para cambiar el grupo propietario de un directorio llamado "mariadb_data" al grupo "docker".

$ sudo chown 1001 mariadb_data/

se utiliza para cambiar el propietario de un directorio llamado "mariadb_data" al usuario con el identificador numérico 1001.

paso 5 - una vez hecha las configuraciones se vuelve a correr el servicio de moodle con el comando:

$ docker compose up

paso 6 - verificar que los contenedores se encuentren corriendo en los puertos correpondientes

$ docker ps

paso 7 - abrir el navegador e ingresar al servicio que esta corriendo de moodle 

$localhost:90



paso 8 - ingresar al sistema de moodle con usuario y contraseña por defecto

-usuario: user

-contraseña: bitnami

