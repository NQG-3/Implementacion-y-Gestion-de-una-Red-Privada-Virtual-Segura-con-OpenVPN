# Configuración del Cliente OpenVPN (Windows)

Este documento describe los archivos necesarios y su propósito en la configuración de un cliente OpenVPN en Windows.

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

