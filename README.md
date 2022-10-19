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
        que les posible de interpretar por el sistema.

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
        
