---
title: Image Server
---
# Сервер изображений EVE (EIS)

Сервер изображений EVE предоставляет способ получения/использования изображений из EVE Online в ваших приложениях.

## Изображения

Доступ к серверу изображений можно получить по следующему URL: `https://images.evetech.net/{category}/{id}/{variation}` со следующими параметрами:

- `{category}`: Категория изображения, которое вы хотите получить. Может быть одной из следующих:
    - `alliances` (альянсы)
    - `characters` (персонажи)
    - `corporations` (корпорации)
    - `types` (типы)
- `{id}`: ID `{category}`, для которого вы хотите получить изображение.
- `{variation}`: Вариация изображения, которую вы хотите получить.
  Если вы не укажете вариацию, сервер вернет JSON-массив доступных вариаций для данных `{category}` и `{id}`.
  В общем, альянсы и корпорации будут иметь вариацию `logo`, персонажи — вариацию `portrait`.
  Типы будут иметь вариации в зависимости от того, что это за тип.

### Параметры запроса

Поддерживаются два параметра запроса: `size` и `tenant`.

Допустимые значения для параметра `size` включают степени двойки в диапазоне от 32 до 1024.
Если этот параметр не указан, сервер вернет изображение в его исходном размере.

Параметр `tenant` определяет сервер, для которого запрашиваются изображения. По умолчанию `tranquility`, но также принимает `singularity`.

### Примечания

- Логотипы NPC-фракций доступны в категории `corporations`, используя их ID фракции.
- ID 1 можно использовать с альянсами, корпорациями и персонажами для получения логотипа/портрета по умолчанию.
- Изображения возвращаются в формате PNG, за исключением портретов персонажей, которые возвращаются в формате JPEG.
- Вы можете направлять ваши клиенты и приложения напрямую к сервису изображений и использовать его как CDN. Вам не нужно кешировать изображения локально.

## Примеры

|                 Категория | Вариация  | Пример                                                                                |
| ------------------------: | --------- | ------------------------------------------------------------------------------------- |
|                  Альянс   | Logo      | [![Alliance Logo](https://images.evetech.net/alliances/99011477/logo?size=64)](https://images.evetech.net/alliances/99011477/logo?size=64)                |
|               Корпорация  | Logo      | [![Corporation Logo](https://images.evetech.net/corporations/1686954550/logo?size=64)](https://images.evetech.net/corporations/1686954550/logo?size=64)   |
| Корпорация (NPC-фракция)  | Logo      | [![Corporation Logo](https://images.evetech.net/corporations/500001/logo?size=64)](https://images.evetech.net/corporations/500001/logo?size=64)           |
|                 Персонаж  | Portrait  | [![Character Portrait](https://images.evetech.net/characters/91072482/portrait?size=64)](https://images.evetech.net/characters/91072482/portrait?size=64) |
|                      Тип  | Render    | [![Type Render](https://images.evetech.net/types/22456/render?size=64)](https://images.evetech.net/types/22456/render?size=64)                            |
|                      Тип  | Icon      | [![Type Render](https://images.evetech.net/types/22456/icon?size=64)](https://images.evetech.net/types/22456/icon?size=64)                                |
|                      Тип  | BPO       | [![Type Render](https://images.evetech.net/types/11568/bp?size=64)](https://images.evetech.net/types/11568/bp?size=64)                                    |
|                      Тип  | BPC       | [![Type Render](https://images.evetech.net/types/11568/bpc?size=64)](https://images.evetech.net/types/11568/bpc?size=64)                                  |
|                      Тип  | Relic     | [![Type Render](https://images.evetech.net/types/30752/relic?size=64)](https://images.evetech.net/types/30752/relic?size=64)                              |
