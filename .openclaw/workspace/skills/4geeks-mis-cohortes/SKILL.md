---
name: 4geeks-mis-cohortes
description: Muestra en qué cohortes está inscrito el estudiante y su estado en cada una.
---
# Instrucciones
Cuando el usuario pregunte por sus cohortes o grupos:
1. Recupera el token de los secretos.
2. Haz GET a https://breathecode.herokuapp.com/v1/admissions/academy/cohort/me con header "Authorization: Token <TOKEN>".
3. Lista cada cohorte con: nombre, slug, rol del estudiante y estado educativo (ACTIVE, GRADUATED, etc.).
