# Форматы фиттингов

Существует несколько форматов для представления фиттингов:

## EFT

EFT расшифровывается как "EVE Fitting Tool" — популярное когда-то стороннее приложение для сборки корабельных фитов.
Хотя приложение давно исчезло, используемый им формат с тех пор был принят многими инструментами и самой игрой.
Это формат, используемый при действии "Копировать в буфер обмена" в окне фиттинга в игре, и формат, ожидаемый для действия "Импорт из буфера обмена".

### Формат

1. Первая строка указывает корпус и название фиттинга в квадратных скобках, разделенные запятой
2. Модули низких слотов
3. Модули средних слотов и заряды (если доступны)
4. Модули высоких слотов и заряды (если доступны) (например, 125mm Railgun I, Antimatter Charge S)
5. Риги
6. Подсистемы
7. Сервисы (для фитов структур)
8. Дроны / файтеры в отсеке дронов/файтеров с количеством (например, Warrior II x2)
9. Предметы в трюме с количеством (например, Antimatter Charge M x42)

Разделы 2–7 разделены пустой строкой, разделы 7–9 разделены двумя пустыми строками.

Дроны и предметы в грузе могут иметь указанное количество с суффиксом ` x42` для 42 единиц, например.

Модули могут иметь суффикс `/offline`, чтобы указать, что они выключены. Однако, хотя игра импортирует эти фиты, суффикс `/offline` игнорируется. Модуль все равно будет импортирован как включенный.

Пустые слоты обозначаются как `[Empty <name> slot]`, где `<name>` — это одно из `low`, `med`, `high`, `rig`, `service`, однако это не присутствует при экспорте из игры, но все равно считается допустимым при импорте.

Названия типов могут быть указаны в любом локализованном формате, а не только на английском.

### Пример

```
[Heron Navy Issue, Deepflow Rift Dredger]
Inertial Stabilizers II
Inertial Stabilizers II /offline

Scan Pinpointing Array II
Scan Rangefinding Array II
Scan Acquisition Array II
Compact EM Shield Amplifier
Compact Thermal Shield Amplifier

Small Tractor Beam II
Small Tractor Beam II
Core Probe Launcher II
Improved Cloaking Device II

Small Gravity Capacitor Upgrade II
Small Core Defense Field Extender I




Sisters Core Scanner Probe x8
```

## DNA

Ship DNA — это компактный формат, описывающий фит в одной строке.
Это формат, используемый при создании ссылок на фиты в чате в игре.

### Формат

Формальная грамматика выглядит следующим образом:

```
DNA -> SHIP ':' HIGHS ':' MEDS ':' LOWS ':' RIGS ':' CHARGES
SHIP -> SHIP_TYPE_ID ( ':' SUBSYSTEM_ID ':' SUBSYSTEM_ID ':' SUBSYSTEM_ID ':' SUBSYSTEM_ID ':' SUBSYSTEM_ID )
HIGHS -> EMPTY | MODULE ( ':' MODULE )
MEDS -> EMPTY | MODULE ( ':' MODULE )
LOWS -> EMPTY | MODULE ( ':' MODULE )
RIGS -> EMPTY | MODULE ( ':' MODULE )
CHARGES -> EMPTY | CHARGE ( ':' CHARGE )
MODULE -> MODULE_ID ( '_' ) ';' QUANTITY
CHARGE -> CHARGE_ID ';' QUANTITY
SHIP_TYPE_ID -> typeID корабля
SUBSYSTEM_ID -> typeID установленных подсистем
MODULE_ID -> typeID установленного модуля
CHARGE_ID -> typeID заряда или дрона
QUANTITY -> целое число, количество типа
```

ID модулей могут сопровождаться символом подчеркивания, чтобы указать, что они не установлены. Заряды всегда считаются неустановленными.

### Пример

`72904:4250;2:4258;1:11577;1:33199;1:33201;1:33197;1:9580;1:9568;1:1405;2:31220;1:31788;1:30488;8::`

Как ссылка в чате:
`<url=fitting:72904:4250;2:4258;1:11577;1:33199;1:33201;1:33197;1:9580;1:9568;1:1405;2:31220;1:31788;1:30488;8::>Deepflow Rift Dredger</url>`

## XML

Это формат, используемый при экспорте фитов в файл в игре или импорте из файла. Формат поддерживает несколько фитов в одной структуре данных.

### Пример

```xml
<?xml version="1.0" ?>
<fittings>
    <fitting name="Deepflow Rift Dredger">
        <description value=""/>
        <shipType value="Heron Navy Issue"/>
        <hardware slot="low slot 0" type="Inertial Stabilizers II"/>
        <hardware slot="low slot 1" type="Inertial Stabilizers II"/>
        <hardware slot="hi slot 0" type="Small Tractor Beam II"/>
        <hardware slot="hi slot 1" type="Small Tractor Beam II"/>
        <hardware slot="hi slot 2" type="Core Probe Launcher II"/>
        <hardware slot="med slot 4" type="Compact Thermal Shield Amplifier"/>
        <hardware slot="med slot 3" type="Compact EM Shield Amplifier"/>
        <hardware slot="hi slot 3" type="Improved Cloaking Device II"/>
        <hardware qty="8" slot="cargo" type="Sisters Core Scanner Probe"/>
        <hardware slot="rig slot 0" type="Small Gravity Capacitor Upgrade II"/>
        <hardware slot="rig slot 1" type="Small Core Defense Field Extender I"/>
        <hardware slot="med slot 2" type="Scan Acquisition Array II"/>
        <hardware slot="med slot 0" type="Scan Pinpointing Array II"/>
        <hardware slot="med slot 1" type="Scan Rangefinding Array II"/>
    </fitting>
</fittings>
```
