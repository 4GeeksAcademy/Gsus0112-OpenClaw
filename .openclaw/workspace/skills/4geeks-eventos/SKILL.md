---
name: 4geeks-eventos
description: Muestra los próximos eventos disponibles en la academia del estudiante.
---
# Instrucciones
Cuando el usuario pregunte por eventos o actividades próximas:
1. Recupera el token de los secretos.
2. Haz GET a https://breathecode.herokuapp.com/v1/events/all?upcoming=true con header "Authorization: Token <TOKEN>".
3. Lista los eventos próximos mostrando: título, fecha, hora y descripción breve.
4. Si no hay eventos próximos, informa que no hay eventos programados por ahora.
