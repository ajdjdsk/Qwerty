# Qwerty — Suno Prompt Engineering

Коллекция тщательно проработанных промптов для генерации музыки в **Suno**.
Каждый файл — один трек. В каждом промпте есть:

- **Название трека** (рядом в скобках — модель: Opus 4.8)
- **Ползунки** Influence и Weirdness (в процентах)
- **Negative prompt** (что исключить)
- **Styles** (строго ≤ 1000 символов)
- **Lyrics** — лирика со смыслом + поэтапное описание звучания (вступление, куплеты, припев, бридж, аутро, приёмы со скрипкой и оркестром)

> **Готовая команда для генерации новых треков:**
> - **Cursor slash-команда** — [`.cursor/commands/suno.md`](.cursor/commands/suno.md). Скопируй её в `~/.cursor/commands/suno.md` (Windows: `%USERPROFILE%\.cursor\commands\suno.md`) и вызывай в чате `/suno` (например `/suno 2 трека, мрачный вальс`).
> - **Или вручную** — [SUNO_PROMPT_ENGINEER_BRIEF.md](SUNO_PROMPT_ENGINEER_BRIEF.md): скопируй блок между `=== COMMAND START ===` и `=== COMMAND END ===` и вставь любой модели.

### Общая эстетика
Эпичный готический оркестр, виртуозная скрипка, динамика и захват с первых секунд.
Голос — **тёплый, зрелый** женский альт (в духе вокала конца 70-х), богатое вибрато,
мелизматическое и эмоциональное пение. Без тонких «молоденьких» высоких голосов.
Язык — английский. Без упоминания реальных групп и исполнителей.

## Треки

