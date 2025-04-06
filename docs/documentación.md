# Configuración del Cliente OpenVPN (Windows)

Este documento describe los archivos necesarios y su propósito en la configuración de un cliente OpenVPN en Windows. También se incluye un ejemplo del archivo de configuración `.ovpn`.

---

## Archivos necesarios

| Archivo              | Descripción |
|----------------------|-------------|
| `cliente1.ovpn`      | Archivo de **configuración principal del cliente OpenVPN**. Define parámetros de conexión como IP del servidor, puerto, certificados, etc. |
| `ca.crt`             | Certificado de la **Autoridad Certificadora (CA)**. Verifica la autenticidad del servidor. |
| `cliente1.crt`       | Certificado del **cliente**. Identifica al cliente como válido en la VPN. Está firmado por la CA. |
| `cliente1.key`       | Clave privada del **cliente**. Se utiliza para autenticación. **Debe mantenerse segura.** |
| `ta.key`             | Clave de **TLS Auth**. Añade una capa de seguridad para proteger contra escaneos y conexiones no autorizadas. Opcional pero muy recomendable. |

> Todos los archivos deben colocarse en la carpeta:
> `C:\Users\Usuario\OpenVPN\config\`

---

## Ejemplo de `cliente1.ovpn`

```ovpn
client
dev tun
proto udp
remote 192.168.1.100 1194
resolv-retry infinite
nobind
persist-key
persist-tun
remote-cert-tls server
cipher AES-256-CBC
auth SHA256
compress lz4
verb 3

ca ca.crt
cert cliente1.crt
key cliente1.key
tls-auth ta.key 1
