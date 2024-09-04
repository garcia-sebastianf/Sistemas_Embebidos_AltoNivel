# Sistemas de Almacenamiento, Sistema Operativo Unix

**1. ¿Qué sistemas de almacenado de datos o “filesystem” existen? NOTA no confundir con el fylesistem de Linux. Liste sólo los más populares mínimo 6. Haga una tabla haciendo una breve descripción por cada uno, describa algunas de sus características e historia i.e. NTFS, FAT, EXT#.**

- **1. NTFS(New Technology File System):** Utilizado principalmente en sistemas operativos Windows. Proporciona características avanzadas como permisos de archivos, compresión y cifrado.

- **2. FAT32(File Allocation Table 32):** Un sistema de archivos más antiguo, ampliamente compatible y utilizado en dispositivos portátiles como unidades USB y tarjetas de memoria. 

- **3. exFAT(Extended File Allocation Table):** Una extensión de FAT que aborda algunas limitaciones de FAT32, como el tamaño máximo de archivo y la capacidad de la unidad. También se usa en dispositivos portátiles y es compatible con Windows y macOS.

- **4. HFS+(Hierarchical File System Plus):** Un Sistema de archivos utilizado en computadoras Mac antes de macOS 10.13 High Sierra. Fue reemplazado por el sistema de archivos APFS. 

- **5. APFS(Apple File System):** Introducido en macOS 10.13 High Sierra, APFS es el sistema de archivos predeterminado para dispositivos Apple. Ofrece beneficios como la instantánea de archivos, cifrado y eficiencia en el uso del espacio. 

- **6. NTFS+:** Variante de NTFS con mejoras en la compatibilidad y características de rendimiento en sistemas macOS a través de software de terceros. 

- **7. F2FS(Flash-Friendly File System):** Un sistema de archivos optimizado para dispositivos de almacenamiento flash, como unidades de estado sólido (SSD) y tarjetas de memoria. Se encuentra comúnmente en sistemas Android.

- **8. ZFS (Zettabyte File System):** Un sistema de archivos avanzado que ofrece capacidades de administración de almacenamiento, protección de datos y administración de volúmenes en una estructura coherente. Se utiliza en sistemas operativos como FreeBSD y Solaris, y también hay implementaciones para Linux. 

- **9. NFS(Network File System):** Utilizado en sistemas operativos Unix y Linux para acceder y compartir archivos en una red. Permite montar sistemas de archivos remotos en sistemas locales. 

- **10. EXT4(Fourth Extended File System):** Un sistema de archivos popular en sistemas Linux. Es una evolución de las versiones anteriores EXT2 y EXT3, con mejoras en la eficiencia y la capacidad para volúmenes más grandes. 

## características e historia de los sistemas de almacenamiento enlistados anteriormente.

**1. NTFS (New Technology File System):**
- Características: NTFS es el sistema de archivos estándar utilizado en sistemas operativos Windows. Ofrece características avanzadas como soporte para permisos de archivos y carpetas, compresión de archivos, cifrado de archivos y carpetas, journaling para recuperación ante fallos y particiones más grandes y eficientes que el sistema FAT. 
- Historia: Fue introducido por primera vez en 1993 con Windows NT. Ha evolucionado con el tiempo, y versiones posteriores han añadido mejoras en términos de seguridad, rendimiento y confiabilidad.
  
**2. FAT32(File Allocation Table 32):**
-	Características: FAT32 es un sistema de archivos simple y ampliamente compatible. Puede manejar particiones de hasta 2 terabytes y archivos de hasta 4 gigabytes. No admite características avanzadas como permisos de archivo y cifrado.
-	Historia: Es una evolución del sistema FAT original (FAT12 y FAT16) y se introdujo para superar algunas de las limitaciones de sus predecesores. Es comúnmente utilizado en dispositivos portátiles y sistemas más antiguos.
  
**3. exFAT (Extended File Allocation Table):**
-	Características: exFAT es una extensión de FAT32 diseñada para abordar limitaciones en el tamaño de archivos y particiones. Es compatible con particiones más grandes y archivos más grandes que FAT32 y es utilizado comúnmente en dispositivos como cámaras digitales y unidades flash USB. 
-	Historia: Fue introducido por Microsoft en 2006 como parte de Windows CE 6.0. Se utiliza ampliamente en dispositivos portátiles debido a su capacidad de manejar archivos grandes.
	
**4. HFS+ (Hierarchical File System Plus):**
-	Características: HFS+ fue el sistema de archivos estándar en Mac OS desde 1998 hasta 2017. Ofrece mejoras en comparación con su predecesor HFS, incluyendo un esquema de nombres Unicode, mayor eficiencia y journaling para recuperación ante fallos.
-	Historia: Fue introducido junto con Mac OS 8.1 en 1998. Aunque ya no es el sistema de archivos predeterminado en macOS, todavía es compatible con versiones anteriores. 

