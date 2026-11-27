# Rigs

Модульные костюмы RIG (Resource Integration Gear).
Всего: 40 типов костюмов (400 RSI внутри папок костюмов) + 3 общих пакета фреймов и контроллеров, всего 403 RSI (1 294 состояния, 32x32).

## Структура каталога костюма

Каждый каталог `Rigs/<suit_id>/` содержит 10 пакетов RSI:

- `icons.rsi` — иконки деталей в инвентаре (обычные и `_sealed`)
- `suit.rsi` — нагрудник на теле (`normal`, `sealed`)
- `helmet.rsi` — шлем на теле (`normal`, `sealed`)
- `gloves.rsi` — перчатки на теле (`normal`, `sealed`)
- `boots.rsi` — ботинки на теле (`normal`, `sealed`)
- `control.rsi` — блок управления на спине (`normal`, `sealed`)
- `unsealed.rsi` — полный набор слоёв в расстёгнутом виде (`control`, `suit`, `helmet`, `gloves`, `boots`)
- `sealed.rsi` — полный набор слоёв в герметичном виде (`control`, `suit`, `helmet`, `gloves`, `boots`)
- `inhand_left.rsi`, `inhand_right.rsi` — отображение контроллера в руках

Общие пакеты: [Rig_Frames.rsi](Rig_Frames.rsi), [control_inhand_left.rsi](control_inhand_left.rsi), [control_inhand_right.rsi](control_inhand_right.rsi).

## Костюмы (40)

### Инженерные и горнодобывающие (CEC)
- `standard_engineer`, `standard_engineer_anodized`, `standard_engineer_burnished`, `standard_engineer_forged`
- `intermediate_engineer`, `intermediate_engineer_anodized`, `intermediate_engineer_burnished`, `intermediate_engineer_forged`
- `advanced_engineer`, `advanced_engineer_anodized`, `advanced_engineer_burnished`, `advanced_engineer_forged`
- `legacy_standard_engineer`
- `vintage`, `heavy_vintage`
- `standard_miner`, `intermediate_miner`, `advanced_miner`, `excavation`

### Гражданские, медицинские и специальные
- `med`
- `emergency`
- `astro`
- `hacker`
- `advanced`

### Охрана и армия (PCSI / EDF / Sprawl)
- `pcsi`, `pcsi_riot`
- `security_standard`, `riot`
- `adv_soldier`, `adv_soldier_dark`, `special_forces`, `venture`, `carver`

### Экспедиционные (SCAF) и юнитологи
- `arctic_survival`, `witness`
- `scaf_elite`, `scaf_legionnaire`, `scaf_sharpshooter`
- `advanced_engineer_unitologist`, `security_standard_zealot`
