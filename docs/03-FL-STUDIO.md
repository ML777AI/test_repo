# 03 — FL Studio: что поставить и как собрать шаблон

Цель: один шаблон `HELL_TEMPLATE.flp`, из которого растут все 15 треков и лайв-проект. Без шаблона трилогия разъедется по громкости, тюнингу и ударным.

## Издание FL Studio

Нужен минимум **Producer**. Лучше **Signature** (Harmor, Gross Beat, Hardcore, Vocodex, Pitcher). All Plugins не обязателен.

Проверить сразу: `Help → About` и список плагинов в `Add → Plugins`. Если нет Harmor / Gross Beat — не блокирует работу, их закрывают Vital + бесплатные гейты.

## Установка VST: правило папки

Одна папка, не размазывать по `Program Files`.

```
C:\VST3\
C:\VSTPlugins\          (только если плагин не умеет VST3)
```

В FL: `Options → Manage plugins → Plugin search paths` — добавить эти пути → `Find plugins`.  
Включить `Keep unsaved plugins` выкл. После скана: нужные плагины `Add to plugin database (tree)`.

ASIO: драйвер **MOTU M2** (не Generic ASIO).  
Студия: buffer 128–256 при записи гитары/вокала, 512–1024 при сведении тяжёлого проекта.  
Sample rate: **48000**. Sample rate M2 в панели MOTU = 48000, иначе щелчки.

## Что уже есть в FL и чем это закрывает стиль

| Роль | Нативный плагин | Как использовать здесь |
| --- | --- | --- |
| Drone / pad | Harmor, Sytrus, Harmless | Один голос, unison 0–2, фильтр низко, длинный release |
| FM-металл | Sytrus | Оператор B→A, ratio 2.01, feedback |
| Гитарный amp | Hardcore (если Signature) | Только черновой; финал — NAM |
| Удар | FPC, Slicex, Drumaxx | FPC под пады MPK; Slicex для нарезки своих industrial one-shots |
| Гейт / stutter | Gross Beat | Rave-окна, не весь трек |
| Реверб | Reverb 2, Convolver | Convolver + свои IR (бетон, ангар, лестница) |
| Дилей | Delay 3 | Ping-pong 1/8 dotted на гитару |
| Грязь | Distructor, Fast Dist, Blood Overdrive, WaveShaper | Параллельный bus, не на master |
| Вокал pitch | Pitcher, Newtone | Коррекция, не эффект |
| Вокал робот/хор | Vocodex | Редкие жесты CORE |
| Грануляр | Granulizer | Dematerialization, View Calculation |
| Макс / мастер | Maximus, Limiter, Soft Clipper | Maximus на buses; Limiter на master −1.0 dBTP |
| Лайв-сборка | Patcher, Performance mode | Обязательно |
| Запись | Edison, Mixer recording | Сухие стволы всегда |

## Обязательный бесплатный набор

Ставить всё. Это и есть «брутальный инструментарий» без аренды Omnisphere.

### Синтез и drone

1. **Vital** — главный wavetable. Дроны, суб, металлические пады.  
   https://vital.audio
2. **Surge XT** — второй движок, другой характер фильтра.  
   https://surge-synthesizer.github.io
3. **Odin 2** — толстый analog-ish для тарана BULLS.
4. **OB-Xd** — если нужен «холодный воздух» FLASH.
5. **Dexed** — FM-колокола и железо Mechanics Set.

### Пространство (это 50% жанра)

6. **Valhalla SuperMassive** — обязателен. Dark ambient без него собирается дольше и хуже.  
   https://valhalladsp.com/shop/reverb/valhalla-supermassive/
7. **TAL-Reverb-4** — короткий «плиточный» хвост, когда SuperMassive слишком бесконечен.
8. **Cloud Reverb** (if available) не нужен, если есть SuperMassive.

Пресеты SuperMassive: огромные `Slow Deep` / `Dark Space`. Mix 20–40% на buses, 80–100% на dedicated verb-return. Не вешать SuperMassive на master.

### Гитара

9. **Neural Amp Modeler (NAM)** + кабинеты с ToneHunt. Искать high-gain / modern / 8-string IR.  
   https://www.neuralampmodeler.com  
   Писать DI всегда. NAM — insert на копии DI.
10. Если NAM неудобен: FL Hardcore + Convolver с кабинетом.

### Анализ и сведение

11. **Voxengo SPAN** — спектр. Смотреть суб 30–50 Hz и грязь 2–5 kHz.
12. **TDR Nova** — динамический EQ (гул 200–400 Hz на гитаре и вокале).
13. **TDR Kotelnikov** — автобусный компрессор.
14. **Youlean Loudness Meter** — мастер под стриминг: цель **−9…−8 LUFS** для этого жанра (не −14: иначе удар умрёт). True Peak ≤ −1.0 dB.

