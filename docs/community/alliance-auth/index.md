---
search:
  exclude: true

title: Alliance Auth
type: service
description: Система аутентификации для EVE Online, помогающая внутриигровым организациям управлять доступом к онлайн-сервисам.
maintainer:
  name: Alliance Auth Team
  gitlab: allianceauth
---

# Alliance Auth 

[![Version](https://img.shields.io/pypi/v/allianceauth)](https://pypi.org/project/allianceauth/)
[![Python Versions](https://img.shields.io/pypi/pyversions/allianceauth)](https://pypi.org/project/allianceauth/)
[![Django Versions](https://img.shields.io/pypi/djversions/allianceauth)](https://pypi.org/project/allianceauth/)
[![License](https://img.shields.io/badge/license-GPLv2-green)](https://pypi.org/project/allianceauth/)
[![Pipeline Status](https://gitlab.com/allianceauth/allianceauth/badges/master/pipeline.svg)](https://gitlab.com/allianceauth/allianceauth/pipelines)
[![Test Coverage](https://gitlab.com/allianceauth/allianceauth/badges/master/coverage.svg)](https://gitlab.com/allianceauth/allianceauth/pipelines)
[![Documentation Status](https://readthedocs.org/projects/allianceauth/badge/?version=latest)](https://allianceauth.readthedocs.io/en/latest/?badge=latest)
[![Pre-Commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

![Alliance Auth](auth-logo.svg)

<div class="grid cards" markdown>

- [:simple-discord: __Discord__](https://discord.gg/fjnHAmk){ .esi-card-link }
- [:simple-gitlab: __GitLab__](https://gitlab.com/allianceauth/allianceauth){ .esi-card-link }
- [:octicons-browser-16: __Документация__](https://allianceauth.readthedocs.io/){ .esi-card-link }

</div>

## Описание

Alliance Auth (AA) — это веб-сайт, который помогает организациям Eve Online эффективно управлять доступом к приложениям и сервисам.

## Возможности

- Автоматически предоставляет или отзывает доступ пользователей к внешним сервисам (например, Discord, Mumble) и веб-приложениям (например, запросы SRP) на основе текущего членства пользователя во [внутриигровых организациях](https://allianceauth.readthedocs.io/en/latest/features/core/states.html) и [группах](https://allianceauth.readthedocs.io/en/latest/features/core/groups.html)

- Предоставляет центральный веб-сайт, где пользователи могут напрямую получать доступ к веб-приложениям (например, запросы SRP, расписание флота) и управлять своим доступом к внешним сервисам и группам.

- Включает набор коннекторов (называемых ["сервисами"](https://allianceauth.readthedocs.io/en/latest/features/services/)) для интеграции управления доступом со многими популярными внешними приложениями / сервисами, такими как Discord, Mumble, Teamspeak 3, SMF и другие

- Включает набор веб-[приложений](https://allianceauth.readthedocs.io/en/latest/features/apps/), которые добавляют множество полезных функций, например: расписание флота, доска таймеров, управление запросами SRP, трекер активности флота

- Может быть легко расширен дополнительными сервисами и приложениями. Многие предоставляются сообществом и могут быть найдены здесь: [Community Creations](https://gitlab.com/allianceauth/community-creations)

- Локализация на английском :flag_gb:, китайском :flag_cn:, немецком :flag_de:, испанском :flag_es:, корейском :flag_kr:, русском :flag_ru:, итальянском :flag_it:, французском :flag_fr:, японском :flag_jp: и украинском :flag_ua: языках

Для получения дополнительной информации об AA - включая руководство по установке и полный список включенных сервисов и плагинов - см. [официальную документацию](https://allianceauth.rtfd.io).

# Сообщество Alliance Auth

- Более 100+ приложений от 30+ разработчиков

<https://gitlab.com/allianceauth/community-creations>
