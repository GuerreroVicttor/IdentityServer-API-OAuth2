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
  3.1 Solicita token de acceso a IdentityServer
  4.1 Solicita indo a API por medio de el token de acceso
  
**Ejemplo tomado de:**

[Protecting an API using Client Credentials](https://identityserver4.readthedocs.io/en/latest/quickstarts/1_client_credentials.html)
