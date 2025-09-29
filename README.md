# Instalación SGE

Para este proyecto tenemos que configurar e instalar WordPress desde Ubuntu Server. Todo esto se hará dentro de una máquina virtual (VM)

## Paso 1:

En este paso tenemos que abrir la terminal de Ubuntu y poner el código "sudo apt update" para asegurarnos de que todo este actualizado.


<img width="920" height="720" alt="Captura desde 2025-09-29 08-54-56" src="https://github.com/user-attachments/assets/104268ca-3a4d-4441-9c37-34c5fb19fa5e" />


En la imagen se puede ver que faltan algunas actualizaciones, pero no son necesarias para este proceso.


Ya que tenemos ese primer paso hehco, hay que instalar las aplicaciones requeridas por WordPress:


<img width="500" height="424" alt="Captura desde 2025-09-29 09-48-04" src="https://github.com/user-attachments/assets/9eb74208-a2b3-4356-9320-c99a73bc5bb9" />


## Paso 2:
En este paso creamos una carpeta con "sudo mkdir", además, esta misma carpeta tendrá permisos de superusuario (root).


Después, con "sudo chown", haremos que la carpeta cambie de propietario.


Por último, cambiamos la ubicación de la carpeta para que esté dentro de un servidor, "curl", y, con "-u", le damos unas credenciales para que llegue óptimamente al servidor.


<img width="800" height="179" alt="Captura desde 2025-09-29 09-55-19" src="https://github.com/user-attachments/assets/3c65494d-ecdd-4568-bbd4-22dab34b6d8c" />
