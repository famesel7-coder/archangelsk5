# Content / Business Reference Set — 2026-08-17

Этот документ фиксирует разбор 18 пользовательских экранов для проекта «Архангельск 5». Он дополняет, но не заменяет `brand/visual-style.md`, `tokens/design-tokens.json` и `prompts/slide-agent.md`.

## Формат и область применения

- целевой мастер проекта: **Full HD, 1920 × 1080 px, 16:9**;
- 15 референсов имеют точный размер `1920 × 1080` и подтверждают геометрию CONTENT / BUSINESS режима;
- 3 референса имеют размер `2048 × 512` и подтверждают только визуальную грамматику панорамной композиции;
- панорамные референсы нельзя растягивать, letterbox или механически обрезать под Full HD — их нужно перекомпоновывать.

Неизменённые raster sources сохранены в `references/screens/content-business-2026-08-17/`. Полные repository paths и SHA-256 всех файлов записаны в `tokens/design-tokens.json` → `reference_sets.content_business_2026_08_17`.

## Full HD references

| Файл | Размер | Основной паттерн |
|---|---:|---|
| `2(1).png` | 1920 × 1080 | плотная аналитика: тренд + bars + прямые подписи |
| `3(2).png` | 1920 × 1080 | lessons mosaic; локальные grouped planes |
| `6(1).png` | 1920 × 1080 | product/category case: графики + промо-evidence + KPI |
| `10.2.png` | 1920 × 1080 | comparison через две крупные пространственные зоны и big bars |
| `12.png` | 1920 × 1080 | store/category audit: фото, таблица, KPI и process strip |
| `13.png` | 1920 × 1080 | category performance: packshots + small multiples + планы |
| `14.png` | 1920 × 1080 | geographic expansion: donuts + карта + маршрут покрытия |
| `15.png` | 1920 × 1080 | product sales dynamics: packshots + trends + KPI summary |
| `22.png` | 1920 × 1080 | category development: chart evidence + one expressive product visual |
| `2049.png` | 1920 × 1080 | local competition: paired trends + documentary storefront photos |
| `2050.png` | 1920 × 1080 | initiative summary + bar trend + revenue line trend |
| `2056.png` | 1920 × 1080 | dense small multiples + regional comparison + reasons/plans |
| `2064.png` | 1920 × 1080 | oversized KPI + analytical map + two-status markers |
| `2077.png` | 1920 × 1080 | local success story: maps + real photo + promo evidence + trend |
| `2078.png` | 1920 × 1080 | multi-series trend + documentary media/application collage |

## Ultrawide references

| Файл | Размер | Смысловой ритм для адаптации в 16:9 |
|---|---:|---|
| `7(2).png` | 2048 × 512 | statement → KPI mosaic → reasons/evidence |
| `11.png` | 2048 × 512 | statement → territory map → annotated trend |
| `3(3).png` | 2048 × 512 | big KPI → territory map → characteristics/conclusion |

В Full HD сохраняется не ширина и не расположение блоков, а последовательность чтения. Базовый reflow: верхняя headline zone и одна или две крупные зоны ниже. Если три смысловых слоя требуют мелкого текста, материал делится на два слайда.

## Confirmed

- CONTENT / BUSINESS живёт на почти чёрном petrol-green canvas: `#051921` или `#0A1B22`; Figma также подтверждает `#03151C`;
- локальные analytical planes используют `#122029` и `#12242B`;
- основной текст и заголовки — белые, X5 Sans; content-title чаще sentence case;
- повторяются левый anchor `85–90 px`, верхний anchor `80–100 px`, правый anchor около `90 px`;
- green `#00DD76` — active/positive highlight;
- cyan `#18BDF3` — comparator/второй статус, а не общий декоративный цвет;
- grey `#828C90` — neutral/previous series;
- magenta `#F03C72` — negative/adverse semantic;
- графики используют direct labels, минимальные axes/gridlines, rounded caps, markers и bars;
- карты работают как самостоятельный analytical visual: зелёная активная территория, тёмный контекст, 1–2 статуса pins;
- реальные project-фото, packshots, промо-листовки и shelf/store evidence являются частью языка CONTENT / BUSINESS;
- photo collage строится вокруг одного hero image, без тяжёлых теней;
- радиусы около `16–24 px` повторяются у photo masks и локальных analytical planes;
- dense slides допустимы, если все элементы подчинены одному выводу.

## Inferred

- рабочая нижняя safe area обычно находится в диапазоне `60–80 px`;
- analytical planes нужны для смысловой группировки, а не как универсальный UI component;
- при 3+ рядах данных могут использоваться дополнительные series colors, но только локально и семантически;
- visual rhythm панорамных экранов переносится в Full HD через reflow, а не через scale;
- в одной презентации cinematic HERO / BRAND и flat CONTENT / BUSINESS режимы должны чередоваться, сохраняя X5 Sans, тёмное поле и зелёный core accent.

## Unconfirmed

- единый обязательный column grid для всех content-слайдов;
- единый точный radius для всех panels и фотографий;
- точные дополнительные series colors для графиков с 3+ рядами;
- обязательная ширина line chart strokes и размер markers;
- универсальное место логотипа на content-слайдах;
- правила обработки каждого типа внешних фотографий за пределами предоставленного набора.

## Что не переносить в систему автоматически

- жёлтый цвет промо-листовки — это цвет content asset, а не новый цвет бренда презентации;
- magenta, amber, red и violet из отдельных графиков не становятся декоративной палитрой;
- карточная композиция из `3(2).png` и `7(2).png` не становится универсальным template для всей презентации;
- cyan не используется в hero-light, типографике и фоне без аналитической причины;
- фотография не вставляется как случайный stock-visual: она должна подтверждать вывод;
- панорамные `2048 × 512` файлы не считаются разрешением рабочего слайда.

## Новые устойчивые архетипы

1. **Annotated trend** — крупный line/bar chart, direct labels, один semantic highlight.
2. **Map + KPI split** — карта занимает 55–70% рабочей зоны, рядом один oversized KPI и короткая легенда.
3. **Evidence collage** — один главный документальный кадр + 1–3 supporting images.
4. **Product performance sheet** — packshot/category visual + trend + 2–3 KPI.
5. **KPI → evidence → action** — панорамная логика, заново собранная в 16:9.

## Production rule

Перед финализацией любой композиции открыть её в `1920 × 1080`, проверить title wrapping, direct labels, photo crops, data collisions и safe area. Референс задаёт грамматику, но новый слайд должен иметь собственный силуэт и один главный вывод.
