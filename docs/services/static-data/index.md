---
title: Static Data
---

# Статические данные

Экспорт статических данных (SDE) содержит статические игровые данные, которые изменяются только с обновлениями игры.
Последний SDE можно найти здесь: [developers.eveonline.com/static-data/](https://developers.eveonline.com/static-data/)

## Форматы данных

SDE доступен в двух форматах:

- [JSON Lines](https://jsonlines.org/)
- [YAML](https://yaml.org/)

### JSON Lines

Ключи JSON должны быть строками.
Когда набор данных содержит целочисленные ключи, они преобразуются в формат списка, где каждая запись содержит:

- `_key`: Фактическое значение ключа.
- `_value`: Значение (когда значение не является объектом).

### YAML

YAML поддерживает целочисленные ключи, поэтому не требует специального кодирования, используемого в JSON Lines.
Обратите внимание, что чтение больших файлов YAML может быть ресурсоемким и медленным.
При работе с большими наборами данных, такими как `mapMoons` и подобные файлы, рассмотрите возможность использования формата JSON Lines.

## Схема

Вы можете найти предоставленные сообществом схемы и альтернативные форматы в разделе [ресурсы сообщества](../../community/#библиотеки-и-ресурсы).

## Изменения схемы

Изменения схемы документируются здесь: [developers.eveonline.com/static-data/tranquility/schema-changelog.yaml](https://developers.eveonline.com/static-data/tranquility/schema-changelog.yaml)

## Автоматизация

Для автоматического доступа к SDE:

- **Последний номер сборки**: [developers.eveonline.com/static-data/tranquility/latest.jsonl](https://developers.eveonline.com/static-data/tranquility/latest.jsonl).
    - Последний номер сборки находится в записи с ключом `sde`.
- **URL данных**: `https://developers.eveonline.com/static-data/tranquility/eve-online-static-data-<build-number>-<variant>.zip`.
- **Изменения**: `https://developers.eveonline.com/static-data/tranquility/changes/<build-number>.jsonl`.
    - Это содержит список изменений.
      Запись с ключом `_meta` содержит `lastBuildNumber`, ссылающийся на предыдущий SDE.

Наконец, есть несколько сокращенных URL для всегда получения последней версии.
Это перенаправит на URL с последним номером сборки.

- JSON Lines: [developers.eveonline.com/static-data/eve-online-static-data-latest-jsonl.zip](https://developers.eveonline.com/static-data/eve-online-static-data-latest-jsonl.zip)
- YAML: [developers.eveonline.com/static-data/eve-online-static-data-latest-yaml.zip](https://developers.eveonline.com/static-data/eve-online-static-data-latest-yaml.zip)

## HTTP-кеширование

Все ресурсы полностью поддерживают заголовки ETag и Last-Modified.
Ресурсы будут обновляться только при фактическом изменении.
Все нестатические файлы кешируются на 5 минут.

## Названия небесных объектов

В SDE обычно не упоминается название звезд, планет, лун, поясов астероидов и NPC-станций.
Это потому, что они могут быть выведены из названия солнечной системы и нескольких полей, связанных с небесным объектом.

Есть несколько исключений; в этих случаях небесный объект имеет поле `name` с их названием.
Во всех остальных случаях следуйте таблице ниже.

| Небесный объект                                     | Содержание                                           |
|-----------------------------------------------------|------------------------------------------------------|
| Звезды                                              | `<solarSystemName>`                                  |
| Планеты                                             | `<orbitName> <celestialIndex>`                       |
| Луны                                                | `<orbitName> - Moon <orbitIndex>`                    |
| Пояса астероидов                                    | `<orbitName> - Asteroid Belt <orbitIndex>`           |
| Станции (где `useOperationName` true)              | `<orbitName> - <corporationName> <operationName>`    |
| Станции (где `useOperationName` не true)           | `<orbitName> - <corporationName>`                    |
| Звездные врата                                      | `Stargate (<solarSystemName>)`                       |

Примечание:

- Для звезд используйте `solarSystemID` для поиска `solarSystemName` через `mapSolarSystems` (как `name`).
- `orbitName` — это название небесного объекта `orbitID`, построенное через таблицу выше.
- `celestialIndex` должен быть представлен римскими цифрами.
- Для станций используйте `ownerID` для поиска `corporationName` через `npcCorporations` (как `name`).
- Для станций используйте `operationID` для поиска `operationName` через `stationOperations`.
- Для звездных врат используйте `destination.solarSystemID` для поиска `solarSystemName` через `mapSolarSystems` (как `name`).
