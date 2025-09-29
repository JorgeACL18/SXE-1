# Instalación SGE

Para este proyecto tenemos que configurar e instalar WordPress desde Ubuntu Server. Todo esto se hará dentro de una máquina virtual (VM)

## Paso 1:

En este paso tenemos que abrir la terminal de Ubuntu y poner el código "sudo apt update" para asegurarnos de que todo este actualizado.


<img width="800" height="720" alt="Captura desde 2025-09-29 08-54-56" src="https://github.com/user-attachments/assets/104268ca-3a4d-4441-9c37-34c5fb19fa5e" />


En la imagen se puede ver que faltan algunas actualizaciones, pero no son necesarias para este proceso.


Ya que tenemos ese primer paso hehco, hay que instalar las aplicaciones requeridas por WordPress:


<img width="800" height="424" alt="Captura desde 2025-09-29 09-48-04" src="https://github.com/user-attachments/assets/9eb74208-a2b3-4356-9320-c99a73bc5bb9" />


## Paso 2:
En este paso creamos una carpeta con "sudo mkdir", además, esta misma carpeta tendrá permisos de superusuario (root).


Después, con "sudo chown", haremos que la carpeta cambie de propietario.


Por último, cambiamos la ubicación de la carpeta para que esté dentro de un servidor, "curl", y, con "-u", le damos unas credenciales para que llegue óptimamente al servidor.


<img width="800" height="179" alt="Captura desde 2025-09-29 09-55-19" src="https://github.com/user-attachments/assets/3c65494d-ecdd-4568-bbd4-22dab34b6d8c" />


## Paso 3:
Ahora tenemos que utilizar el código "sudo nano /etc/apache2/sites-available/wordpress.conf" para poder editar el archivo desde la misma consola. Al ejecutarlo nos llevará a una pantalla donde tendremos que poner el código que se menciona más adelante.

<img width="800" height="41" alt="Captura de pantalla 2025-09-29 173910" src="https://github.com/user-attachments/assets/341d8fbe-96e1-4806-9dca-fdea4f818acc" />


Una vez dentro, tendremos que introducir el siguiente código (ver imagen). Esto configura Apache para servir el sitio WordPress.


<img width="800" height="786" alt="Captura desde 2025-09-29 09-01-18" src="https://github.com/user-attachments/assets/7e09fbc0-15f4-49cd-9772-55db3b03735e" />


Al terminar de introducir el código, se presiona **Ctl+X** para salir y guardarlo. Otra vez en la terminal hay que introducir los siguientes códigos que permitirán el acceso al sitio de WordPress:


<img width="800" height="292" alt="Captura desde 2025-09-29 09-02-59" src="https://github.com/user-attachments/assets/232ba7aa-274c-4dfe-a8f8-a9266145b2f8" />


## Paso 4:
Para este paso tendremos que acceder a la raíz de MySQL para crear una base de datos para dar los permisos a WordPress:


<img width="942" height="523" alt="Captura desde 2025-09-29 09-06-01" src="https://github.com/user-attachments/assets/81f21a9a-19f6-4d23-a03f-e33ea8933096" />


## Paso 5:
Ahora con el comando "sudo -u www-data cp /srv/www/wordpress/wp-config-sample.php /srv/www/wordpress/wp-config.php" podemos crear el archivo de configuración de WordPress y, con los otros comandos, seremos capaces de darle las credenciales que necesita.


<img width="1400" height="80" alt="Captura desde 2025-09-29 09-07-24" src="https://github.com/user-attachments/assets/76c07232-22cb-4d17-94db-e359218cc300" />

Ahora, hay que configurar la dirección del mismo con el código "sudo -u www-data nano /srv/www/wordpress/wp-config.php". Para esto, utilizaremos una página de WordPress que facilita unos códigos generadors aleatoriamente para hacer que nuestro sitio sea más seguro.


<img width="800" height="1048" alt="Captura desde 2025-09-29 09-07-55" src="https://github.com/user-attachments/assets/c34eef88-57c2-4092-bc36-3bbdeb806db0" /> <img width="800" height="928" alt="Captura desde 2025-09-29 09-10-02" src="https://github.com/user-attachments/assets/450ccd00-2b62-4c9e-a465-c929758d2412" />


## Último paso:
Con todo lo anterior ya configurado. Podremos abrir la página http://localhost/ y desde ahí ya podemos poner todas las credenciales, como correo electrónico, nombre de la página, contraseña de la cuenta, entre otros, y ya tendríamos nuestro WordPress configurado.


<img width="800" height="890" alt="Captura desde 2025-09-29 09-11-43" src="https://github.com/user-attachments/assets/737abe4b-a924-45c6-aee4-379f0f6d82d5" />


En esta pantalla se nos da la opción de elegir el idioma que queramos.


<img width="800" height="976" alt="Captura desde 2025-09-29 09-12-43" src="https://github.com/user-attachments/assets/8853ba6b-2406-47d1-bf9c-48f47e1f0bb8" />


Y aquí es donde introduciríamos nuestras credenciales.

# FIN









