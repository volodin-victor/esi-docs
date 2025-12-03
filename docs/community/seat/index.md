---
search:
  exclude: true

title: SeAT
type: service
description: SeAT — это простой инструмент управления корпорациями и API для сбора и использования всех данных ESI.
maintainer:
  name: EveSeat Team
  github: eveseat
---

# SeAT - Simple, EVE Online API Tool

<figure markdown="span">
  ![SeAT](seat-logo.svg)
</figure>
[![License](https://img.shields.io/badge/license-GPLv2-green)](https://github.com/eveseat/seat/blob/master/LICENSE)
<div class="grid cards" markdown>

- [:simple-discord: __Discord__](https://discord.com/invite/NQhnMKhc){ .esi-card-link }
- [:simple-github: __GitHub__](https://github.com/eveseat/seat){ .esi-card-link }
- [:octicons-book-16: __Documentation__](https://eveseat.github.io/docs/){ .esi-card-link }

</div>

## Описание

SeAT — это простой инструмент управления корпорациями и API для [EVE Online](https://www.eveonline.com/). SeAT позволяет отслеживать всё, что связано с вашими персонажами, корпорациями и альянсами: от кошельков до почты, от активов персонажей до активов корпораций. Предназначен для установки на публичном сервере для доступа членов вашей организации.

Также часто используется отдельными игроками для управления собственными аккаунтами, а также альянсами и коалициями для управления членами на основе API, контрразведки и администрирования. Существуют установки с количеством зарегистрированных персонажей от однозначных чисел до более 30 000.

## Возможности

- Потребляет данные ESI зарегистрированных персонажей от публичных данных до всех доступных областей чтения ESI. Это включает данные персонажей, корпораций и альянсов.

- Расширенный контроль доступа на основе ролей для управления разрешениями на просмотр и изменение данных в приложении. Подробнее о [Ролях](https://eveseat.github.io/docs/admin_guides/authorizations/).

- Позволяет автоматизировать роли/разрешения на основе данных API, а также использовать ручные методы. Подробнее о [Отрядах](https://eveseat.github.io/docs/admin_guides/squads/).

- Пакеты сообщества для расширения функциональности инструментами, такими как программы SRP, связывание и управление аккаунтами Discord/Teamspeak (и других), планирование и управление производством. См. список [здесь](https://eveseat.github.io/docs/community_packages/#package-list)

- Простая установка Docker доступна и рекомендуется! [Документация](https://eveseat.github.io/docs/installation/docker_installation/)

- Локализация на английском :flag_gb:, китайском :flag_cn:, французском :flag_fr:, немецком :flag_de:, японском :flag_jp:, корейском :flag_kr:, румынском :flag_ro: и русском :flag_ru: языках (разные уровни завершённости. См. [здесь](https://translations.eveseat.net/)).

Для получения дополнительной информации посетите нашу документацию или присоединяйтесь к обсуждению в Discord!

## Скриншоты

**Главная страница пользователя**

![](seat-index.png)

**Пример листа персонажа**

![](seat-charactersheet.png)


**Пример извлечений корпорации**

![](seat-extractions.png)

**Пример производства корпорации**

![](seat-corpindustry.png)

**Страница настройки ролей**

![](seat-roles.png)

## Основные пакеты

Для получения **реального** исходного кода SeAT обратитесь к следующим репозиториям пакетов:  

| Имя пакета   | Версия       | Загрузки |
|----------------|:--------------|:----------|
| [api](https://github.com/eveseat/api) | [![Latest Stable Version](https://poser.pugx.org/eveseat/api/v/stable)](https://packagist.org/packages/eveseat/api) | [![Total Downloads](https://poser.pugx.org/eveseat/api/downloads)](https://packagist.org/packages/eveseat/api) |
| [eveapi](https://github.com/eveseat/eveapi) | [![Latest Stable Version](https://poser.pugx.org/eveseat/eveapi/v/stable)](https://packagist.org/packages/eveseat/eveapi) | [![Total Downloads](https://poser.pugx.org/eveseat/eveapi/downloads)](https://packagist.org/packages/eveseat/eveapi) |
| [eseye](https://github.com/eveseat/eseye) | [![Latest Stable Version](https://poser.pugx.org/eveseat/eseye/v/stable)](https://packagist.org/packages/eveseat/eseye) | [![Total Downloads](https://poser.pugx.org/eveseat/eseye/downloads)](https://packagist.org/packages/eveseat/eseye) |
| [notifications](https://github.com/eveseat/notifications) | [![Latest Stable Version](https://poser.pugx.org/eveseat/notifications/v/stable)](https://packagist.org/packages/eveseat/notifications) | [![Total Downloads](https://poser.pugx.org/eveseat/notifications/downloads)](https://packagist.org/packages/eveseat/notifications) |
| [services](https://github.com/eveseat/services) | [![Latest Stable Version](https://poser.pugx.org/eveseat/services/v/stable)](https://packagist.org/packages/eveseat/services) | [![Total Downloads](https://poser.pugx.org/eveseat/services/downloads)](https://packagist.org/packages/eveseat/services) |
| [web](https://github.com/eveseat/web) | [![Latest Stable Version](https://poser.pugx.org/eveseat/web/v/stable)](https://packagist.org/packages/eveseat/web) | [![Total Downloads](https://poser.pugx.org/eveseat/web/downloads)](https://packagist.org/packages/eveseat/web) |



# Пакеты сообщества

SeAT сам по себе предоставляет мощный доступ к данным, доступным через ESI. Однако для настройки использования этих данных и расширения функциональности SeAT существуют также различные плагины, которые можно установить и которые перечислены здесь!
<div class="grid cards" markdown>
- [:octicons-plug-16: __Community Packages__](https://eveseat.github.io/docs/community_packages/#package-list){ .esi-card-link }
</div>