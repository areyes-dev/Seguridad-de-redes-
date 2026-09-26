# Seguridad de Redes

## Video demostrativo

[Ver video demostrativo de la práctica](https://youtu.be/CyYBAnvpR9Y)

## Propósito del laboratorio

El propósito de este laboratorio fue diseñar e implementar una infraestructura de red segmentada y protegida en GNS3, utilizando FortiGate como dispositivo principal de seguridad.

La infraestructura fue organizada para separar la red de usuarios, el servidor web y el servidor de base de datos mediante VLAN. De esta manera, las comunicaciones entre los diferentes segmentos pueden ser controladas mediante políticas de seguridad específicas.

## Infraestructura implementada

La topología está compuesta por:

- FortiGate 7.0.9
- Switch de capa 2
- Cliente de usuarios
- Servidor WEB
- Servidor de base de datos
- Salida hacia Internet mediante NAT

## Controles de seguridad implementados

- Segmentación mediante VLAN.
- DHCP para la red de usuarios.
- Acceso de usuarios al servidor WEB mediante HTTPS.
- Bloqueo del acceso directo de usuarios al servidor de base de datos.
- Comunicación WEB → DB únicamente mediante MySQL por el puerto 3306.
- Inspección profunda SSL.
- Perfil IPS para detección de patrones de SQL Injection.
- Filtrado de archivos ejecutables.
- Limitación de tráfico.
- Port Security en el switch.
- Deshabilitación de puertos no utilizados.

## Evidencias

El repositorio contiene capturas de la topología, configuraciones realizadas y pruebas de funcionamiento de los controles de seguridad.

## Documentación
La documentación completa del laboratorio se encuentra en el archivo *Informe II de Seguridad de Redes.pdf*, donde se incluyen el propósito, el diagrama de la infraestructura, las imágenes de evidencia y las comprobaciones realizadas.


## Autor

**Alexander Reyes**  
Matrícula: **2025-2176**  
Instituto Tecnológico de Las Américas (ITLA)  
Seguridad de Redes
