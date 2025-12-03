---
search:
  exclude: true

title: elt
type: service
description: elt — это инструмент командной строки для поиска объектов Eve Online. Доступен для Windows, macOS и Linux.
maintainer:
  name: Erik Kalkoken
  github: ErikKalkoken
---

# elt - EVE Lookup Tool

**elt** — это инструмент командной строки для поиска объектов Eve Online. Доступен для Windows, macOS и Linux.

[![GitHub Release](https://img.shields.io/github/v/release/ErikKalkoken/elt)](https://github.com/ErikKalkoken/elt/elt)
[![GitHub License](https://img.shields.io/github/license/ErikKalkoken/elt)](https://github.com/ErikKalkoken/elt?tab=MIT-1-ov-file#readme)
[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/tVSCQEVJnJ)

<div class="grid cards" markdown>

- [:octicons-mark-github-16: __GitHub__](https://github.com/ErikKalkoken/elt){ .esi-card-link }
- [:simple-discord: __Discord__](https://discord.gg/tVSCQEVJnJ){ .esi-card-link }

</div>

**elt** — это инструмент командной строки, который ищет объекты EVE Online с игрового сервера и выводит их в терминале. Он предоставляет удобную и быструю альтернативу использованию браузера или команд curl для быстрого разрешения ID или имен Eve в терминале.

Например:

```sh
elt "Jita"
```

Выведет

```plain
Solar System:
┌──────────┬──────┬──────────────────┬────────────────────┬───────────┬─────────────┬────────────┐
│    ID    │ NAME │ CONSTELLATION ID │ CONSTELLATION NAME │ REGION ID │ REGION NAME │  SECURITY  │
├──────────┼──────┼──────────────────┼────────────────────┼───────────┼─────────────┼────────────┤
│ 30000142 │ Jita │ 20000020         │ Kimotoro           │ 10000002  │ The Forge   │ 0.94591314 │
└──────────┴──────┴──────────────────┴────────────────────┴───────────┴─────────────┴────────────┘
```

Для получения дополнительной информации посетите [репозиторий Github](https://github.com/ErikKalkoken/elt).
