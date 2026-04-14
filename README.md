# Evaluacion-1-Gonzalez-Ojeda
Evaluacion 1

Estudiantes: Sebastian Gonzalez / Benjamin Ojeda

# CREACION MAQUINA LINUX (REDHAT 9)

Nombre de la maquina virtual y Hardware: Tal y como lo indica la evaluacion, se le puso el nombre "Linux (Nombre Estudiantes)" a la maquina virtual.
Se asignaron 4GB de memoria RAM, 2 CPU y un disco primario de 30GB.

<img width="729" height="645" alt="image" src="https://github.com/user-attachments/assets/8c4ebfa4-6106-465e-bab4-f2c657ba09a8" />

<img width="749" height="474" alt="image" src="https://github.com/user-attachments/assets/677cbd92-a640-4abc-8f34-283916c72fff" />


Esquema de particiones disco principal: Se pidio una particion de /boot (o /boot/efi) de 1024MiB, una particion de /swap de 2Gib y el resto del disco debia ser de la raiz (/)

<img width="1267" height="883" alt="image" src="https://github.com/user-attachments/assets/0ab8c1fd-18b7-4166-8995-15ae030fa979" />


Hostname: Se le asigno el nombre "gonzalez-ojeda" por el apellido de ambos estudiantes

<img width="1282" height="900" alt="image" src="https://github.com/user-attachments/assets/187c37ed-6ed8-4964-b150-710709b98cf6" />

A continuacion se muestra en el lsblk el nuevo disco de 30GB que se solicito para particionar.

<img width="1281" height="858" alt="image" src="https://github.com/user-attachments/assets/b84fcd2e-1c69-4e51-82da-80fa29d92f43" />


Comando lsblk con particiones creadas: Se crearon las 4 particiones correspondientes.

<img width="671" height="402" alt="image" src="https://github.com/user-attachments/assets/a801d593-bc89-4042-a193-93d9743d475e" />


Comando parted print en /dev/sdb: Aca se pueden ver las particiones solicitadas con un poco mas de detalle.

<img width="806" height="431" alt="image" src="https://github.com/user-attachments/assets/8702f3b5-a0cd-475c-a647-c8c8837278fc" />


Archivo /etc/fstab visto con "cat": Aca se ven las particiones sdb1, sdb3 y sdb4 agregadas al archivo fstab, la segunda no esta porque no se debia montar.

<img width="1105" height="485" alt="image" src="https://github.com/user-attachments/assets/5424c4de-bebf-412f-863d-2fb12fcbf150" />


Reboot, last log y lsblk: Aca se siguio la maquina virtual en la casa (por eso la hora). Ademas, para confirmar que la maquina virtual de la casa es completamente igual se adjuntan nuevamente el comando cat, lsblk y parted print.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2eda68eb-5ec8-4dcd-bee3-be998340042e" />


En la siguiente imagen se ve la ultima sesion antes del reboot. (al final sale que la sesion anterior empezo a las 14 horas porque intentamos cambiar la hora para que se mantenga uniforme con las demas capturas, pero preferimos la honestidad antes que la inconsistencia).

<img width="688" height="224" alt="image" src="https://github.com/user-attachments/assets/a42f9155-65c4-4721-a402-e8aa9ca35621" />

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/c5c57238-6df1-497d-a10a-cbd7868c9e15" />


Algo importante a destacar luego de hacer la particion SWAP es que antes no salia como tal en el comando lsblk, pero despues del reboot su punto de montura ahora si aparece como [SWAP]

Con el reboot, se confirma que los discos estan montados correctamente y que los pasos de la maquina virtual Linux estan completados.


# CREACION MAQUINA WINDOWS SERVER 2019 (Estandar con GUI)

Nombre de la maquina virtual y Hardware: Segun lo indicado, la maquina debia tener 4GB de ram, 2CPU y un disco de 30GB al igual que la maquina Linux

<img width="489" height="327" alt="image" src="https://github.com/user-attachments/assets/a80d3fa8-c6fc-40de-9682-c8ddeb10dcd6" />

A continuacion, se procede a hacer la instalacion en version Estandar con GUI

<img width="652" height="585" alt="0" src="https://github.com/user-attachments/assets/ea2a08dc-f9b8-4eb5-a8ab-b2c8ea24210d" />

Particiones: Una vez instalada la maquina, se apaga y se le añaden 2 discos SATA de 5GB

<img width="490" height="91" alt="image" src="https://github.com/user-attachments/assets/67f43c0d-e052-46f3-b992-befc9fa71263" />

Ambos discos son formateados con NTFS. Al primer disco se le asigno la letra X: y al segundo disco la letra Y:

<img width="752" height="687" alt="image (2)" src="https://github.com/user-attachments/assets/7d68d3d3-50f1-49c3-8b66-18ca9bfa6283" />

Una vez los discos estan listos, se creo la carpeta "Benjamin-Sebastian" en el disco X: y la carpeta "Ojeda-Gonzalez" en el disco Y:

<img width="1776" height="690" alt="carpeta discos" src="https://github.com/user-attachments/assets/2add5b5c-c3c6-4d93-84ac-f77ddb100fac" />

Con esto ya se cumplen los requisitos dados por la evaluacion.


