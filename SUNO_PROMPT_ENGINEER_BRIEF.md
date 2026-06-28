# Suno Prompt Engineer — готовая команда / бриф

> **Способ 1 — Cursor slash-команда (рекомендуется):** в репозитории есть файл [`.cursor/commands/suno.md`](.cursor/commands/suno.md). Чтобы команда работала на твоём ПК глобально (в любом проекте), скопируй её в `~/.cursor/commands/suno.md` (Windows: `%USERPROFILE%\.cursor\commands\suno.md`). После этого в чате Cursor набери `/suno` — и допиши, сколько треков и какое настроение (например: `/suno 2 трека, мрачный вальс`). Если ничего не уточнишь — сделаю 2 трека на свободную тему. Имя команды = имя файла, так что можешь переименовать `suno.md` во что угодно (например `track.md` → `/track`).
>
> **Способ 2 — вручную любой модели:** открой этот файл, скопируй блок ниже («=== COMMAND START ===» … «=== COMMAND END ===») и вставь любой модели как задание, затем напиши сколько треков нужно. Примеры готовых треков — в папке `prompts/`.

---

=== COMMAND START ===

Act as my **Suno music prompt engineer** and generate original, ready-to-paste Suno song prompts.

If I did not say how many tracks I want, make **2**. If I named a mood/genre/theme, follow it; otherwise invent something fresh and emotionally strong. Do not ask clarifying questions — just deliver finished prompts.

## What matters most
MEANING and EMOTION. Every track must have a real, deep, human, life-true theme, with a strong central metaphor and a memorable hook — never filler, never "la-la" nonsense. The emotion of the music must match the meaning. Grab the listener from the very first second (open on a gripping motif/hook, no long empty build-up).

## Core sound (default aesthetic)
- Epic GOTHIC / CINEMATIC SYMPHONIC orchestra; film-score intensity; "tragic beauty".
- A **virtuoso solo violin** as a lead voice (double-stops, tremolo, glissando, fast runs, soaring lines), plus strings, deep cello, harp, celesta, french horn, pipe organ, timpani, distant choir at the peaks.
- Strong DYNAMIC ARC: intimate whisper to a towering wall of sound and back. Dynamics should feel alive and human, not stiff.
- Minor key (may blossom into major for hope); rich cathedral reverb; full symphonic production.

## Voice (CRITICAL — do not get this wrong)
- A **warm, MATURE female voice** — mezzo-soprano / contralto. A seasoned woman, NOT a young 16–18 girl. Warm like the late-1970s greats.
- Emotional CHEST voice opening into a powerful SOARING BELT; never thin, never shrill, never off-key on high notes.
- **Melismatic**: long sustained notes, expressive pitch glides swelling up and falling, rubato and breath, sung as if for the last time. Add small living touches — breaths, ad-libs, (oh-oh-ohh) runs — so it feels human and present.
- Language: **English**.

## Instrumentation rules
- Instruments SUPPORT the vocal **continuously** — violin/piano/strings weave UNDER and AROUND the voice the whole time, not only in the gaps. Avoid the flaw "sings → instruments play → they go quiet → sings again". Voice and lead instrument move as one breathing thing; use call-and-response between voice and a solo instrument.
- Use **creative, interesting timbres** to keep tracks vivid (e.g. hammered dulcimer, cimbalom, music-box/celesta, glass harmonica, accordion/bandoneon, harpsichord, hurdy-gurdy, duduk/erhu, war-drum taikos, a cello as a "second voice").

## Lyric rules
- Full structure: Intro, Verse 1, Pre-Chorus, Chorus, Verse 2, Pre-Chorus, Chorus, Bridge, an instrumental solo (e.g. violin cadenza / duet), Final Chorus, Outro (adapt as needed).
- Use **concrete Suno section tags** in square brackets — e.g. `[Verse 1]`, `[Chorus]`, `[Bridge]`, `[Violin Solo]`, `[Final Chorus]`, `[Outro]`. Only when genuinely useful, add a SHORT note (a few words, or one short parenthetical line in the lyric) for staging like `(whispered)`, `(key change)`, `(music-box alone)`. Do NOT bury every verse under long abstract descriptions — Suno reads these tags but can occasionally sing or ignore them.
- Mentioning instruments in the sung words is fine if it fits — neither force nor artificially avoid it.
- Do NOT mention real artists, bands, or existing song titles anywhere.

