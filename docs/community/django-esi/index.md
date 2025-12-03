---
search:
  exclude: true

title: Django-ESI
type: resource
description: Django-приложение для удобного доступа к EVE Swagger Interface (ESI)
maintainer:
  name: Alliance Auth Team
  gitlab: allianceauth
---

# Django-ESI

Django-приложение для удобного доступа к EVE Swagger Interface (ESI)

[![Version](https://img.shields.io/pypi/v/django-esi)](https://pypi.org/project/django-esi/)
[![Python Versions](https://img.shields.io/pypi/pyversions/django-esi)](https://pypi.org/project/django-esi/)
[![Django Versions](https://img.shields.io/pypi/djversions/django-esi)](https://pypi.org/project/django-esi/)
[![License](https://img.shields.io/badge/license-GPLv3-green)](https://pypi.org/project/django-esi/)
[![Pipeline Status](https://gitlab.com/allianceauth/django-esi/badges/master/pipeline.svg)](https://gitlab.com/allianceauth/django-esi/pipelines)
[![Test Coverage](https://gitlab.com/allianceauth/django-esi/badges/master/coverage.svg)](https://gitlab.com/allianceauth/django-esi/pipelines)
[![Documentation Status](https://readthedocs.org/projects/django-esi/badge/?version=latest)](https://django-esi.readthedocs.io/en/latest/?badge=latest)
[![Pre-Commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

<div class="grid cards" markdown>

- [:simple-discord: __Discord__](https://discord.gg/fjnHAmk){ .esi-card-link }
- [:simple-gitlab: __GitLab__](https://gitlab.com/allianceauth/django-esi){ .esi-card-link }
- [:octicons-browser-16: __Документация__](https://django-esi.readthedocs.io/en/latest/){ .esi-card-link }

</div>

## Описание

Django-esi — это Django-приложение, которое предоставляет интерфейс для удобного доступа к EVE Swagger Interface (ESI), официальному API игры [EVE Online](https://www.eveonline.com/).

Оно построено на [Bravado](https://github.com/Yelp/bravado) - клиентской библиотеке Python для сервисов Swagger 2.0.

Django-esi добавляет следующие основные функциональности на сайт Django:

- Динамически генерируемый клиент для взаимодействия с публичными и приватными конечными точками ESI
- Поддержка добавления EVE SSO для аутентификации персонажей и получения токенов
- Контроль над тем, какие версии конечных точек ESI используются
