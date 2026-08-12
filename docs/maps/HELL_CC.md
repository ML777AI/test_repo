# Карта CC для записи в MPK-261 Edit Mode

Прописать одинаково в User Preset 1 и 2 (меняются только назначения в FL `.fsc`).  
`Edit` → выбрать контрол → Type = CC → Number = как в таблице → Channel как указано → `Preset` Save.

## Клавиши

- Type: Note
- Channel: 1
- Aftertouch: On (Global)

## Пады (все банки)

- Type: Note
- Channel: 10
- Bank A notes: 36–51 (C1–D#2) — стандарт MPC/FPC
- Bank B notes: 52–67
- Bank C notes: 68–83
- Bank D notes: 84–99
- Aftertouch падов: On (pressure → modulation в FPC, по желанию)

## Фейдеры

Channel 1. Type: CC. Bank Select не трогать, три банка железа = три набора CC.

| Фейдер | Bank 1 CC | Bank 2 CC | Bank 3 CC |
| --- | --- | --- | --- |
| 1 | 20 | 30 | 40 |
| 2 | 21 | 31 | 41 |
| 3 | 22 | 32 | 42 |
| 4 | 23 | 33 | 43 |
| 5 | 24 | 34 | 44 |
| 6 | 25 | 35 | 45 |
| 7 | 26 | 36 | 46 |
| 8 | 27 | 37 | 47 |

## Крутилки

Channel 1. Type: CC.

| Knob | Bank 1 CC | Bank 2 CC | Bank 3 CC |
| --- | --- | --- | --- |
| 1 | 14 | 50 | 60 |
| 2 | 15 | 51 | 61 |
| 3 | 16 | 52 | 62 |
| 4 | 17 | 53 | 63 |
| 5 | 18 | 54 | 64 |
| 6 | 19 | 55 | 65 |
| 7 | 70 | 56 | 66 |
| 8 | 71 | 57 | 67 |

CC 1 (mod wheel) не занимать фейдерами — оставить колесу модуляции.

## Свитчи

Channel 1. Type: CC, Momentary для mute, Toggle для bypass.

| Switch | Bank 1 CC | Bank 2 CC | Bank 3 CC |
| --- | --- | --- | --- |
| 1 | 80 | 90 | 100 |
| 2 | 81 | 91 | 101 |
| 3 | 82 | 92 | 102 |
| 4 | 83 | 93 | 103 |
| 5 | 84 | 94 | 104 |
| 6 | 85 | 95 | 105 |
| 7 | 86 | 96 | 106 |
| 8 | 87 | 97 | 107 |

Лайв Bank 1 switch 6 (Panic): в FL линковать на Stop + Patcher Kill. На железе Type = CC, в FL — два линка на один CC через formula или просто Stop.

## Педали

- Sustain: CC 64, Channel 1
- Expression: CC 11, Channel 1 → в лайве линк на Patcher Low-pass

## Транспорт

Оставить заводской MMC пресета 11. Не переписывать в обычные CC, если Play уже работает.
