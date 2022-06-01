# IdentityServer-API-OAuth2

## Código ejemplo para proteger API con OAuth2 por medio de IdentityServer4

## Ejecutar
  
```
dotnet restore
dotnet build
```
  
## La solución cuenta con 3 proyectos:

1. IdentityServer - Para gestión de autenticación
2. API - Sirve info al cliente y está protegida por medio del server de IdentityServer
3. Cliente - Solicita información a la API 
   - Solicita token de acceso a IdentityServer
   - Solicita info a API por medio de el token de acceso
  
**Ejemplo tomado de:** [Protecting an API using Client Credentials](https://identityserver4.readthedocs.io/en/latest/quickstarts/1_client_credentials.html)