**5.  APFS (Apple File System):**
-	Características: APFS es el sistema de archivos utilizado en macOS desde 2017. Ofrece instantáneas de archivos, soporte para cifrado nativo, gestión de espacio más eficiente y mejor rendimiento en unidades SSD. 
-	Historia. Apple presentó APFS con macOS 10.13 High Sierra. Remplazó gradualmente a HFS+ como sistema de archivos predeterminado en dispositivos Apple.
   
**6. F2FS (Flash-Friendly File System):**
-	Características: F2FS está diseñado específicamente para dispositivos de almacenamiento flash, como SSDs y tarjetas de memoria. Optimiza la asignación de bloques, la recolección de basura y el rendimiento para mejorar la vida útil de los dispositivos flash.
-	Historia: Fue desarrollado por Samsung para dispositivos Android y se ha integrado en el kernel de Linux.

Estos sistemas de archivos han evolucionado con el tiempo para satisfacer las necesidades cambiantes de los sistemas operativos y los dispositivos de almacenamiento. Cada uno tiene sus propias características y ventajas dependiendo de los casos de uso específicos.

## Inicios sistema Linux

2. Abra una consola Linux, si no cuenta con wsl o con un sistema Linux. Para cada uno de los puntos adjunte una captura de pantalla y explique la salida. 
Se opta por la instalación del sistema operativo basado en Linux (Ubuntu) sobre una máquina virtual (Oracle VM VirtualBox) para la realización de algunos puntos.

