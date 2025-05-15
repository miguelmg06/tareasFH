# Montado de un sistema de ficheros con Chroot
## 1.	Realiza una instalación desde cero de una máquina virtual con sistema operativo debian y en ella tiene que existir un usuario cuyo nombre sea tu nombre personal.

![practica2](imagenes/i1.png)

![practica2](imagenes/i2.png)

![practica2](imagenes/i3.png)

![practica2](imagenes/i4.png)

![practica2](imagenes/i5.png)

![practica2](imagenes/i6.png)

![practica2](imagenes/i7.png)

![practica2](imagenes/i8.png)

![practica2](imagenes/i9.png)

## 2. Ahora empezamos a montar el kali sobre el debian

![practica2](imagenes/i10.png)

![practica2](imagenes/i11.png)

## 2. Empezamos con la terminal

a. Cambiar a castellano el teclado

![practica2](imagenes/i12.png)

b. Iniciamos sesión como root con "sudo su" y confirmamos en /dev que este el sda1

![practica2](imagenes/i13.png)

![practica2](imagenes/i14.png)

c. Usaremos el "chroot" para modificar el live de Kali y entramos en Debian

![practica2](imagenes/i15.png)

d. Montamos el disco /dev/sda1 en /mnt/recuperar

![practica2](imagenes/i16.png)

![practica2](imagenes/i17.png)

![practica2](imagenes/i18.png)

# Verificación
## 1. Generamos un archivo de prueba dentro del entorno Debian montado y posteriormente accedimos a Debian para verificar que se hubiera creado correctamente.

a. El archivo creado estara en la ruta "/home/miguel/pruebla.txt"

![practica2](imagenes/i19.png)

![practica2](imagenes/i20.png)

