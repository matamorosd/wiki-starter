# Wiki personal — guía para Claude

## Configuración inicial (primera vez)

`setup: pendiente`

Si la línea de arriba dice `pendiente`, antes de hacer cualquier otra cosa haz la entrevista de configuración, **una pregunta a la vez**, en lenguaje simple y sin jerga técnica:

1. ¿Cómo te llamo?
2. ¿A qué te dedicas y para qué quieres usar este wiki? (trabajo, estudios, emprendimiento, casa y familia, salud y deporte, hobbies…)
3. ¿Qué días y horarios **no** trabajas? (para no agendar nada ahí)
4. ¿Cuáles son los 2 o 3 frentes o proyectos que tienes abiertos ahora?
5. ¿Usas algún calendario (Google, Outlook, Apple)? ¿Quieres que te lo recuerde cuando aparezca una fecha?
6. ¿Hay algo que este wiki **nunca** debe guardar o tocar? (por ejemplo, cosas de tu trabajo si tu empresa no lo permite)

Con las respuestas:

- Completa la sección **Sobre mí** de este archivo.
- Crea las carpetas temáticas que tengan sentido para su perfil (por ejemplo `clientes/`, `cursos/`, `salud/`, `viajes/`, `recetas/`) y agrégalas a `index.md`. No crees más de 5 al principio.
- Crea una página por cada proyecto que mencionó, con `templates/project-page.md` (ver [[#Proyectos]]).
- Llena `Ahora.md` con su foco y sus fechas.
- Crea el daily de hoy.
- Cambia la línea de arriba a `setup: listo (AAAA-MM-DD)`.
- Termina explicando en 5 líneas cómo usar el wiki día a día (ver [[Método de trabajo del wiki]]).

## Sobre mí

- **Nombre:** <<completar>>
- **Perfil:** <<completar>>
- **Para qué uso este wiki:** <<completar>>
- **Días sin trabajo:** <<completar>> — nunca agendes recordatorios, revisiones ni seguimientos esos días. Si yo misma/o propongo uno de esos días, avísame y confirma.
- **Calendario:** <<completar>>
- **Nunca guardar ni tocar:** <<completar>>

## Tono

Cercano, simple y sin jerga. Si usas un término técnico, explícalo en una frase. Los dailies y el `inbox/` son borradores: no los pulas. Las páginas de proyectos y `evergreen/` sí van más ordenadas y enlazadas.

## Forma del wiki

- `Ahora.md` — una pantalla con foco (máx. 3), a quién espero y próximas fechas.
- `index.md` — el mapa. Mantenlo al día.
- `inbox/` — captura rápida, cualquier cosa.
- `daily/AAAA/MM/AAAA-MM-DD.md` — el daily.
- `projects/` — una carpeta por proyecto.
- `evergreen/` — ideas y aprendizajes que duran.
- `meetings/` — notas de reuniones.
- `attachments/` — imágenes y PDFs.
- `templates/` — plantillas. Se copian, no se editan en el lugar.

## Proyectos

- Cada proyecto vive en `projects/<Nombre>/<Nombre>.md`. El archivo se llama **igual que el proyecto**, para que `[[Nombre]]` funcione en Obsidian. Las subnotas van en la misma carpeta, con nombres como `<Nombre> — Presupuesto.md`.
- El frontmatter lleva `status:` (active | paused | maintenance | done | reference) y `updated:` (AAAA-MM-DD).
- Cada proyecto tiene `▶ Retomar aquí`, con dónde quedó y el próximo paso, y `## Decisiones`, con una línea por decisión: `AAAA-MM-DD — decisión — por qué`.
- Si el archivo principal pasa de ~200 líneas, el detalle se divide en subnotas (plan, bitácora, guías) y el principal queda como resumen.

## Ritmo de trabajo

- Al empezar una sesión, lee `Ahora.md`.
- Al terminar una sesión:
  1. Actualiza el `▶ Retomar aquí` del proyecto y su `updated:`.
  2. Agrega una línea en *Hecho hoy* del daily (créalo desde `templates/daily-note.md` si no existe).
  3. Si cambió el foco o apareció una fecha, actualiza `Ahora.md`.
- Las fechas comprometidas van al calendario de la persona. Si no tienes acceso a su calendario, dale la lista para que las agregue y márcalas con 📅 en la nota cuando estén agendadas. Nunca en sus días sin trabajo.
- **Revisión semanal:** cuando diga "hagamos la revisión semanal", sigue el checklist de `Ahora.md`.

## Frases que entiendes

- **"nuevo daily"** — crea el daily de hoy desde la plantilla.
- **"nuevo proyecto X"** — crea `projects/X/X.md` desde la plantilla, lo agrega a `index.md` y pregunta lo mínimo para llenarlo.
- **"anota esto: …"** — va al daily de hoy, en *Capturas*.
- **"promueve X"** — lee la nota, busca notas relacionadas, crea una nota nueva o la une a una existente, enlaza en ambas direcciones, actualiza `index.md` si corresponde y deja una línea en el origen indicando a dónde se fue.
- **"decidí …"** — agrega la línea a `## Decisiones` del proyecto correspondiente.
- **"¿en qué estaba?"** — resume `Ahora.md` y el `▶ Retomar aquí` del proyecto.
- **"hagamos la revisión semanal"** — checklist de `Ahora.md`.

## Links y etiquetas

- Links internos con `[[Título de la nota]]`, usando el título (el nombre del archivo), no la ruta.
- Etiquetas planas: `#viaje`, `#libro`, `#receta`. Sin jerarquías.
- Los alias van en el frontmatter (`aliases:`).

## Datos sensibles (regla dura)

Nunca escribas en este wiki, aunque yo lo pegue por error:

- Contraseñas, claves, tokens, códigos de verificación o llaves privadas.
- Números de tarjeta o de cuenta bancaria, ni datos para entrar al banco.
- Datos personales de otras personas (RUT/DNI, direcciones, teléfonos) más allá de un nombre.
- Detalles de fichas médicas.

Si pego algo así, bórralo en el lugar y avísame. Para referirte a eso, hazlo en abstracto ("la contraseña está en el gestor de contraseñas").

Aunque el repositorio sea privado, trátalo como si alguien más pudiera leerlo algún día.

## Comportamiento por defecto

- Preferir editar notas existentes antes que crear nuevas.
- Si no sabes dónde va algo, déjalo en `inbox/` y dime.
- No te salgas de esta carpeta: no leas ni escribas archivos fuera del wiki salvo que te lo pida explícitamente.
- No hagas commits ni pushes: el respaldo lo hace GitHub Desktop u Obsidian Git (ver el README).
- Explica lo que hiciste en pocas líneas, sin tecnicismos.
