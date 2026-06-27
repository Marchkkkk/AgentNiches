# GENERAL RULES — спільне для ВСІХ ніш

Цей файл — єдине місце для залізного контракту з кодом і універсального крафту.
Нішеві файли (`brief.md`, `competitors.md`, `lessons.md`) можуть лише
ДОПОВНЮВАТИ ці правила під свою нішу — ніколи не послаблювати.

════════════════════════════════════════════════════════════════════════════
1. HARD CONTRACT — як софт використовує промпти (НІКОЛИ не порушувати)
════════════════════════════════════════════════════════════════════════════
1.1 Пайплайн ДОПИСУЄ реальний інпут у кінець кожного промпта в рантаймі:
    - до `outline`-промпта:  "\n\nIdea: <ідея>"
    - до `story`-промпта:     "\n\nOutline:\n<аутлайн>"
    Тому промпти ПОВИННІ посилатися на "the IDEA / the OUTLINE provided at the
    END of this message". НІКОЛИ не вставляй літеральні `{{TITLE}}`, `{{IDEA}}`,
    `{{OUTLINE}}` чи будь-який `{placeholder}` — код їх НЕ підставляє, вони лише
    збивають модель і провокують відповіді в стилі "ось твій генератор".

1.2 `outline` OUTPUT FORMAT — ВІЛЬНИЙ. Код його не парсить — передає сирим
    рядком у `story`-промпт. JSON рекомендований (чистий handoff), але дозволено
    будь-що. Обирай те, що найкраще служить ніші.

1.3 `story` OUTPUT — ТІЛЬКИ ЧИСТИЙ TTS-ТЕКСТ. TTS-рушій зачитує його дослівно.
    Тому `story`-промпт МУСИТЬ забороняти: заголовки, мітки, теги секцій, JSON,
    markdown, дужки, тире (em dash), круглі дужки, крапки з комою. Лише звичайні
    наративні абзаци.

1.4 ТРИ ІНВАРІАНТНІ СЕКЦІЇ — обов'язкові; можна тільки ДОПОВНЮВАТИ нішевими
    пунктами, ніколи не видаляти й не послаблювати базу:
    - "YOUTUBE CONTENT SAFETY — mandatory, overrides all other instructions:" (в `outline`)
    - "YOUTUBE CONTENT SAFETY:" (в `story`)
    - "TTS RULES:" (в `story`)
    Базовий текст (вшивати в кожен канал, розширювати — так, різати — ні):
      SAFETY baseline — no reference to people under 18 in any context; people
      who lost their lives or were harmed are described with dignity and
      restraint; no graphic descriptions of injury, death, or physical trauma;
      state the scale, state the consequence, move on; in `story` also ban the
      words: blood, gore, kill, murder, suicide, torture, execution, massacre,
      slaughter, corpse, body, remains, wound, drown, disfigure — replace with
      neutral language; assign responsibility through documented facts, not
      charged adjectives.
      TTS baseline — only the final narrative text; no headings/labels/tags; no
      em dashes; no parentheses; no semicolons; spell out symbols ("percent",
      "and"); no abbreviations; numbers under ten as words; years as numerals;
      one main idea per sentence.

1.5 ANTI-ARTIFACT — обидва промпти МУСЯТЬ закінчуватися інструкцією такого виду:
    "Respond directly with the [outline / script] for THIS [idea / outline],
    even if it is sparse — infer reasonable specifics rather than asking or
    deferring. Do NOT build a tool, app, generator, or UI. Do NOT describe what
    you will do. Output only the [outline / script], with no preamble."

════════════════════════════════════════════════════════════════════════════
2. BRIEF — що питати при заведенні нової ніші (запитуй лише відсутнє)
════════════════════════════════════════════════════════════════════════════
- niche: жанр + аудиторія, одне речення.
- narrator: голос + POV (first/second/third person) + характер.
- tone: 3-5 слів (напр. "awe and precision", "warm and direct", "dry skeptical").
- language: мова виходу (за замовч. English).
- target_length: chars для outline-скрипта і для фінального скрипта.
- is_narrative: ця ніша розповідає ІСТОРІЮ з центральним суб'єктом і аркою
  (true crime, історичні події, корпоративні крахи, космокатастрофи) — YES — чи
  вона не-наративна (how-to, листікли, фінанс-поради, новинні дайджести) — NO?
