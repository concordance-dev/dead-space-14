# Правила добавления ассетов

Репозиторий содержит только графические и звуковые ассеты по вселенной Dead Space. Прототипы YAML, код и сторонние шуточные предметы сюда не добавляются.

## Графика (RSI)

- Формат: RSI версии `1` (`meta.json` с `size: {x, y}` и корректной сеткой кадров PNG, кратной заданному размеру).
- Недопустимы пустые имена состояний (`""`), пустые заглушки и вложенные `.rsi` внутри `.rsi`.
- Для каждого костюма в `Rigs/<suit>/icons.rsi` обязательны 10 состояний: `control`, `control_sealed`, `suit`, `suit_sealed`, `helmet`, `helmet_sealed`, `gloves`, `gloves_sealed`, `boots`, `boots_sealed`.
- Только канон Dead Space (костюмы, некроморфы, оружие, окружение и интерфейс серии).

## Аудио (`.ogg`)

- Кодек: `libvorbis` (Ogg Vorbis), частота дискретизации `44100 Hz`.
- Каналы:
  - **Mono (1 ch)** — пространственные звуки мира (`Creatures`, `Weapons_And_Tools`, `Footsteps`, `Dismemberment_And_Gore`, `RIG_And_Suit`, `Human_Voices`, `Ship_Environment`, `UI`).
  - **Stereo (2 ch)** — музыка, эмбиент, маркер/деменция, логи, озвучка и объявления (`Soundtrack`, `Ship_Ambience`, `Dementia_And_Marker`, `Story_And_Logs`, `Announcements`).
- В русской озвучке (`Audio/Announcements/`, `Audio/Human_Voices/Russian/`, `Audio/Story_And_Logs/Russian/`) размещаются только реальные дубляжи (EA/GamesVoice/R.G. MVO/CGInfo), без синтезированного TTS.

## Документация и проверка

- Дубликаты `.ogg` (по SHA-256 и декодированному PCM MD5) и полностью идентичные `.rsi`-пакеты не допускаются.
- Шрифты и клиентская графика (`Fonts/`, `Logo/`, `Parallaxes/`, `Interface/`) сопровождаются файлом лицензии/атрибуции и записью в `ATTRIBUTIONS.md`.
- Ссылки в `README.md` — только относительные, без эмодзи и локальных путей.
- Перед пулл-реквестом изменения проверяются автоматическим воркфлоу `.github/workflows/validate.yml`.
