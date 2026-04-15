# Evaluacion-1-Gonzalez-Ojeda
Evaluacion 1 de Sistemas Operativos Corporativos 02D

Estudiantes: Sebastian Gonzalez / Benjamin Ojeda

# CREACION MAQUINA LINUX (REDHAT 9)

Nombre de la maquina virtual y Hardware: Tal y como lo indica la evaluacion, se le puso el nombre "Linux SebastianGonzalez_BenjaminOjeda" a la maquina virtual.
Se asignaron 4GB de memoria RAM, 2 CPU y un disco primario de 30GB.

<img width="427" height="472" alt="image" src="https://github.com/user-attachments/assets/3b23ecc1-2de0-479d-b2b8-8fc87803775f" />


Esquema de particiones disco principal: Se pidio una particion de /boot (o /boot/efi) de 1024MiB, una particion de /swap de 2Gib y el resto del disco debia ser de la raiz (/)

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/5026a0f3-5a16-4509-9fff-0df7fa013920" />


Hostname: Se le asigno el nombre "gonzalez-ojeda" por el apellido de ambos estudiantes

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/67d76b3f-384a-431a-8895-89683243abc5" />


Servidor con GUI: Segun los requisitos, se tiene que instalar una maquina server con GUI (Interfaz Grafica).

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/eabd4f3b-13dc-421f-a3b4-2b068faad4ac" />


A continuacion, una vez instalado el sistema operativo se muestra en el lsblk el nuevo disco de 30GB que se solicito para particionar.

<img width="762" height="578" alt="image" src="https://github.com/user-attachments/assets/4f6029e2-93d2-4fec-b9e2-c0ff251138e2" />


Comando lsblk con particiones creadas: Se creo la particion 1 de 6GB en formato ext4 y montada en /gonzalezojeda/nuevo1, la particion 2 de 15GB con etiqueta lvm que no se debia montar, la particion 3 de 6GB en formato xfs y montada en /gonzalezojeda/nuevo2 y la particion 4 con el resto disponible del disco como SWAP

<img width="718" height="373" alt="image" src="https://github.com/user-attachments/assets/80def847-d8f5-4fb2-8506-52cbd3bbf761" />


Comando parted print en /dev/sdb: Aca se pueden ver las particiones solicitadas con un poco mas de detalle.

<img width="679" height="391" alt="image" src="https://github.com/user-attachments/assets/c66c374e-6846-414d-b841-04625af59570" />


Comando cat/etc/fstab: Aca se ven las particiones sdb1, sdb3 y sdb4 agregadas al archivo fstab, la segunda no esta porque no se debia montar.

<img width="1105" height="485" alt="image" src="https://github.com/user-attachments/assets/5424c4de-bebf-412f-863d-2fb12fcbf150" />


Reboot y last login: Se uso el comando reboot para reiniciar la maquina y se uso el comando "last" para ver las sesiones anteriores. 

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/4be1c67c-3f01-40f8-b739-f92a1286f2f9" />

<img width="750" height="594" alt="image" src="https://github.com/user-attachments/assets/41ff33f2-4fbf-49c1-aca4-760018078403" />

lsblk luego del reboot: Aqui se puede apreciar que las particiones siguen montadas luego del reboot. Ademas, la particion Swap ahora sale como [SWAP] en los puntos de montura a comparacion de antes que no salia nada.

<img width="718" height="538" alt="image" src="https://github.com/user-attachments/assets/2ddaf5b2-cb25-4696-bb46-0673bd964efa" />

Con esto, los requisitos de la maquina virtual Linux estan completados.


# CREACION MAQUINA WINDOWS SERVER 2019 (Estandar con GUI)

Nombre de la maquina virtual y Hardware: Segun lo indicado, la maquina debia tener 4GB de ram, 2CPU y un disco de 30GB al igual que la maquina Linux

<img width="489" height="327" alt="image" src="https://github.com/user-attachments/assets/a80d3fa8-c6fc-40de-9682-c8ddeb10dcd6" />

A continuacion, se procede a hacer la instalacion en version Estandar con GUI

<img width="652" height="585" alt="0" src="https://github.com/user-attachments/assets/ea2a08dc-f9b8-4eb5-a8ab-b2c8ea24210d" />

Particiones: Una vez instalada la maquina, se apaga y se le añaden 2 discos SATA de 5GB

<img width="490" height="91" alt="image" src="https://github.com/user-attachments/assets/67f43c0d-e052-46f3-b992-befc9fa71263" />

Se accedio al administrador de discos desde la Administracion de servidor/Administracion de equipos/Administrador de discos.

Una vez aca, ambos discos son formateados con NTFS. Al primer disco se le asigno la letra X: y al segundo disco la letra Y:

<img width="752" height="687" alt="image (2)" src="https://github.com/user-attachments/assets/7d68d3d3-50f1-49c3-8b66-18ca9bfa6283" />

Una vez los discos estan listos, se creo la carpeta "Benjamin-Sebastian" en el disco X: y la carpeta "Ojeda-Gonzalez" en el disco Y:

<img width="1776" height="690" alt="carpeta discos" src="https://github.com/user-attachments/assets/2add5b5c-c3c6-4d93-84ac-f77ddb100fac" />

Con esto ya se cumplen los requisitos dados por la evaluacion.