- anchor: якщо наративна — що тримає історію (named особа / компанія / кейс /
  подія) і як вона повертається в кінці; якщо не-наративна — лишити порожнім.
- recurring_device: опційне callback-слово, посаджене в хук, що повертається в
  кінцівці — on/off.
- fact_discipline: чи мають факти бути джерельними; якщо так — які типи джерел
  пасують цій ніші.
- rhythm: відчуття довжини речень під темп каналу.
- banned_phrases: 3-5 кліше специфічних для ніші, які заборонити.
- extra_safety: нішеві слова/теми, які додатково забанити (опційно).

════════════════════════════════════════════════════════════════════════════
3. UNIVERSAL CRAFT — у ОБИДВА промпти (не натягувати форму трагедії силою)
════════════════════════════════════════════════════════════════════════════
ЗАВЖДИ включати в обидва промпти:
- HOOK (2-3 речення, ~10 сек): без розгону, без "Imagine", без імператива до
  глядача, завершується на відкритій напрузі, ніколи не анонсує тему.
- zero-filler discipline: кожне речення несе факт, контраст/іронію, або занурює
  глядача в момент із фактичною вагою; інакше — видалити.
- три інваріантні секції (розділ 1.4) + anti-artifact рядок (розділ 1.5).
- HOOK ANTI-PATTERNS — заборонити завжди:
  "In [year], no one could have imagined...", "What happened next would change
  everything...", "This is the story of...", "By the end of this video you
  will...", будь-яке речення, що анонсує тему замість занурення в неї.
- BANNED PHRASES: підставити 3-5 кліше з `brief.md` цієї ніші.
- RHYTHM: підставити відчуття ритму з `brief.md`.

