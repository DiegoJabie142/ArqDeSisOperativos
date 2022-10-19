# ArqDeSisOperativos

- ¿Qué es un interpretador?

        Es el encargado de traducir código fuente a código máquina.

- ¿Qué es un framework?

        Un framework es un esquema o marco de trabajo que ofrece una estructura 
        base para elaborar un proyecto con objetivos específicos, una especie de plantilla 
        que sirve como punto de partida para la organización y desarrollo de software.

- Enumere, leguajes interpretados que haya visto hasta ahora en la carrera

        Javascript.

- ¿Qué es un compilador?

        Es el encargado de transformar el código fuente de la aplicación en código de máquina
        que le es posible de interpretar por el sistema.

- ¿Qué es virtualizar? 
 
        Es la abstraccion de componentes fisicos en componentes lógicos, se usa para ejecutar 
        varios sistemas operativos y aplicaciones en un solo servidor, por ejemplo.


- ¿Cuál sería el kernel de Windows?

        El kernel de Windows es cerrado.

- ¿Cómo obtengo información del Hardware?

        lscpu ó lshw 

- ¿Cuáles son los elementos fundamentales de un sistema operativo?

        Los elementos fundamentales son: Kernel, terminal, interfaz gráfica, librerías y 
        programas varios.

- ¿Qué es el GPL?

        Es una licencia de software libre y código abierto.

- ¿Cuál es la memoria más cara?

        L3

- ¿Qué tipos de memorias podemos tener en el micro?

        Caché l1, l2 y l3.

- ¿Qué son los archivos compartidos?

        Archivos entre varios ordenadores conectados a una misma red local.

- ¿Qué es un enlace con el comando ln?

        Es la abreviación de un enlace.

- ¿Qué estructura de directorios respeta linux y qué implica ésto?

        Linux respeta la estructura de directorios FHS, ésto implica estandarizar la jerarquía 
        de directorios.

- ¿Cuál es path por excelencia donde se encuentran los archivos de configuración globales de Linux?

        /etc/

- ¿Cuál es el path por excelencia donde se encuentran los logs?

        /$ var/log/

- Se pretende generar un archivo vacío (0 byte). 
- Tílde los comandos correctos (tener en cuenta que se ejecutan desde un usuario sin privilegios de root).

        .touch /tmp/archivo_vacio
        .cat /dev/null > /tmp/archivo_vacio
- ¿Qué es el software libre?

        El software libre es aquel que expone su código y no establece restricciones.
        
- ¿Cuáles son las libertades que establece la  Free Software Foundation o Fundación por el Software Libre?
 
        Libertad de usar el software para cualquier propósito
        Libertad de examinar el código fuente y modificarlo para adecuarse a las necesidades
        Libertad de redistribuir el software
        Libertad de redistribuir el software modificado

- ¿Cuántas particiones primarias puedo tener? *

        1 a 4
- ¿Cuántas particiones Logicas puedo tener?

        Todas las que entren en la particion extendida

- La particion extendida es utilizable para almacenar datos? *
        
        No.

- ¿Qué utilidad tiene particionar disco en lugar de solo crear directorios?

        Facilita el mantenimiento del disco duro, la comprobación de errores o la optimización y desfragmentación de las unidades.
        
---

# Comandos

- Actualizar la base de datos de paquetes.

        apt-get update
- Validar el estado de los paquetes
        
        apt-get check o apt update
- Actualizar paquetes
        
        apt-get upgrade 
- Actualizar la distribución

        apt-get dist-upgrade
- Instalación de un paquete

        apt-get install
                
- Actualizar la distribución.

        apt-get dist-upgrade –y
         
*****COMANDOS INFORMACION DEL SISTEMA*****
*******************************************

- ***arch***                 arquitectura del ordenador
- ***uname -r***             version del kernel
- ***unane -a***             sistema operativo, usuario, kernel
- ***cat /proc/cpuinfo***    informacion sobre la CPU
- ***cat /proc/meminfo***    verifica uso de la memoria RAM
- ***free -m***              muestra el estado y uso de la RAM
- ***cat /proc/net/dev***    adaptadores de red
- ***cat /proc/mounts***     sistema de archivos montado
- ***cat /proc/mounts***     sistema de archivos montado
- ***sudo fdisk -l***        lista los discos y partciones del sistema
- ***lsblk***                lista los discos y particiones del sistema
- ***top -U user***          lista el consumo de ram de los procesos del usuario indicado
- ***du -h directorio***     muestra cuánto ocupa cada archivo dentro de un directorio
- ***du sh***                muestra cuánto espacio ocupa un directorio en total
- ***cat /proc/cpuinfo***    muestra la información del cpu 
- ***sudo mkfs.ext4 /dev/particion*** formatea la partición
- ***sudo mount /dev/particion directorio*** monta la partición en el lugar especificado 
 
******COMANDOS NAVEGACION DEL SISTEMA******
*******************************************

- ***cd /home/usuario***      lleva hasta la ruta indicada, ejemplo usuario
- ***cd..***                  retrocede un nivel de jerarquia de directorios
- ***cd../..***               retrocede dos niveles
- ***cd***                    lleva al directorio raiz
- ***cd ~usuario***           lleva al directorio principal del usuario indicado
- ***cd -***                  lleva al direcotrio anterior
- ***pwd***                   mostrara la ruta del directorio actual
- ***ls***                    muestra los archivos y carpetas
- ***ls -l***                 muestra el detalle de los archivos y carpetas
- ***ls -a***                 muestra los archivos ocultos

******EJEMPLO COMANDO HEAVY******
*******************************************

- ***echo -n "Marca=" > cpu.txt && cat /proc/cpuinfo | grep vendor | uniq | cut -d ":" -f2 >> cpu.txt && echo -n "Modelo de CPU=" >> cpu.txt && cat /proc/cpuinfo | grep model | grep name | uniq | cut -d ":" -f2 >> cpu.txt && echo -n "Frecuencia=" >> cpu.txt && cat /proc/cpuinfo | grep MHz | uniq | cut -d ":" -f2 >> cpu.txt && echo -n "Procesadores=" >> cpu.txt && cat /proc/cpuinfo | grep cores | uniq | cut -d ":" -f2 >> cpu.txt***
        
        Guarda la marca, el modelo del cpu, la frecuencia del cpu y la cantidad de procesadores.