![image](https://github.com/user-attachments/assets/64a948db-3291-4adf-ac64-63d4b59efe7a)

a. Muestre el nombre de usuario actual. 
 ![image](https://github.com/user-attachments/assets/1f7f8850-5cd9-43a6-ad81-9792b4675499)

	b. Muestre el hostname.
 ![image](https://github.com/user-attachments/assets/1c44e503-6326-4ecf-9326-7877b1379eb8)

	c. Corra #uname -a y explique la salida de este comando. 
El comando uname proporciona información sobre el sistema. Dentro de este comando se encuentran la opción -a, el cual otorga la siguiente información del sistema: Nombre del kernel, nombre del nodo de red (hostame), fecha de lanzamiento del kernel, versión, nombre del hardware de la máquina, Plataforma del hardware y sistema operativo. 
 
![image](https://github.com/user-attachments/assets/85cca4c3-93da-449e-b484-c0a64455840b)


	d. Liste el directorio actual por defecto. 
 ![image](https://github.com/user-attachments/assets/173856be-821b-448d-b4f7-35c7966bc664)

 
e. En ese directorio debería encontrar dos archivos bench y hello.c (este punto lo puede hacer en https://bellard.org/jslinux/)

f. Para correr el script bench.py ejecute lo siguiente: #python bench.py 

![image](https://github.com/user-attachments/assets/7af20682-97c9-4238-ba68-62af4e2596fb)

 
g. Para medir cuanto tiempo tarda en ejecutar bench.py use el comando time y como argumento use la línea del punto anterior. 
![image](https://github.com/user-attachments/assets/77f51e5b-3894-482c-94e6-c57b0869de4c)

 
h. Para compilar el programa hello.c primero debe compilarlo, compílelo así: #gcc -o hello hello.c, Averigüe por su cuenta y explique en detalle cada argumento este comando. lo usaremos más adelante así que busque la ayuda de gcc o pidale a chatgpt que le explique los argumentos.
gcc: Es el compilador de GNU para lenguaje C y otros lenguajes relacionados. Este comando se utiliza para compilar programas escritos en lenguaje C en un ejecutable. 
-o hello: El parámetro ‘-o’ se utiliza para especificar el nombre del archivo de salida (ejecutable). En este caso, se está indicando que el nombre del archivo ejecutable resultante será “hello”.
hello.c: Es el nombre del archivo fuente que contiene el código en lenguaje C que se desea compilar. En este caso, se está asumiendo que existe un archivo llamado “hello.c” en el mismo directorio.
En resumen, el comando “gcc -o hello hello.c” compilará el archivo hello.c utilizando el compilador GCC y generará un archivo ejecutable llamado hello en el mismo directorio. Una vez compilado, podrás ejecutar este archivo para ejecutar el programa resultante. 
Utilizando la ayuda desde consola de comandos:

![image](https://github.com/user-attachments/assets/8e344e20-5486-4a0c-88ba-92fbb9d95383)

 
	i. Ejecute el binario que compiló.

 ![image](https://github.com/user-attachments/assets/dec565da-4640-4f2c-8038-7d25636ba01e)


3. Descargue la versión más reciente de Raspberry Pi OS y póngalo a funcionar en una raspberry pi (1, 2, 3, 4, Zero W)(A,B)(+).

Se realiza el siguiente procedimiento para la instalación y uso de la raspberry pi 3B+

Instalación de la imagen del sistema operativo Raspberry Pi OS with desktop. Se extrae el archivo .zip y se obtiene el archivo .img

![image](https://github.com/user-attachments/assets/be8edbfc-7ffe-4dad-9375-cddcc8ad3aee)

 

Adicionalmente, se realiza la descarga del programa Raspberry pi imager cuya funcionalidad corresponde a grabar imágenes de sistemas operativos en memorias microSD formateándola en caso de presentar archivos almacenados. Además de facilitar la instalación, también permite realizar configuraciones del sistema operativo de forma sencilla, en este caso se realizo la configuración de nombre de usuario y contraseña, así como también se estableció una configuración de red previa al grabado de la imagen en la memoria microSD. 

![image](https://github.com/user-attachments/assets/16408e27-a800-403c-b656-775a963a2217)

 

Durante la instalación, resulta de importancia activar el SSH, esto va a permitir el uso de la tarjeta sin tener acceso a pantallas ni a cables HDMI. 



![image](https://github.com/user-attachments/assets/b3c0aefc-db6f-47a6-86f0-d627bf1abf29)


 

Para el uso y visualización de la interfaz gráfica de la tarjeta, se utilizan VNC Viewer y Putty. 
El segundo programa permite establecer una comunicación cliente-servidor con SSH entre un computador personas y la Raspberry pi 3B+ a partir del host raspberrypi.local y una conexión entre el computador y la tarjeta por medio de un cable de red Rj45.

Finalmente, se visualiza la interfaz gráfica de la tarjeta estableciendo la conexión con el programa VNC Viewer y utilizando el mismo hostname utilizado en el programa Putty para establecer la comunicación con el protocolo SSH. 


 
![image](https://github.com/user-attachments/assets/dbbaab08-2c6e-4a31-b05a-a29df20d9a40)


Es importante resaltar que la conexión entre la raspberry pi 3B+ y el computador personal no requiere necesariamente de un cable rj45 para establecer la conexión. Una segunda opción es obteniendo la dirección ip de la tarjeta y establecer la conexión a partir de dicha dirección directamente con el programa VNC Viewer manteniendo los dos dispositivos conectados a la misma red local. 


4. Use lsblk -f para describir los discos en su raspberry pi, explique cada una de las columnas producidas por este comando para cada fila. 


El comando lsblk se utiliza para obtener información de los dispositivos de bloque disponibles como discos duros, unidades flash, CD-ROM, etc. Con la opción -f se obtiene información adicional como nombres, tamaño, etiquetas de dispositivos, puntos de montaje, tipos de sistemas de archivos en los dispositivos, etc. Se obtuvo el siguiente resultado ejecutando este comando sobre la raspberry pi 3 B+.

 
![image](https://github.com/user-attachments/assets/7310381a-6e74-44cc-95dc-b0538a651d4e)


Mmcblk0: Nombre del dispositivo de almacenamiento (Tarjeta microSD utilizada en la raspberry pi 3).
	
Mmcblk0p1 y mmcblk0p2: Corresponden a las particiones en el dispositivo mmcblk0. La partición mmcblk01 utiliza el sistema de archivos FAT32 (vfat) y contiene los archivos de inicio del sistema (bootfs). La partición mmcblk0p2 utiliza el sistema de archivos ext4 y contiene el sistema de archivos raíz (rootfs) del sistema operativo. 

También se indica el tipo de sistema de archivos utilizado en cada partición FSTYPE. En este caso, la partición mmcblk0p1 utiliza FAT32 (vfat) y la partición mmcblk0p2 utiliza ext4.

LABEL: Es la etiqueta asignada al sistema de archivos. La partición mmcblk0p1 tiene la etiqueta “bootfs” y la partición mmcblk0p2 no tiene una etiqueta específica. 

UUID: Es un identificado único universal asignado a casa sistema de archivos. Proporciona una forma única de identificar el sistema de archivos. En este caso, la partición mmcblk0p2 tiene el UUID “eaaa4faa-eab6-400c-950f-dc96ae4e0400”.

FSAVAIL y FSUSE%: Indican la cantidad de espacio disponible en el sistema de archivos y el porcentaje de uso, respectivamente. 

MOUNTPOINT: Es el punto de montaje de la partición en el sistema de archivos. La partición mmcblk0p1 está montada en /boot y la partición mmcblk0p2 está montada en el directorio raíz (“/”).


5. Averigüe como configurar una IP fija a su raspberry pi con raspbian busque por lo menos dos métodos diferentes. 

En primer lugar, se determina la dirección ip actual de la raspberry, se puede realizar de dos formas: La primera utilizando el comando hostname -I y la segunda forma es con el comando ifconfig.


Utilizando comando hostname -I

 ![image](https://github.com/user-attachments/assets/73001416-05f2-421c-add9-8838c62e76cc)


En caso de obtener dos direcciones ip, la primera corresponderá a la dirección ip asignada a una conexión ethernet, la segunda dirección ip corresponde a la dirección wifi. 








Utilizando el comando ifconfig.

 ![image](https://github.com/user-attachments/assets/f640795f-c485-4146-b054-5bd03f162c0a)


Se utiliza el comando ip r para obtener la dirección ip del router.
 
![image](https://github.com/user-attachments/assets/5e4e3c52-b0d6-4409-bfa2-63676919af86)

Para obtener la dirección del DNS se utiliza el siguiente comando: grep “nameserver” /etc/resolv.conf
Esta dirección puede ser o no la misma dirección que la del router. 

![image](https://github.com/user-attachments/assets/25df314d-d528-4181-b8bb-ae49c133d57f)


Ahora, después de realizados los anteriores pasos, existen dos posibilidades para establecer una dirección ip fija en la tarjeta Raspberry. Puede ser por medio de un menú de opciones del sistema operativo o ya sea modificando el archivo dhcpcd.conf.

Modificando el archivo dhcpcd.conf

Se deben descomentar y modificar las siguientes líneas dentro de este archivo. Esto se realiza con el comando sudo nano /etc/dhcpcd.conf desde el directorio por defecto. 

![image](https://github.com/user-attachments/assets/feb55f2c-c0b8-461b-bf23-41b53a910efd)


Este es el siguiente ejemplo realizado con los datos actuales obtenidos en esta tarjeta.

![image](https://github.com/user-attachments/assets/9726769d-1fe1-4630-bb92-7c93fa0c163c)


Finalmente, se debe oprimir CTRL + O y ENTER para establecer los cambios junto con CTRL + X para salir y reiniciar la máquina con sudo reboot para que se ejecuten los cambios. 

Por medio de opciones del sistema operativo.

Se da click derecho del mouse sobre el símbolo de wifi y se selecciona la opción Wireless & Wired Network Settings.

 
![image](https://github.com/user-attachments/assets/b97ef0db-b51b-427e-a06b-515ed96f3f54)



Se selecciona la opción wlan0 y se escriben los datos obtenidos anteriormente, que son los mismos utilizados al momento de modificar el archivo dhcpcd.conf.

 ![image](https://github.com/user-attachments/assets/d2218f89-76a1-4e3b-8a66-2832cf295dff)

Se da click en aplicar, luego en cerrar y se procede a reiniciar el sistema para aplicar los cambios. 


CONCLUSIONES. 

•	Existen diversos sistemas de almacenamiento de datos desarrollados para distintos sistemas operativos e inclusive para diferentes aplicaciones.  Por ejemplo, pueden ser ya sea en sistemas operativos o en dispositivos portátiles de almacenamiento.

•	Los sistemas de almacenamiento de datos principalmente cumplen la función de organizar y administrar la información almacenada en bloques de memoria, esto es útil para saber en qué parte de la memoria inicia y en qué parte termina un archivo. Sin embargo, con el desarrollo de la tecnología, los servicios ofrecidos por estos sistemas de almacenamiento fueron cada vez mayores y más avanzados, como sistemas de cifrado, compresión y permisos de archivos, instantánea de archivos, mayor eficiencia en el el uso de la memoria, journaling para la recuperación de archivos, entre otros. 

•	El sistema operativo Linux sigue el estándar Unix. Esto significa que muchos comandos van a ser compatibles para diversos sistemas que se rijan con este estándar como Raspberry Pi OS basado en Debian o incluso para derivaciones del sistema operativo de Linux, como Ubuntu. 

•	Es posible tener acceso al sistema operativo de la tarjeta raspberry pi 3 sin necesidad del uso de cables HDMI o pantallas. Ya que basta con buscar la dirección IP de la tarjeta en la red local por medio de algún programa o simplemente establecer una conexión SSH con el uso del Hostname. Después de realizada esta conexión se puede tener acceso a la interfaz gráfica del sistema.

•	La tarjeta raspberry pi 3 utiliza como disco la microSD y crea dos particiones en esta para dos distintas funciones como archivos para el inicio del sistema y datos del sistema. Para cada una de las particiones utiliza diferentes sistemas de almacenamiento. 

•	A pesar de que la tarjeta raspberry pi 3 B+ cuente con un sistema operativo e interfaz gráfica. Todo lo que se puede realizar con el uso del mouse y la interfaz se puede realizar de igual forma con el uso de comandos. Un ejemplo de esto es establecer la dirección ip estática, en el presente trabajo se mostraron dos formas distintas de establecer una dirección ip. A partir de la consola de comando y con el uso de los menús de opciones del sistema operativo. 