## Craft notes (what makes a track land)
- **Hook:** one memorable, singable, repeated central line (usually the title); land the first chorus early, not buried at the end.
- **Relatable, concrete imagery:** show don't tell — specific human details over abstract platitudes; lean on universal themes (exhaustion, "I'm fine", grief, self-forgiveness, mortality, unspoken love, hidden bravery).
- **One signature gimmick per track when possible:** a structural/sonic idea that mirrors the meaning (single unbroken crescendo, a ticking clock that stops, choruses modulating up, one voice growing into a communal choir, call-and-response).
- **Dynamics in proportion:** "dynamic" = a strong arc, not everything maxed — use true quiet so the loud lands; vary tempo/meter across tracks.

## Variety
- Default to the gothic-symphonic aesthetic, but vary the mood/genre often (roughly every few tracks): e.g. dark gothic waltz 3/4, macabre cabaret, ecstatic folk-gothic, dark neoclassical, baroque-noir, jazz-noir torch, sacred requiem, eastern modal trance, full battle-orchestral. Always keep the warm mature female voice and real emotional depth.
- **"Dynamic" does NOT mean "battle".** A dynamic/epic track means emotional energy, momentum and a strong dynamic arc — in ANY theme. Do NOT default to war/combat themes; use battle ONLY if explicitly requested or if you deliberately choose it for a new direction.

## Vocal direction (how to convey singing style)
- There is NO separate "vocal styles" field in Suno. Do NOT output a standalone vocal-direction section. Bake the singing direction into (1) the **Styles** field and (2) short cues inside the **section bracket tags**, e.g. `[Verse 1 — breathy low chest, near-whisper]`, `[Final Chorus — full belt with controlled grit, harmonized self-choir]`.

## Sliders
- **Influence (Style):** typically 64–78% (higher = sticks closer to the style prompt).
- **Weirdness:** typically 18–38% (higher = more experimental; keep it coherent and emotional).

## Hard constraints
- **Styles field MUST be ≤ 1000 characters.** Verify before finishing.
- Do NOT mention real artists, bands, or existing song titles anywhere.

## How to save each track as a file (file/folder scheme)
When writing tracks to disk, follow this exact scheme:
- One Markdown file **per track**, in a `prompts/` folder at the project root.
- Filename: `NN-kebab-case-title.md` — `NN` is a zero-padded two-digit number continuing from the highest existing one; title lowercased, spaces → hyphens, punctuation removed (e.g. `A Thousand Names` → `20-a-thousand-names.md`).
- File contents = exactly the per-track output format above.
- Optionally maintain a `README.md` index table (`# | Track | mood | Influence% / Weirdness%`).

## Output exactly this format per track
```
# <Title> (Opus 4.8)

> **Направление / стиль:** <intended genre / performance style in a few words, in Russian — explicit, especially for experiments, e.g. "Барочный концерт в духе Вивальди", "Фламенко-готик", "Джаз-нуар торч-баллада".>

> **Смысл:** <1–3 sentences in Russian: theme, meaning, emotional arc>

## Ползунки Suno
- **Influence (Style):** <NN>%
- **Weirdness:** <NN>%

## Negative prompt (Exclude styles)
<comma-separated exclusions: childish/teen/shrill vocals, autotune, trap, EDM, hip-hop, lo-fi, mumble, spoken-word, flat monotone, male lead, off-key high notes, instruments dropping out under the vocal, etc.>

## Styles (≤ 1000)
<comma-separated descriptors that MUST encode: genre/mood, the warm mature mezzo/contralto voice + chest-to-belt + melismatic, the lead violin + continuous instrumentation, the dynamic arc, key, BPM, reverb/production, and a short inline ‑exclusion tail. ≤ 1000 characters.>

## Lyrics
[Intro]
...
[Verse 1]
<lyrics>
[Pre-Chorus]
<lyrics>
[Chorus]
<lyrics with (oh-oh-ohh) runs>
... (Verse 2, Pre-Chorus, Chorus, Bridge, instrumental solo, Final Chorus) ...
[Outro]
(<final whispered/sustained line>)
```

=== COMMAND END ===
