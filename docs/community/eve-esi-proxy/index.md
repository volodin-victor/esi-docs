---
search:
  exclude: true

title: EVE ESI Proxy
type: resource
description: HTTP-прокси для ESI API.
maintainer:
  name: Kenneth Jørgensen
  github: autonomouslogic
---

# EVE ESI Proxy

HTTP-прокси, специально разработанный для ESI API.

<div class="grid cards" markdown>

- [:octicons-mark-github-16: __GitHub__](https://github.com/autonomouslogic/eve-esi-proxy){ .esi-card-link }
- [:simple-discord: __Discord__](https://everef.net/discord){ .esi-card-link }

</div>

## Возможности

ESI API — отличный ресурс, но с ним может быть сложно работать.
Все перечисленные ниже функции — это вещи, о которых вы должны остро знать.
Использование этого прокси позволит вам заняться написанием вашего приложения и не беспокоиться о деталях знаний ESI.

* **Вход персонажа** поддерживается, и OAuth обрабатывается автоматически
* **Кеширование ответов** на диск для улучшения времени запросов и снижения нагрузки на сам ESI
* **Условные запросы** для обновления объектов в кеше
* **Ограничение скорости** для избежания бана, включая различные лимиты для конечных точек, имеющих специальные недокументированные ограничения
* **Обработка заголовков лимита ошибок ESI** для остановки всех запросов при достижении лимита
* **Повтор неудачных запросов** при возврате 5xx
* **Заголовок user agent** обрабатывается автоматически
* **Получение нескольких страниц параллельно**, если в запросе не установлена страница (или страница 0), объединяя все страницы в один ответ

Кеширование, ограничение скорости, повторы и т.д. обрабатываются прозрачно.

## Использование
Запуск через Docker:
```bash
docker run -it -v eve-esi-proxy:/data -p 8182:8182 -m 2g -e "ESI_USER_AGENT=<your email>" autonomouslogic/eve-esi-proxy:latest
```

Затем вы запрашиваете данные так же, как на ESI, просто с localhost:
```bash
curl "http://localhost:8182/latest/status/"
```
или
```bash
curl "http://localhost:8182/latest/markets/10000002/orders/?order_type=all"
```