### Текстуры и «ад»

15. **PaulXStretch** — Dematerialization, хвосты View Calculation.
16. **Chow Tape Model** — Septic Condition.
17. **Airwindows** (Density, Console, ClipOnly) — клей и клип kick.
18. **Melda MFreeFXBundle** — MMultiBandDistortion, MConvolutionEZ.
19. **GClip** или клиппер Airwindows на kick-bus.

### Сэмплеры / хор

20. **Decent Sampler** + бесплатные тёмные хоры/органы (не cinematic trailer packs).
21. **Spitfire BBC Symphony Orchestra Discover** (бесплатно, осторожно с лимитами Content ID: это библиотека, не «loop pack», обычно ок, но не класть готовые фразы-демо).

### Не ставить

- Готовые «Dark Ambient Loop Kit 24bit» с Splice, если планируется Content ID.
- Десять ревербов «на всякий». SuperMassive + TAL-4 + Convolver хватает.
- iZotope озон как костыль вместо сведения.

## Платный набор: только если звук упёрся

Покупать **после** того, как 2–3 трека BULLS собраны на бесплатном.

| Покупка | Зачем | Когда |
| --- | --- | --- |
| Valhalla VintageVerb + Shimmer | Храм и «свет» FLASH | Если SuperMassive не даёт короткий hall |
| FabFilter Pro-Q 3 / Saturn 2 | Хирургия и насыщение | Если Nova/Distructor не хватает |
| Output Portal | Грануляр как инструмент | Dematerialization / View Calculation |
| Neural DSP Gojira или Nolly | Скорость гитарного тона | Если NAM надоел |
| Serum 2 | Один универсальный synth | Если Vital неудобен |
| Soundtoys Decapitator | Мясо на buses | Опционально |

Omnisphere не нужен для этой трилогии.

## Шаблон HELL_TEMPLATE.flp

### Mixer (имена каналов сохранить)

| Канал | Назначение |
| --- | --- |
| 1 DRONE | Vital/Surge суб+пад |
| 2 AIR | Шум, хор, tape hiss |
| 3 GTR DI | Сухой DI, без amp |
| 4 GTR AMP | NAM / Hardcore |
| 5 GTR FX | Reverb/stretch гитара |
| 6 KICK | Kick + clipper |
| 7 PERC | Hats, snare, metals |
| 8 VOC DRY | Сухой вокал |
| 9 VOC FX | Параллель грязь+реверб |
| 10 FX SEND | One-shots, risers (свои) |
| 11 BUS DRONE | 1+2 |
| 12 BUS GTR | 3–5 |
| 13 BUS DRUM | 6+7 |
| 14 BUS VOC | 8+9 |
| 15 VERB | SuperMassive return |
| 16 DELAY | Delay 3 return |
| 17 MASTER | EQ → Maximus → Limiter → Youlean |

Сенды: все музыкальные каналы → 15 и 16. Kick в VERB почти не слать (0–5%).

### Channel rack

- FPC `HELL_DRUMS` с 16 своими или самосведёнными ударными (kick, cannon, snare, 3 hats, 4 metals, 4 vocal chops, 2 silences/mute).
- Vital `DRONE_A`, Vital `DRONE_B`, Surge `METAL`.
- Sampler для гитарных one-shots.
- Patcher `LIVE_FX` (фильтр + dist + verb send) — тот же Patcher едет в лайв.

### Tuning

В шаблоне: `Options → Project general settings → Pitch` = 0.  
Гитарный тюнер внешний в E. Не транспонировать проект.

### Маркеры Playlist

Шаблонные маркеры: `INTRO / GATE / RAVE / HELL / EXIT / TAIL`.  
Для View Calculation: `ROOM1 … ROOM5 / WALKOFF`.

## Запись

Гитара: M2 input 2 Inst, pad если клипит, gain так, чтобы DI пики −10 dBFS.  
Вокал: M2 input 1 Mic. Мониторинг через Direct Monitor M2, не через FL (иначе латенция).  
Запись в Edison **и** на playlist-клип. Edison-файл сразу Save as `BULLS_02_voc_take03.wav` в папку стемов.

Структура папок:

```
D:\HELL\
  _template\HELL_TEMPLATE.flp
  BULLS\01_Mechanics_Set\ project.flp, audio\, renders\
  BULLS\02_Bravery_Glory\
  ...
  CORE\08_View_Calculation\
  FLASH\...
  _live\HELL_LIVE.flp
  _stems\
  _masters\
  _artwork\
  _video\
```

Рендер стемов: каждый bus отдельно, same start, 48k/24, leave tail. Лайв питается от `_stems`, не от студийного `.flp`.
