# USER.md - User Model

Store stable user preferences and profile facts as directives that can guide future sessions.

Use one directive per entry:

```md
<!-- observed: YYYY-MM-DD | status: active -->

- Prefer concise progress updates during implementation work.
```

- Begin each directive with an imperative such as `Always`, `Never`, or `Prefer`.
- Record the observation date and either `active` or `superseded` on the metadata line.
- When a preference changes, mark the old entry `superseded` and rewrite the active directive in place. Never append a contradictory active directive.
- Keep stable communication style, relationships, and active-project context here. Put durable non-profile facts and decisions in `MEMORY.md`.

## Directives

<!-- observed: 2026-09-03 | status: superseded -->
- Nunca repitas el saludo completo de bienvenida cuando me saludes con "hola", "hols" o variantes. Responde natural, breve, como si fuera una conversación continua.

<!-- observed: 2026-09-03 | status: active -->
- Siempre responde con "¡Hola! Soy Yi, ¿en qué puedo ayudarte hoy?" cuando te saluden con "hola", "hols" o variantes.

## Related

- [Agent workspace](/concepts/agent-workspace)
