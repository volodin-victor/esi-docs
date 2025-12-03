---
search:
  exclude: true

title: EVE API for TypeScript
type: resource
description: Клиентская библиотека TypeScript для API EVE Online (ESI).
maintainer:
  name: Leigh Griffin
  github: lgriffin
---

# ESI.ts

[![npm version](https://badge.fury.io/js/%40lgriffin%2Fesi.ts.svg)](https://badge.fury.io/js/%40lgriffin%2Fesi.ts)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.5%2B-blue)](https://www.typescriptlang.org/)

Современная типобезопасная реализация TypeScript для [EVE Online ESI API](https://esi.evetech.net/). Построена на принципах чистой архитектуры, с комплексной обработкой ошибок и обширным тестированием.

## 🚀 Возможности

- **Типобезопасность**: Полная поддержка TypeScript с комплексными определениями типов
- **Чистая архитектура**: Разделение ответственности с внедрением зависимостей
- **Отказоустойчивость**: Встроенная обработка ошибок, логика повторных попыток и автоматические выключатели
- **Высокая производительность**: Интеллектуальное кеширование ETag для оптимального использования пропускной способности
- **Тестируемость**: Обширное покрытие тестами со сценариями BDD
- **Современность**: Использует новейшие возможности TypeScript и лучшие практики
- **Полнота**: Покрывает все конечные точки ESI API с организованной структурой клиента

## 📦 Установка

```bash
npm install @lgriffin/esi.ts
```

## 🔧 Начало работы

ESI.ts предлагает несколько способов использования API в зависимости от ваших потребностей:

### 1. Полный ESI-клиент (Все API)

Полный `EsiClient` предоставляет доступ ко всем конечным точкам ESI:

```typescript
import { EsiClient } from '@lgriffin/esi.ts';

// Полный клиент со всеми доступными API
const client = new EsiClient({
  clientId: 'your-app-name',
  accessToken: 'your-access-token', // Опционально - требуется для аутентифицированных конечных точек
  timeout: 30000,                   // Опционально - таймаут запроса в мс
  retryAttempts: 3                  // Опционально - количество попыток повтора
});
```

### 2. Пользовательский облегчённый клиент (Выбранные API)

Создайте облегчённый клиент только с нужными вам API:

```typescript
import { CustomEsiClient } from '@lgriffin/esi.ts';

// Облегчённый клиент только с определёнными API
const customClient = new CustomEsiClient({
  clientId: 'my-trading-bot',
  clients: ['characters', 'market', 'universe'] // Загружайте только то, что вам нужно
});

// Доступ к выбранным вами API
const character = await customClient.characters?.getCharacterPublicInfo(123456);
const prices = await customClient.market?.getMarketPrices();
```

### 3. Паттерн Builder для пользовательских клиентов

Используйте паттерн Builder для более читаемого построения клиента:

```typescript
import { EsiClientBuilder } from '@lgriffin/esi.ts';

// Построение пользовательского клиента шаг за шагом
const client = new EsiClientBuilder()
  .addClient('characters')
  .addClient('corporations')
  .addClients(['market', 'universe'])
  .withClientId('my-corp-manager')
  .withAccessToken('your-token')
  .build();
```

### 4. Отдельные API-клиенты (Сверхлёгкий вариант)

Создавайте автономные клиенты для отдельных групп API:

```typescript
import { EsiApiFactory } from '@lgriffin/esi.ts';

// Только API персонажей
const characterClient = EsiApiFactory.createCharacterClient({
  clientId: 'character-lookup-tool'
});

const character = await characterClient.getCharacterPublicInfo(123456);

// Только API рынка
const marketClient = EsiApiFactory.createMarketClient({
  clientId: 'market-analyzer'
});

const prices = await marketClient.getMarketPrices();
```

### 5. Прямое создание экземпляров API-классов

Для максимального контроля создавайте экземпляры API-клиентов напрямую:

```typescript
import { CharacterClient, ApiClient, ApiClientBuilder } from '@lgriffin/esi.ts';

// Создание базового API-клиента
const apiClient = new ApiClientBuilder()
  .withClientId('direct-api-client')
  .withBaseUrl('https://esi.evetech.net')
  .build();

// Создание клиента персонажей напрямую
const characterClient = new CharacterClient(apiClient);
const character = await characterClient.getCharacterPublicInfo(123456);
```

## 📊 Архитектура клиента

### Доступные типы клиентов

Все перечисленные выше подходы предоставляют доступ к следующим организованным API-клиентам:

```typescript
// Доступные клиенты:
client.alliance      // Информация об альянсах
client.characters    // Данные персонажей
client.corporations  // Управление корпорациями
client.market        // Рыночные данные и торговля
client.universe      // Информация о вселенной (системы, станции, предметы)
client.fleets        // Управление флотами
client.industry      // Производство и индустрия
client.mail          // Внутриигровая почта
client.contacts      // Управление контактами
client.assets        // Управление активами
client.wallet        // Операции с кошельком
client.killmails     // Данные киллмейлов
client.location      // Местоположение персонажа
client.skills        // Навыки персонажа (если доступны)
client.factions      // Фракционная война
client.wars          // Информация о войнах
client.sovereignty   // Данные о суверенитете
client.incursions    // Информация о вторжениях
client.opportunities // Система возможностей
client.fittings      // Сборки кораблей
client.clones        // Управление клонами
client.loyalty       // Очки лояльности
client.bookmarks     // Управление закладками
client.calendar      // Календарные события
client.contracts     // Система контрактов
client.insurance     // Информация о страховании
client.route         // Планирование маршрутов
client.search        // Функция поиска
client.status        // Статус сервера
client.ui            // Взаимодействие с UI
```

## 🎯 Выбор правильного подхода

### Когда использовать каждый метод

| Подход | Лучше всего для | Использование памяти | Время запуска |
|----------|----------|--------------|--------------|
| **Full EsiClient** | Полные приложения, использование нескольких API | Высокое | Медленнее |
| **CustomEsiClient** | Сфокусированные приложения, выбранные API | Среднее | Среднее |
| **EsiApiFactory** | Инструменты одного назначения, микросервисы | Низкое | Быстро |
| **Direct Instantiation** | Библиотеки, встроенное использование | Минимальное | Быстрее всего |

### Практические примеры по случаям использования

#### Инструмент поиска персонажей (Сверхлёгкий вариант)

```typescript
import { EsiApiFactory } from '@lgriffin/esi.ts';

const characterClient = EsiApiFactory.createCharacterClient({
  clientId: 'character-lookup-v1'
});

// Только операции с персонажами
const character = await characterClient.getCharacterPublicInfo(123456);
const portrait = await characterClient.getCharacterPortrait(123456);
console.log(`${character.body.name} - ${portrait.body.px128x128}`);
```

#### Торговый бот (Выбранные API)

```typescript
import { EsiClientBuilder } from '@lgriffin/esi.ts';

const tradingBot = new EsiClientBuilder()
  .addClients(['market', 'characters', 'universe', 'wallet'])
  .withClientId('trading-bot-v2')
  .withAccessToken(process.env.EVE_ACCESS_TOKEN)
  .build();

// Загружаются только нужные вам API
const prices = await tradingBot.market?.getMarketPrices();
const wallet = await tradingBot.wallet?.getCharacterWallet(characterId);
```

#### Панель управления корпорацией (Пользовательский клиент)

```typescript
import { CustomEsiClient } from '@lgriffin/esi.ts';

const corpManager = new CustomEsiClient({
  clientId: 'corp-dashboard',
  accessToken: directorToken,
  clients: ['corporations', 'characters', 'assets', 'wallet', 'mail']
});

// Эффективное управление корпорацией только с нужными API
const corp = await corpManager.corporations?.getCorporationInfo(corpId);
const members = await corpManager.corporations?.getCorporationMembers(corpId);
```

## 📋 Типичные паттерны использования

### Публичные данные (Аутентификация не требуется)

```typescript
// Получить информацию об альянсе
const alliance = await client.alliance.getAllianceById(99005338);
console.log(`Alliance: ${alliance.name} [${alliance.ticker}]`);

// Получить публичную информацию о персонаже
const character = await client.characters.getCharacterPublicInfo(1689391488);
console.log(`Character: ${character.name}`);

// Получить информацию о корпорации
const corporation = await client.corporations.getCorporationInfo(98742334);
console.log(`Corporation: ${corporation.name} [${corporation.ticker}]`);

// Получить рыночные цены
const prices = await client.market.getMarketPrices();
console.log(`Found ${prices.length} market prices`);

// Получить информацию о солнечной системе
const system = await client.universe.getSystemById(30000142);
console.log(`System: ${system.name} (Security: ${system.security_status})`);
```

### Аутентифицированные данные (Требуется токен доступа)

```typescript
// Инициализация с токеном доступа
const authenticatedClient = new EsiClient({
  clientId: 'your-app-name',
  accessToken: 'your-character-access-token'
});

const characterId = 1689391488;

// Получить активы персонажа
const assets = await authenticatedClient.assets.getCharacterAssets(characterId);
console.log(`Character has ${assets.length} assets`);

// Получить баланс кошелька персонажа
const wallet = await authenticatedClient.wallet.getCharacterWallet(characterId);
console.log(`Wallet balance: ${wallet.toLocaleString()} ISK`);

// Получить почту персонажа
const mail = await authenticatedClient.mail.getCharacterMail(characterId);
console.log(`Character has ${mail.length} mail messages`);

// Получить рыночные заказы персонажа
const orders = await authenticatedClient.market.getCharacterOrders(characterId);
console.log(`Character has ${orders.length} active market orders`);
```

### Сложные рабочие процессы

```typescript
// Сборка профиля персонажа
async function getCompleteCharacterProfile(characterId: number) {
  const [character, portrait, corporation, location] = await Promise.all([
    client.characters.getCharacterPublicInfo(characterId),
    client.characters.getCharacterPortrait(characterId),
    client.characters.getCharacterPublicInfo(characterId).then(char => 
      client.corporations.getCorporationInfo(char.corporation_id)
    ),
    client.location.getCharacterLocation(characterId)
  ]);

  return {
    character,
    portrait,
    corporation,
    location
  };
}

// Анализ рынка
async function analyzeMarketData(regionId: number, typeId: number) {
  const [prices, orders, history] = await Promise.all([
    client.market.getMarketPrices(),
    client.market.getMarketOrders(regionId, { type_id: typeId }),
    client.market.getMarketHistory(regionId, typeId)
  ]);

  const currentPrice = prices.find(p => p.type_id === typeId)?.average_price;
  const buyOrders = orders.filter(o => o.is_buy_order);
  const sellOrders = orders.filter(o => !o.is_buy_order);

  return {
    currentPrice,
    bestBuyPrice: Math.max(...buyOrders.map(o => o.price)),
    bestSellPrice: Math.min(...sellOrders.map(o => o.price)),
    dailyVolume: history[0]?.volume || 0
  };
}
```

## 📊 Обработка ошибок

Библиотека предоставляет комплексную обработку ошибок с конкретными типами ошибок:

```typescript
import { ApiError, ApiErrorType } from '@lgriffin/esi.ts';

try {
  const alliance = await client.alliance.getAllianceById(99999999); // Неверный ID
} catch (error) {
  if (error instanceof ApiError) {
    switch (error.type) {
      case ApiErrorType.NOT_FOUND:
        console.log('Альянс не найден');
        break;
      case ApiErrorType.RATE_LIMITED:
        console.log('Ограничение скорости - повторить после:', error.retryAfter);
        break;
      case ApiErrorType.SERVER_ERROR:
        console.log('Ошибка сервера ESI:', error.statusCode);
        break;
      case ApiErrorType.NETWORK_ERROR:
        console.log('Проблема с сетевым подключением');
        break;
      case ApiErrorType.AUTHENTICATION_ERROR:
        console.log('Неверный или истёкший токен доступа');
        break;
      default:
        console.log('Неожиданная ошибка:', error.message);
    }
  }
}
```

### Корректная обработка ошибок в сложных рабочих процессах

```typescript
async function safeCharacterLookup(characterId: number) {
  try {
    // Использование Promise.allSettled для сценариев частичного успеха
    const results = await Promise.allSettled([
      client.characters.getCharacterPublicInfo(characterId),
      client.characters.getCharacterPortrait(characterId),
      client.location.getCharacterLocation(characterId)
    ]);

    const profile: any = {};

    if (results[0].status === 'fulfilled') {
      profile.character = results[0].value;
    }
    
    if (results[1].status === 'fulfilled') {
      profile.portrait = results[1].value;
    }
    
    if (results[2].status === 'fulfilled') {
      profile.location = results[2].value;
    } else if (results[2].status === 'rejected') {
      console.log('Местоположение недоступно (персонаж может быть оффлайн)');
    }

    return profile;
  } catch (error) {
    console.error('Не удалось получить данные персонажа:', error);
    return null;
  }
}
```

## ⚡ Производительность и кеширование

### Интеллектуальное кеширование ETag

ESI.ts включает сложную систему кеширования ETag, которая автоматически оптимизирует API-вызовы, избегая ненужных передач данных. Эта функция **включена по умолчанию** и работает прозрачно со всеми GET-запросами.

#### Как работает кеширование ETag

ETags (Entity Tags) — это уникальные идентификаторы, возвращаемые серверами ESI, которые представляют текущую версию ресурса. Когда данные не изменились, сервер возвращает статус `304 Not Modified` вместо полных данных, значительно снижая использование пропускной способности и улучшая время отклика.

#### Базовое использование (Автоматическое)

```typescript
import { EsiClient } from '@lgriffin/esi.ts';

// Кеширование ETag включено по умолчанию
const client = new EsiClient({
  clientId: 'my-eve-app'
});

// Первый вызов - загружает и кеширует данные
const alliances1 = await client.alliance.getAlliances();

// Второй вызов - возвращает кешированные данные, если они не изменились (ответ 304)
const alliances2 = await client.alliance.getAlliances(); // ⚡ Очень быстро!
```

#### Пользовательская конфигурация кеша

```typescript
const client = new EsiClient({
  clientId: 'my-eve-app',
  enableETagCache: true, // По умолчанию: true
  etagCacheConfig: {
    maxEntries: 1000,      // Максимальное количество кешированных ответов (по умолчанию: 1000)
    defaultTtl: 300000,    // TTL кеша в мс (по умолчанию: 5 минут)
    cleanupInterval: 60000, // Частота очистки (по умолчанию: 1 минута)
    persistToStorage: true, // Сохранять в localStorage (по умолчанию: false)
    storageKey: 'my-esi-cache' // Пользовательский ключ хранилища
  }
});
```

#### Управление кешем

```typescript
// Получить статистику кеша
const stats = client.getCacheStats();
console.log(`Cache: ${stats.totalEntries}/${stats.maxEntries} entries`);
console.log(`Оптимизация процента попаданий: ${stats.hitRate}%`);

// Очистить кеш вручную
client.clearCache();

// Обновить настройки кеша во время выполнения
client.updateCacheConfig({
  maxEntries: 2000,
  defaultTtl: 600000 // 10 минут
});

// Отключить кеширование для конкретных случаев использования
const client = new EsiClient({
  enableETagCache: false // Полностью отключить кеширование
});
```

#### Преимущества производительности

- **🚀 Более быстрое время отклика**: Кешированные ответы возвращаются мгновенно
- **📉 Снижение использования пропускной способности**: Избегание загрузки неизменённых данных
- **🔋 Дружелюбность к серверу**: Снижение нагрузки на серверы ESI
- **💰 Экономичность**: Меньшее использование данных для мобильных/ограниченных подключений
- **🎯 Умное кеширование**: Кешируются только GET-запросы с ETags

#### Поведение кеша

| Сценарий | Поведение | Влияние на производительность |
|----------|----------|-------------------|
| Первый API-вызов | Загружает данные, сохраняет ETag | Обычная скорость |
| Данные не изменились | Возвращает кешированные данные (304) | ⚡ **~95% быстрее** |
| Данные изменились | Загружает новые данные, обновляет кеш | Обычная скорость |
| Кеш истёк | Загружает свежие данные | Обычная скорость |
| Кеш заполнен | Автоматически удаляет самые старые записи | Минимальное влияние |

#### Расширенные возможности ETag

```typescript
// Мониторинг производительности кеша
client.on('cacheHit', (url, etag) => {
  console.log(`Попадание в кеш для ${url} с ETag ${etag}`);
});

client.on('cacheMiss', (url) => {
  console.log(`Промах кеша для ${url} - загрузка свежих данных`);
});

// Программная проверка кеша
const cache = client.getETagCache();
if (cache) {
  const entry = cache.get('https://esi.evetech.net/latest/alliances');
  if (entry) {
    console.log(`Возраст кешированных данных: ${Date.now() - entry.timestamp}мс`);
    console.log(`ETag: ${entry.etag}`);
  }
}
```

#### Когда кеширование ETag помогает больше всего

- **📊 Рыночные данные**: Списки цен, которые обновляются периодически
- **🏢 Информация о корпорациях/альянсах**: Относительно статические организационные данные  
- **🌌 Данные вселенной**: Информация о солнечных системах, станциях и типах
- **👥 Списки персонажей**: Реестры членов и публичная информация
- **📈 Статистика**: Агрегированные данные, которые обновляются с интервалами

#### Детали реализации

- **Архитектура**: Реализовано на уровне основного `ApiRequestHandler`
- **Область действия**: Работает со ВСЕМИ GET-запросами автоматически
- **Совместимость**: Полностью обратно совместимо — существующий код работает без изменений
- **Потокобезопасность**: Использует атомарные операции для управления кешем
- **Эффективное использование памяти**: Автоматическая очистка и управление размером
- **Варианты хранения**: В памяти (по умолчанию) или постоянное localStorage

## 🔧 Расширенная конфигурация

### Пользовательские таймауты и логика повторных попыток

```typescript
const client = new EsiClient({
  clientId: 'my-eve-app',
  timeout: 60000,      // Таймаут 60 секунд
  retryAttempts: 5,    // Повторять до 5 раз
  baseUrl: 'https://esi.evetech.net' // Пользовательская конечная точка ESI (опционально)
});
```

### Использование переменных окружения

```typescript
// Установить переменные окружения
// ESI_CLIENT_ID=your-app-name
// ESI_ACCESS_TOKEN=your-token
// ESI_TIMEOUT=30000

const client = new EsiClient({
  clientId: process.env.ESI_CLIENT_ID,
  accessToken: process.env.ESI_ACCESS_TOKEN,
  timeout: parseInt(process.env.ESI_TIMEOUT || '30000')
});
```

## 🚀 Примеры из реального мира

### Торговый бот EVE Market (Облегчённая версия)

```typescript
import { EsiClientBuilder } from '@lgriffin/esi.ts';

class MarketBot {
  private client: any; // CustomEsiClient

  constructor(accessToken: string) {
    // Загружаем только действительно нужные нам API
    this.client = new EsiClientBuilder()
      .addClients(['market', 'universe'])
      .withClientId('market-bot-v1')
      .withAccessToken(accessToken)
      .build();
  }

  async findArbitrageOpportunities(regionId: number, typeId: number) {
    try {
      const [orders, history] = await Promise.all([
        this.client.market.getMarketOrders(regionId, { type_id: typeId }),
        this.client.market.getMarketHistory(regionId, typeId)
      ]);

      const buyOrders = orders.filter(o => o.is_buy_order).sort((a, b) => b.price - a.price);
      const sellOrders = orders.filter(o => !o.is_buy_order).sort((a, b) => a.price - b.price);

      if (buyOrders.length > 0 && sellOrders.length > 0) {
        const spread = buyOrders[0].price - sellOrders[0].price;
        const spreadPercent = (spread / sellOrders[0].price) * 100;

        return {
          profitable: spread > 0,
          spread,
          spreadPercent,
          bestBuy: buyOrders[0],
          bestSell: sellOrders[0],
          dailyVolume: history[0]?.volume || 0
        };
      }

      return null;
    } catch (error) {
      console.error('Не удалось проанализировать рынок:', error);
      return null;
    }
  }
}
```

### Панель управления корпорацией (Пользовательский клиент)

```typescript
import { CustomEsiClient } from '@lgriffin/esi.ts';

class CorporationManager {
  private client: CustomEsiClient;

  constructor(accessToken: string) {
    // Загружаем только API, связанные с корпорациями
    this.client = new CustomEsiClient({
      clientId: 'corp-manager',
      accessToken,
      clients: ['corporations', 'characters', 'wallet']
    });
  }

  async getCorporationOverview(corporationId: number) {
    try {
      const [corp, members, wallets] = await Promise.all([
        this.client.corporations.getCorporationInfo(corporationId),
        this.client.corporations.getCorporationMembers(corporationId),
        this.client.wallet.getCorporationWallets(corporationId)
      ]);

      return {
        corporation: corp,
        memberCount: members.length,
        totalBalance: wallets.reduce((sum, wallet) => sum + wallet.balance, 0)
      };
    } catch (error) {
      if (error instanceof ApiError && error.type === ApiErrorType.AUTHENTICATION_ERROR) {
        throw new Error('Недостаточно прав для доступа к данным корпорации');
      }
      throw error;
    }
  }
}
```

### Простой поиск персонажа (Прямой API)

```typescript
import { EsiApiFactory } from '@lgriffin/esi.ts';

// Сверхлёгкий вариант: только один API, одна функция
async function lookupCharacter(characterId: number) {
  const characterClient = EsiApiFactory.createCharacterClient({
    clientId: 'simple-lookup'
  });

  const character = await characterClient.getCharacterPublicInfo(characterId);
  return character.body.name;
}

// Использование
const name = await lookupCharacter(1689391488);
console.log(name); // "deiseman"
```

### Использование API-классов напрямую

```typescript
import { CharacterClient, ApiClientBuilder } from '@lgriffin/esi.ts';

// Максимальный контроль - создайте именно то, что вам нужно
const apiClient = new ApiClientBuilder()
  .setClientId('direct-usage')
  .setLink('https://esi.evetech.net')
  .build();

const characterClient = new CharacterClient(apiClient);

// Прямое использование без обёртки
const character = await characterClient.getCharacterPublicInfo(123456);
const portrait = await characterClient.getCharacterPortrait(123456);
```

### Пример микросервиса (Единственная ответственность)

```typescript
import { EsiApiFactory } from '@lgriffin/esi.ts';

// Микросервис, которому нужны только рыночные данные
class PriceService {
  private marketClient;

  constructor() {
    // Загружаем только то, что нужно этому сервису
    this.marketClient = EsiApiFactory.createMarketClient({
      clientId: 'price-service-v1'
    });
  }

  async getCurrentPrice(typeId: number): Promise<number> {
    const prices = await this.marketClient.getMarketPrices();
    const price = prices.body.find((p: any) => p.type_id === typeId);
    return price?.average_price || 0;
  }

  async getBestPrices(regionId: number, typeId: number) {
    const orders = await this.marketClient.getMarketOrders(regionId, { type_id: typeId });
    
    const buyOrders = orders.body.filter((o: any) => o.is_buy_order);
    const sellOrders = orders.body.filter((o: any) => !o.is_buy_order);
    
    return {
      bestBuy: Math.max(...buyOrders.map((o: any) => o.price)),
      bestSell: Math.min(...sellOrders.map((o: any) => o.price))
    };
  }
}
```

## 🧪 Тестирование

### Запуск тестов

```bash
# Запустить модульные тесты
npm test

# Запустить модульные тесты с покрытием
npm run coverage

# Запустить BDD тесты (поведенческие сценарии)
npm run bdd

# Запустить конкретные наборы BDD тестов
npm run bdd:alliance
npm run bdd:character
npm run bdd:market

# Запустить все тесты
npm run test:all
```

## 🚀 Рабочие примеры

### Попробуйте примеры

ESI.ts включает рабочие примеры, демонстрирующие реальное использование API:

```bash
# Запустить полный пример профиля персонажа
npm run example

# Запустить примеры гибкого использования API (все 5 подходов)
npm run examples:flexible
```

### Пример профиля персонажа

Основной пример (`npm run example`) демонстрирует:
- ✅ Полную сборку профиля персонажа
- ✅ Параллельные API-вызовы для эффективности
- ✅ Обработку ошибок и корректную деградацию
- ✅ Очистку ресурсов
- ✅ Замер производительности

**Пример вывода:**
```
🚀 ESI.ts Character Profile Example
=====================================

🔍 Gathering complete profile for character ID: 1689391488
📋 Fetching basic character information...
🚀 Fetching detailed profile data in parallel...

============================================================
🎯 CHARACTER PROFILE SUMMARY
============================================================
👤 Name: deiseman
🆔 Character ID: 1689391488
🎂 Birthday: 2/3/2008
⚖️  Security Status: 0.16

🏢 Corporation: Brittas Empire [BREMP]
👥 Members: 360
🤝 Alliance: Pandemic Horde [REKTD]
📊 Founded: 2/4/2015

🖼️  Portrait URLs:
   📱 64x64: https://images.evetech.net/characters/1689391488/portrait?tenant=tranquility&size=64
   🖥️  128x128: https://images.evetech.net/characters/1689391488/portrait?tenant=tranquility&size=128
   🖼️  256x256: https://images.evetech.net/characters/1689391488/portrait?tenant=tranquility&size=256
   📺 512x512: https://images.evetech.net/characters/1689391488/portrait?tenant=tranquility&size=512

📍 Current Location: Unavailable (character may be offline)
============================================================

⏱️  Total execution time: 154ms
✅ Character profile retrieved successfully!
```

### Примеры гибкого использования API

Примеры гибкого использования (`npm run examples:flexible`) демонстрируют:
- ✅ Полный ESI-клиент (все API)
- ✅ Пользовательский облегчённый клиент (выбранные API)
- ✅ Использование паттерна Builder
- ✅ Отдельные API-клиенты
- ✅ Прямое создание экземпляров API-классов
- ✅ Сравнение производительности
- ✅ Пример микросервиса

**Пример вывода:**
```
🚀 ESI.ts Flexible API Usage Examples
=====================================

1️⃣  Full ESI Client (All APIs)
✅ Character: deiseman (using full client)

2️⃣  Custom Lightweight Client (Selected APIs)
✅ Character: deiseman (using custom client)
📊 Enabled clients: characters, corporations

3️⃣  Builder Pattern
✅ Character: deiseman (using builder pattern)

4️⃣  Individual API Client (Ultra Lightweight)
✅ Character: deiseman (using standalone client)

5️⃣  Direct API Class Instantiation
✅ Character: deiseman (using direct instantiation)

🎯 Performance Comparison
=========================
⏱️  Startup time comparison:
   Full Client: 1ms
   Custom Client (1 API): 0ms
   Individual Client: 0ms

💰 Microservice Example: Price Service
======================================
💎 Tritanium average price: 3.78 ISK
```

### Файлы примеров

| Файл | Назначение | Команда |
|------|---------|---------|
| `src/index.ts` | Сборка профиля персонажа | `npm run example` |
| `demo/flexible-examples.ts` | Все гибкие паттерны использования API | `npm run examples:flexible` |

### Путь обучения

1. **Начните здесь**: Запустите `npm run example`, чтобы увидеть полный рабочий процесс из реального мира
2. **Изучите варианты**: Запустите `npm run examples:flexible`, чтобы увидеть все различные способы использования API
3. **Выберите подход**: Выберите метод, который лучше всего подходит для вашего случая использования
4. **Создайте приложение**: Используйте примеры как шаблоны для своего приложения

### Тестирование ваших приложений

```typescript
import { EsiClient } from '@lgriffin/esi.ts';
import { TestDataFactory } from '@lgriffin/esi.ts';

describe('My EVE Application', () => {
  let client: EsiClient;

  beforeEach(() => {
    client = new EsiClient({
      clientId: 'test-client'
    });
  });

  afterEach(async () => {
    await client.shutdown();
  });

  it('should handle character lookup', async () => {
    // Мок-данные для тестирования
    jest.spyOn(client.characters, 'getCharacterPublicInfo')
      .mockResolvedValue(TestDataFactory.createCharacterInfo({
        character_id: 123456,
        name: 'Test Character'
      }));

    const character = await client.characters.getCharacterPublicInfo(123456);
    expect(character.name).toBe('Test Character');
  });
});
```

## 🛠️ Управление ресурсами

### Корректная очистка

```typescript
// Всегда очищайте ресурсы после завершения
async function myApplication() {
  const client = new EsiClient({
    clientId: 'my-app'
  });

  try {
    // Ваша логика приложения здесь
    const alliance = await client.alliance.getAllianceById(99005338);
    console.log(alliance.name);
  } finally {
    // Важно: всегда завершайте работу клиента
    await client.shutdown();
  }
}

// Или используйте паттерн try-with-resources
class EsiClientManager {
  private client: EsiClient;

  constructor(config: any) {
    this.client = new EsiClient(config);
  }

  async use<T>(callback: (client: EsiClient) => Promise<T>): Promise<T> {
    try {
      return await callback(this.client);
    } finally {
      await this.client.shutdown();
    }
  }
}

// Использование
const manager = new EsiClientManager({ clientId: 'my-app' });
const result = await manager.use(async (client) => {
  return await client.alliance.getAllianceById(99005338);
});
```

## 🤝 Участие в разработке

1. Форкните репозиторий
2. Создайте ветку с новой функцией
3. Напишите тесты для ваших изменений
4. Убедитесь, что все тесты проходят: `npm test && npm run bdd`
5. Откройте Pull Request

## 📄 Лицензия

GPL-3.0-or-later - см. файл [LICENSE](LICENSE) для подробностей.

---

**Приятного программирования, капсулёры! o7**
