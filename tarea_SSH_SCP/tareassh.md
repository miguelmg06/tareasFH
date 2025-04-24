# Práctica SSH

## Configuración Inicial

1. Configuramos los puertos de red de nuestras dos máquinas virtuales:
   - Máquina A: puerto 2222
   - Máquina B: puerto 2223

  ![cap1](imagenes/f1.png)
  ![cap2](imagenes/f2.png)

2. Nos conectamos por el **SSH** a las dos máquinas.

  ![cap3](imagenes/f3.png)
  ![cap4](imagenes/f4.png)

## Creamos los usuarios

- En la máquina **A**, creamos el usuario `Alez`.

  ![cap5](imagenes/f5.png)

- En la máquina **B**, creamos el usuario `Brais`.

  ![cap6](imagenes/f6.png)

## Conexión SSH entre Máquinas

- Desde la máquina **A**, realizamos una conexión SSH hacia la máquina **B**.

  ![cap7](imagenes/f7.png)

- Al conectarnos, se genera un archivo `known_hosts` en `~/.ssh/` que guarda la huella digital del servidor B.

  ## Transferencia de Archivos

  1. En la máquina **A**, creamos el directorio `prueba` con el archivo `prueba.txt` en la ruta temporal y enviamos la información a la máquina B.

  ![cap8](imagenes/f8.png)

  2. En la máquina **B**, creamos el directorio `prueba2` con el archivo `prueba2.txt` en su ruta temporal y lo enviamos a la A. (antes de ese comando ejecutaremos este: mkdir /tmp/prueba2)

  ![cap9](imagenes/f9.png)

  3. Pasaremos los directorios `prueba` y `prueba2` al ordenador anfitrión. Ejecutamos los comandos necesarios desde la máquina anfitrión.(la ruta es C:\Users\ASIR115\Desktop\ q sale cortada q no me di cuenta)

  ![cap10](imagenes/f10.png)
  ![cap11](imagenes/f11.png)
  ![cap12](imagenes/f12.png)

  4. Creamos el directorio `prueba3` en el servidor con **200 archivos .txt** y lo transmitimos al escritorio del anfitrión.

  ![cap13](imagenes/f13.png)
  
  (en esta imagen el comando es acp -p 2222 -r Alex@localhost:/tmp/prueba3 ∼ "C:\Users\ASIR115\Desktop\")
  ![cap14](imagenes/f14.png)
  ![cap15](imagenes/f15.png)

  ## Conexión SSH con clave y passphrase

1. Generamos un par de claves en el cliente.
2. Establecemos la conexión con el servidor.
3. Creamos la frase de paso (*passphrase*) con el valor `servidorssh`.
4. Nos conectamos desde el usuario **Alex** al usuario **Brais** utilizando la clave correspondiente a `servidorssh`.

![cap16](imagenes/f16.png)
![cap17](imagenes/f17.png)
![cap18](imagenes/f18.png)
