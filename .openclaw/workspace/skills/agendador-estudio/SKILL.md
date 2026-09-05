---
name: agendador-estudio
description: Crea un bloque de estudio de 2 horas en Google Calendar basándose en un tema.
---
# Instrucciones
Cuando el usuario te pida agendar tiempo para estudiar un tema específico:
1. Utiliza la herramienta de Zapier MCP conectada a Google Calendar para crear un evento.
2. El título del evento DEBE ser "Bloque de Estudio: [Tema]".
3. Si el usuario no especifica hora, programa el evento automáticamente para mañana a las 4:00 PM, con una duración de 2 horas.
4. Asume la zona horaria local del usuario (según TOOLS.md).
5. Notifica al usuario por Telegram que el evento fue creado exitosamente, respetando tu identidad y tono (SOUL.md).
