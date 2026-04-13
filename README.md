# Evaluacion-1-Gonzalez-Ojeda
Evaluacion 1

CREACION MAQUINA LINUX (REDHAT 9)

Nombre de la maquina virtual y Hardware: Tal y como lo indica la evaluacion, se le puso el nombre "Linux (Nombre Estudiantes)" a la maquina virtual.
Se asignaron 4GB de memoria RAM, 2 CPU y un disco primario de 30GB.

<img width="729" height="645" alt="image" src="https://github.com/user-attachments/assets/8c4ebfa4-6106-465e-bab4-f2c657ba09a8" />

<img width="749" height="474" alt="image" src="https://github.com/user-attachments/assets/677cbd92-a640-4abc-8f34-283916c72fff" />

Esquema de particiones disco principal: Se pidio una particion de /boot (o /boot/efi) de 1024MiB, una particion de /swap de 2Gib y el resto del disco debia ser de la raiz (/)

<img width="1267" height="883" alt="image" src="https://github.com/user-attachments/assets/0ab8c1fd-18b7-4166-8995-15ae030fa979" />

Hostname: Se le asigno el nombre "gonzalez-ojeda" por el apellido de ambos estudiantes

<img width="1282" height="900" alt="image" src="https://github.com/user-attachments/assets/187c37ed-6ed8-4964-b150-710709b98cf6" />

Creacion nuevo disco 30GB

<img width="1281" height="858" alt="image" src="https://github.com/user-attachments/assets/b84fcd2e-1c69-4e51-82da-80fa29d92f43" />

Comando lsblk con particiones creadas: Se crearon las 4 particiones correspondientes.

<img width="671" height="402" alt="image" src="https://github.com/user-attachments/assets/a801d593-bc89-4042-a193-93d9743d475e" />

Comando parted print en /dev/sdb: Aca se pueden ver las particiones solicitadas con un poco mas de detalle.

<img width="806" height="431" alt="image" src="https://github.com/user-attachments/assets/8702f3b5-a0cd-475c-a647-c8c8837278fc" />

Archivo /etc/fstab visto con "cat": Aca se ven las particiones sdb1, sdb3 y sdb4 agregadas al archivo fstab, la segunda no esta porque no se debia montar.

<img width="1105" height="485" alt="image" src="https://github.com/user-attachments/assets/5424c4de-bebf-412f-863d-2fb12fcbf150" />

Last log, Reboot y lsblk: Aca se siguio la maquina virtual en la casa (por eso la hora). Ademas, para confirmar que la maquina virtual de la casa es completamente igual se adjuntan nuevamente el comando cat, lsblk y parted print.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2eda68eb-5ec8-4dcd-bee3-be998340042e" />

<img width="688" height="224" alt="image" src="https://github.com/user-attachments/assets/a42f9155-65c4-4721-a402-e8aa9ca35621" />

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/c5c57238-6df1-497d-a10a-cbd7868c9e15" />






