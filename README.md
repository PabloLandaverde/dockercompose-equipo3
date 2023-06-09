# dockercompose-equipo3

correr el servicio de moodle, configurarlo, crear cursos y usuarios con sus diversos roles especificos

paso 1 - clonar el github para ejecutar el docker-compose.yml

git clone https://github.com/PabloLandaverde/dockercompose-equipo3

![WhatsApp Image 2023-06-09 at 3 48 00 AM](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/d47ec6ec-7478-4085-8c8f-c0fa6a508c01)




paso 2- entrar a la carpeta del directorio clonado

$cd dockercompose-equipo3

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/b0fed263-b184-4029-ba01-cf8d223e616f)


paso 3 - correr el docker compose con el siguiente comando:

 $docker compose up
 
 ![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/ec2dd929-db30-4f66-b81b-47483896b89d)


paso 4 - se presentan errores y hay que detener los contenedores y configurar con superusuario el grupo y usuario 

$docker compose stop

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/608fbd80-0a6b-4af6-a392-71766bcf43ec)


$ sudo chgrp docker mariadb_data/

se utiliza para cambiar el grupo propietario de un directorio llamado "mariadb_data" al grupo "docker".


$ sudo chown 1001 mariadb_data/

se utiliza para cambiar el propietario de un directorio llamado "mariadb_data" al usuario con el identificador numérico 1001.


![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/e310b85b-74f9-4708-b2a1-914cd756aa9e)



paso 5 - una vez hecha las configuraciones se vuelve a correr el servicio de moodle con el comando:

$ docker compose up

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/9738f894-1229-483b-b200-cfc3ea4d1163)


paso 6 - verificar que los contenedores se encuentren corriendo en los puertos correpondientes

$ docker ps

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/385930dc-b3ca-4220-8e5a-c1eeb819a3d4)


paso 7 - abrir el navegador e ingresar al servicio que esta corriendo de moodle 

$localhost:90

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/9251bb6b-db3d-492d-9804-11a7709b6ab7)



paso 8 - ingresar al sistema de moodle con usuario y contraseña por defecto

-usuario: user

-contraseña: bitnami


![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/43fabb02-2038-4ea0-ad37-ad7f162fa8d2)


![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/20dd959e-6ec4-4c1b-9644-23ec923af3d2)



paso 9 - configurar el administrador 


![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/82248fc8-5ebe-4eed-8b54-f43d2c2e49d6)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/f00f15f6-704f-4e2f-af35-8088ab07cec7)




paso 10 - crear curso 

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/4103470c-36aa-4f67-b59a-d1de13e0985b)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/9e67bc8a-d23c-46ee-80d5-e127a5dfcb02)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/89cfe24f-1f79-4109-8bd3-10c448db3618)


paso 11 - crear usuarios 

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/631d7fb5-a77d-4b2e-bffd-8dce84741020)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/c605c946-dba2-41ad-9f62-a5416f8d3bb9)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/db0c449e-da41-473b-9ed2-cf39f736c7d0)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/fd68b6d9-c974-496c-b200-d5c8aa1dc314)



paso 12 - listar los usuarios 


![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/2423695f-7678-41f8-995e-a92fd5461199)


paso 13 - agregar usuarios al curso y asignarles su rol

![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/8dae60c9-bc76-418f-a5b3-cff57246ddb8)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/ffa07317-682f-412a-94df-bf230066243e)



![image](https://github.com/PabloLandaverde/dockercompose-equipo3/assets/115749532/a572c756-90ca-4099-b572-68b1702b73bc)






