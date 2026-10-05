# Claude Mods Starter Kit

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![Claude Mods Starter Kit](guia/assets/banner.jpg)](https://inematds.github.io/claude-mods-starter-kit/guia/)

> Espelho INEMA de [promptadvisers/claude-mods-starter-kit](https://github.com/promptadvisers/claude-mods-starter-kit) (licença MIT). Todo o crédito à Prompt Advisers.

## 📖 Guia de uso

Guia completo em português (landing + passo a passo): **https://inematds.github.io/claude-mods-starter-kit/guia/**

## Deixe o Claude Code com a sua cara

**Dez mods com código-fonte. Dez prompts completos para criar. Um guia para iniciantes que diz onde digitar cada comando.**

Um mod é a mudança que você quer. Um plugin é o pacote que leva essa mudança para o Claude Code. Comece com um bichinho no terminal, veja o trabalho numa linha do tempo, ache os arquivos que o Claude criou e deixe um ponto de retomada para depois.

[Comece aqui](START-HERE.md) · [PDF](CLAUDE-MODS-VIEWER-GUIDE.pdf) · [Crie o seu](guides/BUILD-YOUR-OWN.md) · [Desligar tudo](guides/DATA-AND-REMOVAL.md) *(documentos em inglês)*

## Primeira vitória

Com o Claude Code instalado e logado, rode no terminal:

```bash
claude plugin marketplace add promptadvisers/claude-mods-starter-kit --scope user
claude plugin install terminal-pet@claude-mods-kit --scope user
```

Abra uma sessão nova do Claude Code e digite `/pet party`. Para esconder, `/pet off`.

Quer só testar? Na pasta do kit, rode `bash scripts/try.sh terminal-pet`. Ele cria uma pasta de demonstração nova; suas configurações de plugin não mudam.

## Escolha a mudança

| Mod | Para quê | Dentro do Claude Code |
|---|---|---|
| [Terminal Pet](guides/01-terminal-pet.md) | Companhia enquanto o Claude trabalha. | `/pet on` |
| [Coral Skin](guides/02-coral-skin.md) | Deixa o trabalho mais fácil de ler. | `/skin on` |
| [Context Meter](guides/03-context-meter.md) | Mostra o quanto a conversa está cheia. | automático |
| [Repo Heatmap](guides/04-repo-heatmap.md) | Mostra quais arquivos o Claude mexe. | `/heatmap open` |
| [Flight Recorder](guides/05-flight-recorder.md) | O trabalho numa linha do tempo. | `/timeline open` |
| [Model Router](guides/06-model-router.md) | Modelo mais leve para os subagentes. | `/router on` |
| [Output Tray](guides/07-output-tray.md) | Acha os arquivos que o Claude criou. | `/tray show` |
| [Changes Receipt](guides/08-changes-receipt.md) | Lista clara do que mudou. | `/receipt on` |
| [Session Bookmarks](guides/09-session-bookmarks.md) | Nota de "volte aqui" para a sessão. | `/bm save Login walkthrough` |
| [Auto Handoff](guides/10-auto-handoff.md) | Ponto de partida para a próxima conversa. | `/autohandoff` |

## O que tem dentro

- **VIEWER-GUIDE.html** e **CLAUDE-MODS-VIEWER-GUIDE.pdf**: guia offline com busca e referência ilustrada (em inglês).
- **prompts/**: dez especificações completas e editáveis.
- **plugins/**: código-fonte, manifestos e testes.
- **demo-project/**: um fluxo de login fictício para explorar sem usar seu trabalho.
- **scripts/**: demo temporária, instalar/desativar/desinstalar e checagens.
- **templates/starter-mod/**: um mod mínimo para aprender.
- **guia/**: o guia INEMA em PT, EN e ES.

## Vários de uma vez, ou desligar o kit

```bash
bash scripts/manage.sh install user all   # instala os dez
bash scripts/manage.sh disable user all   # desativa os dez
```

Router muda qual modelo trabalha e Handoff grava arquivos e faz uma chamada extra ao modelo: escolha esses com calma.

## Limites

Versão 1.0.0, conferida com Claude Code 2.1.287 no macOS em 2 de outubro de 2026. Testes unitários simulam terminal e desktop; não é certificação de ponta a ponta. Output Tray abre/mostra arquivos só no macOS. Custos exibidos são estimativas. Detalhes em [VERIFICATION.md](VERIFICATION.md).

## Créditos

Projeto comunitário da [Prompt Advisers](https://promptadvisers.com) · [Early AI Adopters](https://www.skool.com/earlyaidopters/about). Sem vínculo com a Anthropic. Código MIT, ver [LICENSE](LICENSE). Guia PT/EN/ES: [INEMA.CLUB](https://inema.club).
