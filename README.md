# Utiliza docker-compose para configurar las IP fijas a los dos contenedores 
**Configuramos las IPs fijas añadiendo la siguiente sección en los contenedores:**

***Contenedor DNS***:

    networks:
      bind9_subnet:
        ipv4_address: 172.28.5.10

***Contenedor Apache***:

    networks:
      bind9_subnet:
        ipv4_address: 172.28.5.15
***Contenedor Cliente***:

    networks:
      bind9_subnet:
        ipv4_address: 172.28.5.12  