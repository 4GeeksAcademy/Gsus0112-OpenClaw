---
name: 4geeks-autenticar
description: Verifica que el token de estudiante de 4Geeks sea válido y que la sesión esté activa.
---
# Instrucciones
Cuando el usuario te pida verificar su conexión con 4Geeks:
1. Recupera el token almacenado en los secretos de configuración (variable 4GEEKS_TOKEN o secrets.4geeks_token).
2. Haz una petición GET a https://breathecode.herokuapp.com/v1/admissions/user/me con el header "Authorization: Token <TOKEN>".
3. Si la respuesta es exitosa (200), responde con el nombre del usuario, su email y las academias vinculadas.
4. Si falla (401 o error), informa que el token no es válido o ha expirado.
