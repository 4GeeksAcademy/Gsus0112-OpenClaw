---
name: 4geeks-resumen-progreso
description: Da una visión general de cuánto ha avanzado el estudiante en el curso.
---
# Instrucciones
Cuando el usuario pregunte por su progreso o avance:
1. Recupera el token de los secretos.
2. Haz GET a https://breathecode.herokuapp.com/v1/assignment/user/me/task con header "Authorization: Token <TOKEN>".
3. Calcula estadísticas: total de tareas, completadas (DONE+APPROVED), pendientes (PENDING), rechazadas (REJECTED).
4. Calcula el porcentaje de avance: (completadas / total) * 100.
5. Presenta un resumen claro con el porcentaje y un desglose por tipo de tarea.
