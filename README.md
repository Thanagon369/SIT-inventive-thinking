# SIT Inventive Thinking (Skill)

A reusable skill that guides an AI assistant through **Systematic Inventive Thinking (SIT)**: generate structured, non-obvious ideas by modifying what already exists with five operations - Subtraction, Division, Task Unification, Multiplication and Attribute Dependency - inside a "Closed World".

> Pensamiento Inventivo Sistemático (SIT): una skill que guía al asistente para generar ideas a partir de lo que ya existe, usando cinco operaciones dentro de un "mundo cerrado". Funciona en español e inglés: responde en el idioma del usuario.

## What it does
1. Frames the system and the Closed World.
2. Inventories components and attributes.
3. Applies the five SIT tools.
4. Finds a beneficiary for each variant (Function Follows Form).
5. Filters out ideas that break the rules or are obvious.
6. Returns a table plus a short ranked shortlist.

## Install
This repository is a single skill folder whose entry point is `SKILL.md` (YAML frontmatter with `name` and `description`, followed by instructions). Copy the folder to the skills location used by your Claude environment, or upload it where your product accepts skills. Check the current official documentation for exact steps, since these change over time.

## Usage examples
- "Use SIT to find new variants of our onboarding flow."
- "Apply the five SIT tools to this game mechanic."
- "I want new ideas for this process without adding anything new."

See `examples/walkthrough.md` for a worked example.

## Limitations
SIT generates candidate ideas; it does not validate them. Feasibility, cost and market fit still need human judgment and testing.

## Credits and trademark
Independent, unofficial implementation based on publicly described SIT ideas (derived from TRIZ; developed by Roni Horowitz, Jacob Goldenberg, David Mazursky and colleagues). Not affiliated with or endorsed by SIT Ltd. "Systematic Inventive Thinking" / "SIT" may be registered trademarks of their owners. Recommended reading: *Inside the Box* by Drew Boyd and Jacob Goldenberg.

## License
MIT - see `LICENSE`.
