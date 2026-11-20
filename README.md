# Wiki Starter: tu wiki personal con Obsidian + Claude

Un cuaderno digital para ordenar tus proyectos, tus decisiones y tu día a día. Tú escribes y conversas; **Claude** te ayuda a ordenar, resumir y conectar las notas; y **GitHub** guarda una copia privada de todo en internet.

- **Obsidian** es la app donde lees y escribes tus notas. Gratis.
- **Claude** es el asistente que trabaja dentro de tu carpeta de notas. Necesita un plan pagado de Claude (Pro o superior).
- **GitHub** es donde se respalda tu wiki, en un espacio **privado** que solo tú ves. Gratis.
- **GitHub Desktop** es la app que sube tus cambios a GitHub con un par de clics. Gratis.

> Tiempo total la primera vez: unos 45 minutos. Si alguien te acompaña, sigan esta guía juntos.

---

## Índice

1. [Crear tu cuenta de GitHub](#1-crear-tu-cuenta-de-github)
2. [Crear tu copia privada del wiki](#2-crear-tu-copia-privada-del-wiki)
3. [Instalar GitHub Desktop y bajar tu wiki al computador](#3-instalar-github-desktop-y-bajar-tu-wiki-al-computador)
4. [Instalar Obsidian y abrir tu wiki](#4-instalar-obsidian-y-abrir-tu-wiki)
5. [Instalar Claude y conectarlo a tu wiki](#5-instalar-claude-y-conectarlo-a-tu-wiki)
6. [Primera conversación: configurar el wiki para ti](#6-primera-conversación-configurar-el-wiki-para-ti)
7. [El día a día](#7-el-día-a-día)
8. [Respaldar en GitHub](#8-respaldar-en-github)
9. [Privacidad: lo que nunca va en el wiki](#9-privacidad-lo-que-nunca-va-en-el-wiki)
10. [Problemas frecuentes](#10-problemas-frecuentes)
11. [Anexo para quien acompaña: respaldo automático](#anexo-para-quien-acompaña-respaldo-automático)

---

## 1. Crear tu cuenta de GitHub

Si ya tienes cuenta, salta al paso 2.

1. Entra a **https://github.com/signup**.
2. Escribe tu correo, una contraseña y un **nombre de usuario**. Elige uno simple, porque aparece en tus links (por ejemplo `mariagonzalez`).
3. Resuelve la verificación (un pequeño puzzle) y escribe el **código que te llega al correo**.
4. Si te pregunta por un plan, elige **Free** (gratis). Las preguntas de personalización se pueden saltar.
5. Recomendado: activa la verificación en dos pasos en **tu foto (arriba a la derecha) → Settings → Password and authentication**. Guarda los códigos de recuperación en tu gestor de contraseñas, **no en el wiki**.

## 2. Crear tu copia privada del wiki

Así obtienes tu propio wiki, separado del de los demás. Nadie más lo ve.

1. Con tu sesión de GitHub abierta, entra a **https://github.com/matamorosd/wiki-starter**.
2. Arriba a la derecha, haz clic en el botón verde **Use this template** → **Create a new repository**.
3. Completa:
   - **Owner:** tu usuario.
   - **Repository name:** `mi-wiki` (o el nombre que quieras).
   - Marca **Private**. ⚠️ Es importante: así solo tú puedes verlo.
4. Haz clic en **Create repository**.

Listo: ahora tienes `github.com/<tu-usuario>/mi-wiki`, privado.

## 3. Instalar GitHub Desktop y bajar tu wiki al computador

1. Descarga GitHub Desktop desde **https://desktop.github.com** e instálalo.
   - **Mac:** abre el archivo descargado y arrastra GitHub Desktop a **Aplicaciones**.
   - **Windows:** ejecuta el instalador.
2. Abre GitHub Desktop → **Sign in to GitHub.com**. Se abre el navegador: haz clic en **Authorize desktop** y vuelve a la app.
3. Si te pide nombre y correo para "Git", deja los que aparecen y haz clic en **Finish**.
4. Elige **Clone a repository from the Internet…** (o en el menú **File → Clone repository…**).
5. En la pestaña **GitHub.com**, selecciona `mi-wiki`.
6. En **Local path**, elige tu carpeta **Documentos**. Quedará en `Documentos/mi-wiki`.
7. Haz clic en **Clone**.

## 4. Instalar Obsidian y abrir tu wiki

1. Descarga Obsidian desde **https://obsidian.md** e instálalo.
2. Ábrelo y elige **Open folder as vault** (abrir carpeta como bóveda).
3. Selecciona `Documentos/mi-wiki` → **Open**.
4. Abre la nota **`index`** en el panel izquierdo. Ese es el mapa de tu wiki.

Tres cosas útiles de Obsidian:

- Escribir `[[` crea un link a otra nota.
- El ícono de calendario en la barra izquierda abre **el daily de hoy**.
- `Cmd + O` (Mac) o `Ctrl + O` (Windows) busca cualquier nota por su nombre.

## 5. Instalar Claude y conectarlo a tu wiki

Necesitas una cuenta de Claude con plan **Pro o superior** (https://claude.ai).

**Opción recomendada: la app de escritorio de Claude**

1. Descarga la app desde **https://claude.ai/download**, instálala e inicia sesión.
2. Entra a la sección **Code** (Claude Code).
3. Cuando te pida una carpeta, elige `Documentos/mi-wiki`.
4. Claude te va a pedir permiso antes de crear o editar notas. Léelo y acepta. Puedes permitirlo "siempre" para esta carpeta.

**Alternativa: la Terminal** (si quien te acompaña lo prefiere)

- Mac: abre **Terminal** y pega `curl -fsSL https://claude.ai/install.sh | bash`.
- Windows: abre **PowerShell** y pega `irm https://claude.ai/install.ps1 | iex`.
- Luego: `cd ~/Documents/mi-wiki` y `claude`. La primera vez te pide iniciar sesión en el navegador.

> Claude trabaja solo dentro de la carpeta de tu wiki. Las reglas que sigue están en el archivo `CLAUDE.md`. Puedes leerlo, y Claude lo completa contigo en el paso siguiente.

## 6. Primera conversación: configurar el wiki para ti

Con Claude abierto en tu carpeta, escribe:

> **Hola. Lee CLAUDE.md y hagamos la configuración inicial del wiki.**

Claude te hará unas 6 preguntas, una a la vez: cómo llamarte, a qué te dedicas, qué días no trabajas, en qué proyectos estás, si usas calendario y qué no debe guardar nunca. Con eso:

- crea las carpetas que tengan sentido para ti (por ejemplo *clientes*, *cursos*, *salud*, *viajes*),
- crea una página para cada proyecto,
- llena tu página **Ahora** (foco y fechas),
- crea tu primer daily.

Al terminar, respalda en GitHub (paso 8).

## 7. El día a día

Cosas que puedes decirle a Claude tal cual:

| Dices | Claude hace |
| --- | --- |
| "nuevo daily" | Crea la nota de hoy |
| "anota esto: llamar al dentista el jueves" | Lo guarda en el daily de hoy |
| "nuevo proyecto Mudanza" | Crea la página del proyecto y te hace un par de preguntas |
| "¿en qué estaba con la Mudanza?" | Te resume dónde quedó y el próximo paso |
| "decidí arrendar en vez de comprar, porque…" | Lo anota en las decisiones del proyecto, con fecha |
| "promueve la nota X del inbox" | La ordena y la lleva a su lugar |
| "hagamos la revisión semanal" | Repasa contigo los proyectos y actualiza **Ahora** |

**Un buen ritmo:**

- **Cada día:** abre el daily y anota lo que vaya surgiendo. Trabaja con Claude en lo que toque; al cerrar, Claude deja anotado dónde quedaste.
- **Una vez por semana (15 min):** "hagamos la revisión semanal". Elige un día fijo, por ejemplo el viernes.
- **Cuando aparezca una fecha:** agrégala a tu calendario (Google, Outlook o Apple) y márcala con 📅 en la nota.

Más detalle en la nota **Método de trabajo del wiki**, dentro de tu wiki.

## 8. Respaldar en GitHub

Hazlo **al final de cada día** en que hayas usado el wiki (toma 10 segundos):

1. Abre **GitHub Desktop**. A la izquierda verás las notas que cambiaron.
2. Abajo a la izquierda, en **Summary**, escribe algo corto, como `notas del día`.
3. Haz clic en **Commit to main**.
4. Haz clic en **Push origin** (arriba).

Listo: tu copia en GitHub está al día. Si usas el wiki en dos computadores, en el otro haz clic en **Fetch origin** y luego en **Pull origin** antes de empezar.

> ¿Prefieres que se respalde solo, sin clics? Pídele a quien te acompaña el [anexo de respaldo automático](#anexo-para-quien-acompaña-respaldo-automático).

## 9. Privacidad: lo que nunca va en el wiki

Aunque tu repositorio es privado, **nunca** guardes en el wiki:

- contraseñas, códigos de verificación ni claves,
- números de tarjeta o de cuenta bancaria,
- datos personales de otras personas (documento de identidad, dirección, teléfono),
- detalles de fichas médicas.

Para eso usa un gestor de contraseñas (Contraseñas de Apple, 1Password, Bitwarden). Claude tiene la instrucción de borrar esos datos si los pegas por error, y de avisarte.

Si tu trabajo tiene reglas sobre dónde guardar información de la empresa, respétalas: este wiki es **personal**.

## 10. Problemas frecuentes

- **"Claude no encuentra mis notas":** revisa que hayas abierto Claude en la carpeta `Documentos/mi-wiki`, no en otra.
- **GitHub Desktop no muestra cambios:** guarda la nota en Obsidian (se guarda sola) y espera unos segundos. Revisa que en GitHub Desktop esté seleccionado `mi-wiki` arriba a la izquierda.
- **"Push rejected" o un aviso de conflicto:** primero haz **Pull origin** y después **Push origin**. Si aparece un conflicto, pide ayuda antes de seguir.
- **Un link `[[...]]` sale en otro color y crea una nota vacía:** la nota con ese nombre no existe. Pídele a Claude: "revisa los links rotos".
- **Borré algo por error:** en GitHub Desktop, clic derecho sobre el archivo → **Discard changes**. Si ya lo habías subido, la historia en GitHub guarda todas las versiones: pide ayuda para recuperarlo.

## Actualizaciones de esta plantilla

Las mejoras se anotan en [CHANGELOG.md](CHANGELOG.md). Tu wiki no se actualiza solo (es tuyo). Si una mejora te interesa, pídele a Claude: *"lee el CHANGELOG de github.com/matamorosd/wiki-starter y aplícame el cambio X"*.

---

## Anexo para quien acompaña: respaldo automático

Opcional. Reemplaza el paso 8 por un respaldo automático cada 10 minutos desde Obsidian, con el plugin **Git**. Requiere git por línea de comandos y credenciales HTTPS.

**Mac**

1. Terminal: `xcode-select --install` (instala git; acepta el diálogo).
2. Instalar GitHub CLI: `brew install gh`, o el instalador de https://cli.github.com.
3. `gh auth login` → GitHub.com → HTTPS → *Login with a web browser*. Después, `gh auth setup-git`.
4. Verificar dentro de `~/Documents/mi-wiki`: `git pull` y `git push` sin que pida contraseña.

**Windows**

1. Instalar **Git for Windows** (https://git-scm.com), con las opciones por defecto (incluye Git Credential Manager).
2. En PowerShell, dentro de la carpeta del wiki: `git push`. Se abre el navegador para autorizar una vez.

**En Obsidian (ambos sistemas)**

1. **Settings → Community plugins → Turn on community plugins → Browse**, buscar **Git** (de Vinzent03) → **Install** → **Enable**.
2. En las opciones del plugin:
   - *Auto commit-and-sync interval*: `10` minutos.
   - *Pull on startup*: activado.
   - *Commit message*: `vault backup: {{date}}`.
3. Probar: editar una nota, esperar 10 minutos y revisar el historial en github.com.

**Checklist de acompañamiento**

- [ ] Repo creado desde la plantilla y **privado**.
- [ ] 2FA activado en GitHub.
- [ ] Clonado en `Documentos/mi-wiki` y abierto en Obsidian.
- [ ] Claude abierto en esa carpeta y configuración inicial hecha (`setup: listo` en `CLAUDE.md`).
- [ ] Primer respaldo hecho y visible en github.com.
- [ ] Revisión semanal agendada en su calendario.