| # | Трек | Настроение | Influence / Weirdness |
|---|------|------------|------------------------|
| 01 | [The Lighthouse Keeper's Last Dawn](prompts/01-the-lighthouse-keepers-last-dawn.md) | скорбное достоинство → светлое принятие | 68% / 24% |
| 02 | [The Cartographer of Goodbyes](prompts/02-the-cartographer-of-goodbyes.md) | тоска → благодарность, маршевый драйв | 64% / 30% |
| 03 | [Crown of Broken Glass](prompts/03-crown-of-broken-glass.md) | ярость → торжество, воинственный | 70% / 33% |
| 04 | [The Light You Left Behind](prompts/04-the-light-you-left-behind.md) | светлое утешение «с той стороны», минор→мажор | 74% / 18% |
| 05 | [The Unwritten Will](prompts/05-the-unwritten-will.md) | величественное, суверенное; рояль-соавтор | 76% / 22% |
| 06 | [The Last Song in the Deep](prompts/06-the-last-song-in-the-deep.md) | щемящая трагическая красота, оголённо-скорбное | 72% / 28% |
| 07 | [The Hour That Almost Won](prompts/07-the-hour-that-almost-won.md) | на грани отчаяния → ярость к жизни, драйв | 72% / 26% |
| 08 | [Letters to the Girl I Was](prompts/08-letters-to-the-girl-i-was.md) | тёплая нежность → сияющая сила, самопрощение | 75% / 19% |
| 09 | [Everything Has a Price](prompts/09-everything-has-a-price.md) | мрачный готический вальс 3/4, соблазн → прозрение | 70% / 34% |
| 10 | [The Name She Cannot Find](prompts/10-the-name-she-cannot-find.md) | деменция матери: любовь живёт за гранью памяти | 74% / 20% |
| 11 | [I Burned the Way Back](prompts/11-i-burned-the-way-back.md) | сжечь путь назад: ярость → яростная свобода | 71% / 30% |
| 12 | [Carousel](prompts/12-carousel.md) | горько-сладкое кружение времени, 6/8, креативные тембры | 70% / 33% |
| 13 | [Everything I Never Said](prompts/13-everything-i-never-said.md) | невысказанные слова любви, исповедь, виолончель-дуэт | 73% / 24% |
| 14 | [I'd Choose the Fall](prompts/14-id-choose-the-fall.md) | отклонение настроения: страстное, светлое «да» жизни | 75% / 21% |
| 15 | [Dance, Old Friend](prompts/15-dance-old-friend.md) | лукаво-макабрическое, театральное; танец со Смертью | 70% / 38% |
| 16 | [Barefoot in the Storm](prompts/16-barefoot-in-the-storm.md) | экстатическое, дикое, эйфоричное; танец под грозой | 68% / 32% |
| 17 | [The Wolves at the Gate](prompts/17-the-wolves-at-the-gate.md) | боевой: героический последний рубеж, трагич.-славный | 73% / 30% |
| 18 | [Vengeance Is a Patient Beast](prompts/18-vengeance-is-a-patient-beast.md) | боевой: хищная угроза → взрывная расплата | 72% / 33% |
| 19 | [Count Me In](prompts/19-count-me-in.md) | фишка: тикающие часы ускоряются → обрыв во вне-время | 71% / 35% |
| 20 | [A Thousand Names](prompts/20-a-thousand-names.md) | мистический восточный/суфийский транс, кружение | 70% / 36% |
| 21 | [Ember to Inferno](prompts/21-ember-to-inferno.md) | фишка: единый крещендо-болеро, уголёк → пожар | 74% / 30% |
| 22 | [Higher Than the Dark](prompts/22-higher-than-the-dark.md) | фишка: припевы по нарастающим тональностям; вытащить из тьмы | 75% / 26% |
| 23 | [Nobody's Rock Tonight](prompts/23-nobodys-rock-tonight.md) | новое: джаз-нуар торч-сонг; право быть слабой | 71% / 27% |
| 24 | [Carry Them Home](prompts/24-carry-them-home.md) | новое: сакральный реквием (лат. хор); скорбь → благодать | 74% / 24% |
| 25 | [The Quiet Brave](prompts/25-the-quiet-brave.md) | флагман: невидимое мужество обычных людей; один голос → общий хор | 73% / 23% |
| 26 | [The Floor Will Remember](prompts/26-the-floor-will-remember.md) | новое: фламенко-готик (duende); вбить боль в танец | 72% / 31% |
| 27 | [Storm and Spring](prompts/27-storm-and-spring.md) | новое: барочный концерт (Вивальди), быстро-медленно-быстро; принять все сезоны жизни | 73% / 28% |
| 28 | [Dust for a Name](prompts/28-dust-for-a-name.md) | новое: спагетти-вестерн-готик; реинвенция, оставить прежнюю себя | 72% / 30% |
| 29 | [Hallelujah in the Wreckage](prompts/29-hallelujah-in-the-wreckage.md) | новое: готик-госпел-возрождение; дерзкая благодать на дне | 73% / 27% |
| 30 | [The Oldest Song](prompts/30-the-oldest-song.md) | колыбельная сквозь поколения; любовь как нить, что передают | 74% / 21% |
| 31 | [The Understudy](prompts/31-the-understudy.md) | ядро готик-симфо; «дублёр» выходит на свет; скрипка из ансамбля в соло | 74% / 23% |
| 32 | [Three Minutes](prompts/32-three-minutes.md) | новое: тёмное аргентинское танго (бандонеон); невозможная любовь, один танец | 72% / 30% |
| 33 | [The Last Green Hill](prompts/33-the-last-green-hill.md) | новое: кельтский плач (uilleann pipes); эмиграция, дом внутри тебя | 71% / 28% |
| 34 | [The Staying](prompts/34-the-staying.md) | ядро готик-симфо; негромкий героизм долгой любви длиною в жизнь | 74% / 20% |
| 35 | [Dance the Dark Away](prompts/35-dance-the-dark-away.md) | итало/евро-диско 70-х × готик-ядро; танцем лечить сердце | 70% / 28% |
| 36 | [Signal in the Dark](prompts/36-signal-in-the-dark.md) | новое: космо-диско 70-х × готик-ядро; сигнал любви в космос | 70% / 31% |
| 37 | [Both of Me](prompts/37-both-of-me.md) | эксперимент-ядро: скрипка как «тень»-дуэт, 7/8→4/4; перемирие с собой | 71% / 38% |
| 38 | [The Summer We Were Gold](prompts/38-the-summer-we-were-gold.md) | средиземноморское «закатное» итало 70-х × готик-ядро; золотое лето в памяти | 71% / 26% |
| 39 | [Rewind Me Home](prompts/39-rewind-me-home.md) | эксперимент: жизнь задом наперёд, reverse-свеллы, кульминация в «начале» | 72% / 37% |
| 40 | [A Choir of One](prompts/40-a-choir-of-one.md) | эксперимент: вокальный канон/раунд из одного голоса; одна ≠ одинока | 72% / 36% |
| 41 | [The Beauty of the Falling](prompts/41-the-beauty-of-the-falling.md) | новое+эксперимент: японский гагаку/мин'ё × готик; «ма»-тишина; mono no aware | 71% / 37% |
| 42 | [Blow My Cover](prompts/42-blow-my-cover.md) | новое: нео-нуар «шпионский» оркестр; броня → смелость быть узнанной | 71% / 29% |
| 43 | [Read Me Backwards](prompts/43-read-me-backwards.md) | эксперимент: обратимый текст — отчаяние ↔ надежда; минор-спуск → мажор-подъём | 72% / 35% |
| 44 | [My Father's Son](prompts/44-my-fathers-son.md) | эксперимент: МУЖСКОЙ голос (баритон); мужская броня → слёзы, прорыв плотины | 73% / 27% |
| 45 | [Through Me Like a Storm](prompts/45-through-me-like-a-storm.md) | эксперимент: МУЖСКОЙ мелодичный хард-рок × готик (грит-белт, диджериду); капитуляция буре | 73% / 28% |
| 46 | [Between You and the Dark](prompts/46-between-you-and-the-dark.md) | эксперимент: МУЖСКОЙ хард-рок голос в чистом ядре; обет быть стеной от тьмы | 74% / 26% |
| 47 | [The Love Story Nobody Writes](prompts/47-the-love-story-nobody-writes.md) | ядро (жен.); дружба как главная любовь жизни; маскировка под романс | 74% / 21% |
| 48 | [At the Same Time](prompts/48-at-the-same-time.md) | эксперимент ядра: политональность (мажор+минор разом); радость и горе вместе | 72% / 35% |
| 49 | [The Age You Were](prompts/49-the-age-you-were.md) | ядро (жен.); прощение матери — «теперь мне столько, сколько было тебе»; минор→мажор | 74% / 22% |
| 50 | [Whenever You Come Home](prompts/50-whenever-you-come-home.md) | ядро (жен.); свет на крыльце для ушедшего ребёнка; безусловная любовь | 74% / 21% |
| 51 | [The Women Before Me](prompts/51-the-women-before-me.md) | новое+эксперимент: балканские «mystery voices», 7/8→9/8, диссонанс→унисон; женская родовая сила | 71% / 38% |

> В каждом файле трека теперь есть поле **«Направление / стиль»** — явно указанная манера исполнения/жанр (особенно полезно для экспериментов).

> Вокальная подача зашита прямо в поле **Styles** и в короткие пометки в **тегах секций** (отдельного раздела «стиль пения» нет — его нельзя вставить в Suno).

> **Заметка по подаче (с батча 3):** инструментал поддерживает вокал непрерывно — скрипка/рояль/бас вьются под и вокруг голоса, а не только в паузах (никакого «спела → заиграли → затихли → опять спела»). Поэтапное звучание по-прежнему расписано прямо в скобочных ремарках внутри лирики.
