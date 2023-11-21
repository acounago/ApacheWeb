# Utiliza docker-compose para configurar las IP fijas a los dos contenedores 
**Configuramos las IPs fijas añadiendo la siguiente sección en los contenedores:**

***Contenedor DNS***:

  ![ IP fija DNS ](./img/ipfijaDNS.png)

***Contenedor Apache***:

![ IP fija DNS ](./img/IPfijaapache.png)

***Contenedor Cliente***:

![ IP fija DNS ](./img/ipcliente.png) 

# Añadimos dos zonas al DNS
1. www.fabulasmaravillosas.int
2. www.fabulasoscuras.com

***Primera Zona***:

![ Primera Zona ](./img/zona1.png) 

***Comprobación con el "dig"***

![  Comprobación con dig ](./img/digzona1.png) 

***Segunda Zona***:

![ Segunda Zona ](./img/zona2.png) 

  ***Comprobación con el "dig"***

![  Comprobación con dig ](./img/digzona2.png) 

# Utilización de la directiva "DirectoryIndex"

*Esta directiva se utiliza en servidores web para especificar el nombre de los archivos que se deben buscar y mostrar cuando un cliente solicita acceder a un directorio en lugar de un archivo específico.*

![ DirectoryIndex ](./img/indexdirectory.png) 

*En este ejemplo, se le está diciendo al servidor web Apache que, al acceder a un directorio, primero busque un archivo llamado "index.html" y, si no lo encuentra, busque un archivo llamado "hola.html". Si ninguno de estos archivos está presente, el servidor podría mostrar una lista de archivos en el directorio o devolver un error, dependiendo de la configuración adicional.*
