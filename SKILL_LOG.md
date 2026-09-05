# 📋 Registro de Skills — Integración 4Geeks API
## Conversación de descubrimiento
**Prompt inicial:** "Quiero darte la habilidad de conectarte a mi cuenta de 4Geeks usando mi token de estudiante, sin que tenga que desarrollar código de mi parte. ¿Qué debemos hacer?"
**Qué sugirió OpenClaw:** Me pidió el token de estudiante y sugirió guardarlo de forma segura en los secretos de configuración. Luego propuso crear skills individuales para cada endpoint de la API de BreatheCode, empezando por la autenticación.
---
## Skill 1: Autenticar
- **Prompt:** "Necesito que puedas verificar si mi token de 4Geeks es válido y decirme quién soy en la plataforma."
- **Qué hace:** Llama a GET /v1/admissions/user/me con el token almacenado y devuelve nombre, email y academias vinculadas.
- **Endpoint:** GET /v1/admissions/user/me
- **Resultado de prueba:** El agente respondió con mi nombre (Jesús), mi email y confirmó que el token es válido y la sesión está activa.
---
## Skill 2: Obtener mis proyectos
- **Prompt:** "Ahora quiero que me digas todos mis proyectos asignados y en qué estado está cada uno."
- **Qué hace:** Llama a GET /v1/assignment/user/me/task?task_type=PROJECT y lista los proyectos agrupados por estado.
- **Endpoint:** GET /v1/assignment/user/me/task?task_type=PROJECT
- **Resultado de prueba:** El agente listó mis proyectos separados por estado (PENDING, DONE, APPROVED, REJECTED) con nombres y fechas.
---
## Skill 3: Trabajo pendiente
- **Prompt:** "¿Qué me falta por entregar? Dime solo lo que tengo pendiente."
- **Qué hace:** Llama a GET /v1/assignment/user/me/task?task_status=PENDING y filtra solo las tareas sin completar.
- **Endpoint:** GET /v1/assignment/user/me/task?task_status=PENDING
- **Resultado de prueba:** El agente mostró las tareas pendientes organizadas por tipo (proyectos, lecciones, ejercicios) con un total al final.
---
## Skill 4: Resumen de progreso
- **Prompt:** "Dame un resumen general de cuánto he avanzado en el curso."
- **Qué hace:** Llama a GET /v1/assignment/user/me/task, calcula estadísticas y muestra un porcentaje de avance.
- **Endpoint:** GET /v1/assignment/user/me/task
- **Resultado de prueba:** El agente calculó mi porcentaje de avance y mostró un desglose: X tareas completadas de Y totales.
---
## Skill 5 (Adicional): Mis cohortes
- **Prompt:** "¿En qué cohortes estoy inscrito y cuál es mi estado en cada una?"
- **Qué hace:** Llama a GET /v1/admissions/academy/cohort/me y lista las cohortes con nombre, rol y estado educativo.
- **Endpoint:** GET /v1/admissions/academy/cohort/me
- **Resultado de prueba:** El agente mostró mi cohorte activa con el nombre del programa y mi estado como ACTIVE.
---
## Skill 6 (Adicional): Próximos eventos
- **Prompt:** "¿Hay algún evento próximo en mi academia?"
- **Qué hace:** Llama a GET /v1/events/all?upcoming=true y lista los eventos futuros con título, fecha y hora.
- **Endpoint:** GET /v1/events/all?upcoming=true
- **Resultado de prueba:** El agente listó los eventos próximos de la academia con sus fechas.
