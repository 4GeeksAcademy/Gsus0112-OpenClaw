---
name: 4geeks-mis-proyectos
description: Recupera la lista de proyectos asignados al estudiante con su estado actual.
---
# Instrucciones
Cuando el usuario pregunte por sus proyectos:
1. Recupera el token de los secretos.
2. Haz GET a https://breathecode.herokuapp.com/v1/assignment/user/me/task?task_type=PROJECT con header "Authorization: Token <TOKEN>".
3. Lista cada proyecto mostrando: nombre, estado (PENDING, DONE, APPROVED, REJECTED) y fecha.
4. Agrupa por estado para que sea fácil de leer.
