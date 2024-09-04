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

