# Claude Mods Starter Kit

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![Claude Mods Starter Kit](guia/assets/banner-es.jpg)](https://inematds.github.io/claude-mods-starter-kit/guia/es/)

> Espejo INEMA de [promptadvisers/claude-mods-starter-kit](https://github.com/promptadvisers/claude-mods-starter-kit) (licencia MIT). Todo el crédito a Prompt Advisers.

## 📖 Guía de uso

Guía completa en español (landing + paso a paso): **https://inematds.github.io/claude-mods-starter-kit/guia/es/**

## Haz que Claude Code se sienta tuyo

**Diez mods con código fuente. Diez prompts completos para crear. Una guía para principiantes que te dice dónde escribir cada comando.**

Un mod es el cambio que quieres. Un plugin es el paquete que lleva ese cambio a Claude Code. Empieza con una mascota en la terminal, mira el trabajo en una línea de tiempo, encuentra los archivos que Claude creó y déjate un punto para retomar después.

[Empieza aquí](START-HERE.md) · [PDF](CLAUDE-MODS-VIEWER-GUIDE.pdf) · [Crea el tuyo](guides/BUILD-YOUR-OWN.md) · [Apagar todo](guides/DATA-AND-REMOVAL.md) *(documentos en inglés)*

## Primera victoria

Con Claude Code instalado y con sesión iniciada, ejecuta en la terminal:

```bash
claude plugin marketplace add promptadvisers/claude-mods-starter-kit --scope user
claude plugin install terminal-pet@claude-mods-kit --scope user
```

Abre una sesión nueva de Claude Code y escribe `/pet party`. Para ocultarla, `/pet off`.

¿Solo quieres probar? En la carpeta del kit, ejecuta `bash scripts/try.sh terminal-pet`. Crea una carpeta de demostración nueva; tu configuración de plugins no cambia.

## Elige el cambio

| Mod | Para qué | Dentro de Claude Code |
|---|---|---|
| [Terminal Pet](guides/01-terminal-pet.md) | Compañía mientras Claude trabaja. | `/pet on` |
| [Coral Skin](guides/02-coral-skin.md) | Hace el trabajo más fácil de leer. | `/skin on` |
| [Context Meter](guides/03-context-meter.md) | Muestra qué tan llena está la conversación. | automático |
| [Repo Heatmap](guides/04-repo-heatmap.md) | Muestra qué archivos toca Claude. | `/heatmap open` |
| [Flight Recorder](guides/05-flight-recorder.md) | El trabajo en una línea de tiempo. | `/timeline open` |
| [Model Router](guides/06-model-router.md) | Modelo más ligero para los subagentes. | `/router on` |
| [Output Tray](guides/07-output-tray.md) | Encuentra los archivos que Claude creó. | `/tray show` |
| [Changes Receipt](guides/08-changes-receipt.md) | Lista clara de lo que cambió. | `/receipt on` |
| [Session Bookmarks](guides/09-session-bookmarks.md) | Nota de "vuelve aquí" para la sesión. | `/bm save Login walkthrough` |
| [Auto Handoff](guides/10-auto-handoff.md) | Punto de partida para la próxima conversación. | `/autohandoff` |

## Qué incluye

- **VIEWER-GUIDE.html** y **CLAUDE-MODS-VIEWER-GUIDE.pdf**: guía offline con búsqueda y referencia ilustrada (en inglés).
- **prompts/**: diez especificaciones completas y editables.
- **plugins/**: código fuente, manifiestos y pruebas.
- **demo-project/**: un flujo de login ficticio para explorar sin usar tu trabajo.
- **scripts/**: demo temporal, instalar/desactivar/desinstalar y verificaciones.
- **templates/starter-mod/**: un mod mínimo para aprender.
- **guia/**: la guía INEMA en PT, EN y ES.

## Varios a la vez, o apagar el kit

```bash
bash scripts/manage.sh install user all   # instala los diez
bash scripts/manage.sh disable user all   # desactiva los diez
```

Router cambia qué modelo trabaja y Handoff escribe archivos y hace una llamada extra al modelo: elige esos con calma.

## Límites

Versión 1.0.0, verificada con Claude Code 2.1.287 en macOS el 2 de octubre de 2026. Las pruebas unitarias simulan terminal y escritorio; no es una certificación de extremo a extremo. Output Tray abre/muestra archivos solo en macOS. Los costos mostrados son estimaciones. Detalles en [VERIFICATION.md](VERIFICATION.md).

## Créditos

Proyecto comunitario de [Prompt Advisers](https://promptadvisers.com) · [Early AI Adopters](https://www.skool.com/earlyaidopters/about). Sin vínculo con Anthropic. Código MIT, ver [LICENSE](LICENSE). Guía PT/EN/ES: [INEMA.CLUB](https://inema.club).
