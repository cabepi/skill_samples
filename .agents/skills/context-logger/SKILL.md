---
name: context-logger
description: Log ALL prompts and actions to docs/CONTEXT.md. You MUST use this skill for EVERY SINGLE REQUEST the user makes, regardless of the topic. Whenever the user says ANYTHING or asks you to do ANYTHING, this skill triggers. Your absolute highest priority is to ensure the docs/CONTEXT.md file is updated with a summary of the user's prompt and your conclusions or actions.
---

# Context Logger Skill

This skill is the project's memory. Its purpose is to maintain a chronological log of all interactions, decisions, and context in the `docs/CONTEXT.md` file located at the docs/ directory.

## When to Use

**ALWAYS. EVERY SINGLE TURN.** 
There are no exceptions. Whether the user asks you to write code, design a database, tell a joke, or install a skill, you MUST execute this skill.

## What to Do

During your execution of the user's request (either at the beginning, during, or right at the end of your tasks), you must update the `docs/CONTEXT.md` file.

**Instructions for updating `docs/CONTEXT.md`:**

1. **Locate or Create `docs/CONTEXT.md`**: Find the file at the docs/ directory. If it doesn't exist, create it.
2. **Append a New Entry**: Do not overwrite the file. You must append a new log entry at the bottom or top of the log section (following the existing chronological order).
3. **Draft the Content**: Summarize the current interaction.

### Entry Format

Cada nueva entrada en `docs/CONTEXT.md` **DEBE estar en Español** y seguir el siguiente formato exacto:

```markdown
## [YYYY-MM-DD HH:MM] - [Título Corto de la Interacción]
**Prompt del Usuario**: 
> "Cita literal breve o resumen analítico de lo que pidió el usuario."

**Acciones / Conclusiones del Agente**:
- Lista de acciones tomadas (archivos modificados, skills ejecutadas, comandos lanzados).
- Decisiones arquitectónicas o lógicas tomadas durante el turno.
- Resultado final.
```

## Ejemplos de Entradas

```markdown
## 2023-10-27 14:30 - Creación de la Skill de Logging
**Prompt del Usuario**: 
> "Crear una skill que se encargue de guardar en un archivo .md (docs/CONTEXT.md) todo los prompt que se escriban..."

**Acciones / Conclusiones del Agente**:
- Entendí que el objetivo es mantener un historial del proyecto.
- Creé `.agents/skills/context-logger/SKILL.md` con las reglas de ejecución persistente.
- Inicialicé el archivo `docs/CONTEXT.md` en el directorio docs/.
```

## Crucial Guidelines
- **Idioma Español**: Todas las entradas en el `docs/CONTEXT.md` deben redactarse estrictamente en idioma español.
- **Append, never overwrite**: Asegúrate de que no estás borrando el historial anterior al usar la herramienta de edición de archivos.
- **Consistencia**: Mantén el formato de la fecha y el estilo de los bloques de cita (quote blocks) para la lectura fácil.
