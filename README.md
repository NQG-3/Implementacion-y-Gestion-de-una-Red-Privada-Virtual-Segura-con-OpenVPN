# Proyecto VPN con Raspberry Pi 4, Router y Aplicación Web

## Introducción

Este proyecto tiene como objetivo implementar y configurar una red privada virtual (VPN) utilizando **OpenVPN** en una **Raspberry Pi 4**, conectada a un **router doméstico configurado para crear una red local**. Además, se desarrollará una **aplicación web** que permitirá a los usuarios autenticarse y conectarse fácilmente a la VPN desde una interfaz gráfica accesible. Esta solución facilitará el acceso remoto seguro a los recursos internos de la red local, protegiendo la transmisión de datos mediante cifrado robusto.

## Finalidad

La finalidad del proyecto es ofrecer una solución integral de acceso remoto seguro mediante VPN, orientada a usuarios particulares, pequeñas empresas o entornos educativos. Se busca garantizar la **confidencialidad, integridad y disponibilidad** de la información, permitiendo que los usuarios se conecten desde ubicaciones remotas a una red local gestionada por un router, utilizando una Raspberry Pi como servidor VPN.  
La **aplicación web** facilitará la conexión al sistema, simplificando el proceso de autenticación y conexión para los usuarios, sin necesidad de realizar configuraciones técnicas complejas en los dispositivos cliente.

## Objetivos

- Implementar una VPN segura y estable con OpenVPN sobre una Raspberry Pi 4.
- Configurar un router doméstico para crear una red local protegida a la que se accederá desde el exterior.
- Desarrollar una aplicación web que permita a los usuarios autenticarse y conectarse a la VPN de forma sencilla, integrando funciones de gestión de usuarios.
- Establecer medidas de seguridad avanzadas, como el uso de certificados, autenticación TLS y 2FA.
- Automatizar la gestión de conexiones y usuarios a través de scripts.
- Monitorizar el rendimiento y la seguridad de la red VPN con herramientas como Nagios o Zabbix.
- Evaluar el rendimiento del sistema, especialmente en cuanto a velocidad, estabilidad y latencia.
- Documentar todo el proceso de desarrollo e implementación, incluyendo pruebas y resultados.

## Medios necesarios

### Hardware

- Una **Raspberry Pi 4** con sistema operativo Linux (Raspberry Pi OS).
- Un **router configurable** que permita crear la red local y redireccionar puertos.
- Ordenadores de prueba con Windows.
- Acceso a Internet estable para pruebas remotas.

### Software

- **OpenVPN** (última versión).
- **Servidor web** (como Apache o Nginx) y backend para la aplicación web (por ejemplo, Flask, Node.js o Django).
- Herramientas de monitoreo como **Nagios** o **Zabbix**.
- Frameworks de desarrollo web (HTML, CSS, JavaScript, y/o frameworks como React o Vue.js).
- Sistemas operativos de prueba (Windows, Linux).

## Planificación

| Actividad                                                                 | Duración estimada |
|--------------------------------------------------------------------------|-------------------|
| Instalación y configuración de OpenVPN en la Raspberry Pi               | 3 horas           |
| Configuración del router para redirección de puertos y red local        | 1 hora            |
| Desarrollo e implementación de la aplicación web para conexión a la VPN | 8 horas           |
| Creación de clientes VPN en ordenadores de prueba                       | 2 horas           |
| Implementación de cifrado, certificados, TLS y 2FA                      | 2 horas           |
| Configuración de reglas de firewall y NAT en la Raspberry Pi           | 3 horas           |
| Implementación de sistema de failover o redundancia                     | 4 horas           |
| Pruebas de rendimiento de la VPN (latencia y velocidad)                 | 3 horas           |
| Configuración de herramientas de monitoreo y gestión de red             | 3 horas           |
| Optimización con split tunneling                                        | 3 horas           |
| Pruebas de seguridad (penetración, vulnerabilidades)                    | 5 horas           |
| Implementación de control de acceso por roles y usuarios                | 5 horas           |
| Generación de informes automáticos sobre la actividad de la VPN        | 4 horas           |
| Automatización para la gestión de usuarios y conexiones                 | 5 horas           |
| Documentación del proceso y resultados                                  | 6 horas           |
| Pruebas finales de conectividad y seguridad                             | 5 horas           |
| Prueba de todo el proyecto en condiciones reales                        | 6 horas           |

**Total estimado de horas: 68 horas**

