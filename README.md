# IdentityServer-API-OAuth2

## Código ejemplo para proteger API con OAuth2 por medio de IdentityServer4 utilizando BD

## Se incluyeron los packages en el proyecto IdentityServer
- IdentityServer4.EntityFramework
- IdentityServer4.EntityFramework.Storage
- Microsoft.EntityFrameworkCore.Design
- Microsoft.EntityFrameworkCore.SqlServer

## Ejecutar
  
```
dotnet restore
dotnet build
```
## Importante
> **Descomentar del archivo Startup.cs del proyecto IdentityServer la línea 53 ( InitializeDatabase(app); ), solo ejecutar la primera vez para cargar info del archivo Config.cs, después comentar de nuevo la línea 53**

> Del archivo Startup.cs del proyecto IdentityServer ajustar cadena de conexión
  
URL para validar Identity Server: `https://localhost:5001/.well-known/openid-configuration`

## La solución cuenta con 3 proyectos:

1. IdentityServer - Para gestión de autenticación
2. API - Sirve info al cliente y está protegida por medio del server de IdentityServer
3. Cliente - Solicita información a la API 
   - Solicita token de acceso a IdentityServer
   - Solicita info a API por medio de el token de acceso
  
**Ejemplo tomado de:** [Protecting an API using Client Credentials](https://identityserver4.readthedocs.io/en/latest/quickstarts/1_client_credentials.html)