- AUTHENTICITY / ANTI-INAUTHENTIC (вимога YouTube з 2025; вшивати в ОБИДВА
  промпти, бо інакше канал ризикує позначкою "inauthentic / mass-produced"):
  YouTube вважає неавтентичним шаблонний, конвеєрний контент без оригінальної
  цінності та авторського бачення (мінімальні зміни між відео, слайдшоу без
  сенсу, простий voiceover чужих матеріалів, передрук новин без переробки).
  Тому КОЖЕН скрипт МУСИТЬ:
  1. ADD VALUE — нести знання, інсайт, інтерпретацію або розвагу, а не лише
     переказувати факти. Має бути ВИДНО, навіщо це відео існує.
  2. AUTHORIAL VOICE — присутність автора з власною ДУМКОЮ: явні судження,
     оцінки, гіпотези, чесні застереження ("here's my honest opinion", "what
     fascinates me", "the part I'd push back on"). Не нейтральний реферат.
  3. TRANSFORM, NOT RESTATE — якщо матеріал спирається на чужі джерела/новини,
     значно переробляти: новий кут, синтез кількох фактів у тезу, аналогії,
     порівняння, висновок, якого немає в джерелі.
  4. ANTI-TEMPLATE — уникати конвеєрного відчуття: не починати кожне відео
     однаковим шаблоном-реченням; варіювати хук, порядок розкриття, приклади.
     Дві серії поспіль не мають читатися як заповнена та сама форма.
  5. ORIGINAL THESIS — кожне відео тримає одну авторську тезу/точку зору, а не
     просто список фактів. Це і є "authorial component", якого вимагає YouTube.
  Нішевий brief може ПОСИЛИТИ цей пункт (напр. указати, ДЕ саме автор вставляє
  свою думку), але не послабити.

════════════════════════════════════════════════════════════════════════════
4. is_narrative SWITCH — головний важіль універсальності
════════════════════════════════════════════════════════════════════════════
ЯКЩО is_narrative = YES:
  включити anchor-element thread (opening / middle / closing), fact-integrity
  per block, optional ironic-loop (якщо recurring_device on), macro→micro "zoom",
  immersive-scene variety, paragraph-ending tension rotation (open question /
  suspended action / contrast / quiet detail / time-or-scale shift — ніколи двічі
  поспіль), і self-check блок у `story`-промпті.

ЯКЩО is_narrative = NO:
  ВИКИНУТИ anchor-element, ironic-loop, immersive-scene та accountability модулі.
  Замінити структуру тим, що потрібно ніші (numbered points, problem→method→
  payoff, claim→evidence→takeaway). Лишити hook, zero-filler, rhythm, banned
  phrases, три інваріантні секції та anti-artifact. НЕ приробляти сюжетну арку до
  контенту, в якого її нема.

════════════════════════════════════════════════════════════════════════════
5. REFERENCE SKELETON — `outline` (наративні ніші; [BRACKET] = з brief.md)
════════════════════════════════════════════════════════════════════════════
You are an expert scriptwriter for a YouTube channel about [NICHE].

Channel style:
- Voice: [NARRATOR]
- Tone: [TONE]
- Every claim must be [FACT_DISCIPLINE]
- If uncertain: use phrases like "reports suggest", "available evidence
  indicates", "no public record confirms".
- Emotion comes from [WHERE_EMOTION — contrast / stakes / irony].

TASK:
The IDEA for this specific video is provided at the very END of this message
(the software appends it after this prompt as "Idea: ..."). Generate a
structured outline for a [OUTLINE_TARGET_LENGTH] YouTube script based on THAT
idea. You decide the structure and the number of blocks. Build the outline
around what this specific story needs, not around a template.

FIXED REQUIREMENTS:
1. HOOK — 2-3 sentences, ~10s, no warm-up, ends on unresolved tension, no
   "Imagine"/imperative, never announces the theme. [if recurring_device on:
   plant one word here that returns in the closing — label it ironic_loop_word.]
2. ANCHOR ELEMENT — [ANCHOR]. Its arc must [SAFETY_CONSTRAINTS].
3. FACT INTEGRITY per block — every key fact carries its source basis
   [SOURCE_TYPES]; uncertain claims flagged [UNCERTAINTY_PHRASES]; unsourceable
   facts reframed or removed.

YOUTUBE CONTENT SAFETY — mandatory, overrides all other instructions:
[SAFETY baseline from 1.4 + extra_safety]

OUTPUT FORMAT: [free — JSON recommended; design the schema the story prompt will
consume: title, hook(+ironic_loop_word), anchor_element, blocks[focus/key_facts/
transition], closing].

[ANTI-ARTIFACT line per 1.5, outline variant.]

════════════════════════════════════════════════════════════════════════════
6. REFERENCE SKELETON — `story` (наративні ніші; [BRACKET] = з brief.md)
════════════════════════════════════════════════════════════════════════════
You are writing a full YouTube script in [LANGUAGE] based on the OUTLINE provided
at the very END of this message (appended as "Outline: ..."). Produce one
continuous script of ~[STORY_TARGET_LENGTH], ready for TTS, no structural labels.

ZERO TOLERANCE FOR FILLER: every sentence delivers a fact, creates contrast/irony,
or places the viewer in a factual moment; else delete it.

CORE TECHNIQUES (наративні): three-layer hook; anchor-element thread (opening/
middle/closing, show not explain); macro→micro zoom; anchor scene as one unbroken
passage ending on a quiet unanswerable line; [if recurring_device on] ironic loop
returns in closing, unexplained; sentence rhythm [RHYTHM]; show-don't-tell
accountability [adapt/drop for non-investigative].

STYLE: Voice [NARRATOR]; tone [TONE]; numbers carry contrast; no restatements;
each paragraph ends on tension rotating through UNANSWERED QUESTION / SUSPENDED
ACTION / IRONIC CONTRAST / QUIET DETAIL / TIME-OR-SCALE SHIFT (never same type
twice in a row).

BANNED PHRASES: [BANNED_PHRASES] + opening a scene with weather + closing on a
rhetorical question + anaphora as filler.

IMMERSIVE SCENE STRUCTURE: each scene a different opening — sensory / object /
action / absence / witness — never repeat within one script.

YOUTUBE CONTENT SAFETY:
[SAFETY baseline from 1.4 + extra_safety, story variant with banned words list]

TTS RULES:
[TTS baseline from 1.4 + any niche additions]

STRUCTURE: HOOK (three short paragraphs, no labels); BRIDGE (one sentence ≤20
words naming the payoff); BLOCKS (continuous prose in outline order, broken into
25-30 word chunks, no labels); CLOSING (reflection returning to anchor, then
ironic-loop echo, end in silence; final sentence is the narrator's own presence).

SELF-CHECK BEFORE OUTPUT: filler / structure / facts / safety / rhythm all pass.

[ANTI-ARTIFACT line per 1.5, story variant.]

════════════════════════════════════════════════════════════════════════════
7. SELF-CHECK перед видачею двох промптів (правити, поки всі не пройдуть)
════════════════════════════════════════════════════════════════════════════
[ ] ніде нема `{{TITLE}}`/`{{IDEA}}`/`{{OUTLINE}}` і жодних `{placeholders}`
[ ] кожен промпт посилається на IDEA / OUTLINE, дописані в кінці
[ ] всі три інваріантні секції присутні, база ціла, лише розширена
[ ] `story` забороняє не-TTS вихід (заголовки/JSON/markdown/тире/дужки/;)
[ ] anti-artifact інструкція в кінці ОБОХ промптів
[ ] скелет відповідає is_narrative (без насильної арки на не-наративі)
[ ] banned_phrases і rhythm підставлені з brief.md цієї ніші

════════════════════════════════════════════════════════════════════════════
8. COMPETITOR ANALYSIS METHODOLOGY (Mode B — як розбирати конкурентів)
════════════════════════════════════════════════════════════════════════════
Виведено з реального розбору ніші china_tech. Застосовувати ДО КОЖНОГО
конкурента, незалежно від ніші. Мета — не копіювати контент, а витягти
ПАТЕРНИ, що підсилять промпти. Усе писати в `competitors.md` цієї ніші.

8.1 СИГНАЛ ПЕРЕГЛЯДІВ → нішевий фокус (робити ПЕРШИМ)
  - Оператор зазначає перегляди (часто в назві файлу). Скласти таблицю
    "перегляди → тема/формат".
  - Знайти СОЛОДКУ ТОЧКУ: що саме в топах (тема, кут, тип героя, антагоніст).
  - Знайти АНТИ-ПАТЕРН: які теми/формати ПРОВАЛИЛИСЬ (офф-ніша, абстракція,
    відсутність відчутного "героя"). Це так само цінно, як і перемоги.
  - Вивід одним реченням: формула, що корелює з переглядами.

8.2 ОДИН КОНКУРЕНТ ЗА РАЗ, кілька скриптів кожен
  - Назвати "школу" каналу (його окремий стилістичний підхід).
  - Якщо конкурентів кілька — РАНЖУВАТИ їх і питати оператора, який #1
    (еталон для емуляції).

8.3 ОСІ РОЗБОРУ (проходити по кожній для кожного каналу):
  - HOOK: з чого починає (сцена / число / парадокс / питання); скільки частин;
    чи є pivot-обман; чи є roadmap; чим завершує.
  - STRUCTURE: як побудовано тіло (ескалація / вкладені викриття / numbered /
    claim-evidence / лекція-питання). Які зшивки між блоками.
  - DEVICES: повторювані прийоми — тріадне обрамлення, анафора, callback-слово,
    аналогія-на-абстракцію, tally до/після, епіграма-закриття, cross-reference
    власних відео.
  - FACT-DISCIPLINE: чи джерельні факти; named-джерела; дати; числа В КОНТРАСТІ;
    рівень хеджування vs сміливі твердження.
  - RHYTHM: чергування коротких/довгих речень; на чому закінчуються речення.
  - TONE: 3-5 слів (трилер / аналітик / скептик / awe+dread).
  - ANCHOR / THEME: наскрізний протагоніст або теза; іронічна петля; чи
    повертається в кінці.
  - AUTHENTICITY: де автор вставляє ВЛАСНУ думку; чи це реферат чи авторська
    позиція; як трансформує чужий матеріал (це прямо живить розділ 3 ADD VALUE).
  - CTA / RETENTION: як просить підписку/коменти; binge-гачки.

8.4 ПО-СКРИПТОВИЙ РОЗБІР
  - Для кожного скрипта 1-2 рядки: що саме спрацювало і ЯК це привʼязано до
    переглядів. Цитувати влучні фрази дослівно (вони — взірець голосу).

8.5 КОЛІЗІЯ З GENERAL_RULES (обовʼязкова перевірка)
  - Явно зафіксувати, ДЕ переможний стиль конкурента порушує наші універсальні
    правила (особливо HOOK anti-patterns: імператив, "By the end…", "Imagine").
  - НЕ вирішувати самому — винести оператору: (а) тримати наші правила і
    програти в стилі, чи (б) зробити нішеве виключення в brief.md. Рішення
    записати в brief.md як підтверджене оператором.

8.6 СИНТЕЗ
  - Якщо шкіл кілька — таблиця-порівняння по осях 8.3.
  - Назвати ЕТАЛОННУ модель і сформулювати, що саме з неї беремо в промпти.

8.7 ДИСЦИПЛІНА ЗАПИСУ
  - competitors.md = ПАТЕРНИ, не сам контент (не передруковувати скрипти).
  - Зберігати на диск проактивно (контекстне вікно може скінчитись), але
    дотримуватись WRITE-ONLY-AFTER-"зберігай" правила для дозволу оператора.
  - Розбори накопичувати, не перезаписувати: нова інформація ДОПОВНЮЄ.

8.8 MATCH-AND-BEAT (коли оператор каже «зроби краще за конкурента»)
  Мета не копія, а: (1) наше відео мусить подобатись АУДИТОРІЇ конкурента
  (та сама дофамінова механіка утримання), (2) і бути КРАЩИМ. Тому для кожної
  виявленої фішки конкурента будувати рядок таблиці match-and-beat:
    | Вісь | Що робить конкурент | Наша КРАЩА версія |
  «Краща версія» = одне з: щільніше (різати bloat), свіжіше (не з банку метафор
  конкурента), чесніше (хедж раніше й гостріше), авторськіше (думка в тілі, не
  лише у фіналі), різноманітніше (не повторювати ту саму зшивку двічі). НІКОЛИ
  не «краще» через гучніші прикметники — це програш.

8.9 RETENTION-ОСІ (додаткові осі до 8.3, спеціально про утримання)
  - ДЕФЛЯЦІЙНИЙ ДВИГУН: чи знецінює канал щойно подану сенсацію, щоб підняти
    наступний шар; якими зшивками («the real story is narrower», «that does not
    mean…»). Це часто головний механізм утримання, а не хук.
  - BALANCE-AS-TRUST: чи показує і де герой ВИГРАВ, і де ПРОГРАВ (баланс =
    валюта довіри проти чисто-трилерних каналів).
  - DIVIDE-CTA: чи дає глядачу дві сторони (A-чи-B) для суперечки в коментах —
    це ютуб-сигнал залученості, не просто «підпишись».
  - CAVEAT-COUNT: скільки пронумерованих застережень і ДЕ (рано/вплетено vs
    звалено в кінець). Кількість плаває (3-4) — не вважати жорсткою трійкою.

8.10 ПРІОРИТЕТ РЕФЕРЕНСУ
  - Якщо оператор називає канал, який «ютуб просуває» → це РЕФЕРЕНС №1, еталон
    емуляції механіки утримання (не стилю слово-в-слово). Інші конкуренти —
    допоміжні. Фіксувати, ХТО еталон, у competitors.md.

8.11 BEAT-THE-REFERENCE → FINGERPRINT-КАРАНТИН
  - Виявити FINGERPRINT-закриття/зшивку еталона (повторюваний шаблон у ВСІХ його
    відео, напр. «X did not win by Y. It won by proving Z»). Занести в карантин:
    НАШИМ каналам цей шаблон ЗАБОРОНЕНИЙ — кожному дати власний ritual word і
    живу кінцівку (див. нішевий channels.md DE-FINGERPRINT MATRIX). Інакше наші
    канали читатимуться як клон еталона.
