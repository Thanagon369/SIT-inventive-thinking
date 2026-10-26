# Manual de uso: skill SIT (Systematic Inventive Thinking)

Guía corta para instalar y usar la skill `sit-inventive-thinking`.

## 1. ¿Qué hace?

Te ayuda a generar ideas nuevas **a partir de lo que ya existe**, usando 5 operaciones:
**Sustracción, División, Unificación de tareas, Multiplicación y Dependencia de atributos**.
Trabaja dentro de un "mundo cerrado": solo usa componentes que ya están en tu problema, sin agregar apps, sensores o IA nuevos.

Sirve para mejorar un producto, servicio, proceso, flujo de trabajo o mecánica de juego.

---

## 2. Instalación

Elige **una** de estas opciones.

### Opción A: Claude.ai (web o app de escritorio), descargando `SKILL.md`

La skill se sube como un archivo ZIP. **Importante:** el ZIP debe contener una *carpeta* con `SKILL.md` adentro, no el archivo suelto.

1. Abre este enlace y descarga `SKILL.md` (botón de descarga arriba a la derecha del archivo):
   `https://github.com/Thanagon369/SIT-inventive-thinking/blob/main/SKILL.md`
2. En tu computador, crea una carpeta llamada exactamente **`sit-inventive-thinking`** (en minúsculas, con guiones).
3. Mete `SKILL.md` dentro de esa carpeta.
4. Comprime **la carpeta** (clic derecho sobre la carpeta, "Comprimir" o "Enviar a carpeta comprimida"). No comprimas solo el archivo.
5. Entra a `claude.ai/customize/skills` (**Customize > Skills**), usa la opción de subir una skill y selecciona el ZIP.
6. **Activa** la skill con su interruptor.

### Opción B: Claude Code (terminal)

Clona el repositorio directamente dentro de tu carpeta de skills, con el nombre correcto:

```bash
git clone https://github.com/Thanagon369/SIT-inventive-thinking ~/.claude/skills/sit-inventive-thinking
```

Abre `claude` en cualquier proyecto y escribe `/sit-inventive-thinking` para usarla.

### Sobre el conector de GitHub

El conector de GitHub **no instala skills**. Sirve para que Claude lea o modifique tus repositorios, pero no activa la skill en tu cuenta. Para instalarla usa la Opción A o la B.

### No uses "Download ZIP" de GitHub

Ese ZIP trae una carpeta llamada `SIT-inventive-thinking-main`, que no coincide con el nombre de la skill (`sit-inventive-thinking`) y puede dar error. Usa la Opción A.

---

## 3. Comprobar que funciona

En un chat nuevo escribe:

> Usa SIT para encontrar variantes de un sistema de reservas de citas

Si está bien instalada, Claude te mostrará: el marco del problema, una lista de componentes, una tabla de variantes y un ranking de las mejores ideas.

---

## 4. Cómo usarla

**Regla de oro: da contexto.** Cuanto más concreto sea tu mensaje, mejores ideas obtienes.

Ejemplos:

- *"Usa SIT en la reserva de citas de mi clínica dental, sin agregar software nuevo."*
- *"Aplica las 5 herramientas de SIT a esta mecánica de mi juego: el jugador recoge munición."*
- *"Quiero variantes de nuestro proceso de recuperación de contraseñas usando solo lo que ya tenemos."*

**Qué recibes:**
1. Los supuestos y el límite del "mundo cerrado".
2. El inventario de componentes y variables.
3. Una tabla con cada idea: herramienta usada, nueva configuración, quién se beneficia, viabilidad y riesgo.
4. Las 3 a 5 mejores ideas y qué validar primero.

**Después puedes pedir:**
- Repetir con un mundo cerrado más estrecho o más amplio.
- Combinar dos herramientas en un mismo componente.
- Profundizar en una idea concreta.

---

## 5. Problemas comunes

| Problema | Qué hacer |
|---|---|
| La skill no se activa | Menciona "SIT" o "pensamiento inventivo sistemático" en tu mensaje y revisa que esté activada en Customize > Skills |
| Error al subir el ZIP | Comprueba que el ZIP contenga la carpeta `sit-inventive-thinking/` con `SKILL.md` adentro y que el nombre coincida |
| Error de YAML | La línea `description:` del encabezado debe ir entre comillas y en una sola línea |
| Las ideas son genéricas | Da más contexto y define qué recursos están permitidos |
| Propone cosas nuevas (apps, sensores) | Recuérdale: "mantente dentro del mundo cerrado" |

---

## 6. Recuerda

- SIT **genera ideas candidatas**, no las valida. La viabilidad, el costo y el mercado los confirmas tú.
- Las viabilidades que indica son aproximadas.
- Esta skill es una implementación independiente y no oficial, basada en ideas públicas de SIT (derivadas de TRIZ). Para profundizar, lee *Inside the Box* de Drew Boyd y Jacob Goldenberg.

Repositorio: https://github.com/Thanagon369/SIT-inventive-thinking
