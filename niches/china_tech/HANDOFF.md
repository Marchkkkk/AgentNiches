# HANDOFF — china_tech

Передача контексту наступному агенту/собі. Repo — єдине джерело правди (Claude НЕ памʼятає між сесіями; усе, чого немає у файлах, втрачається).

---

## Сесія 2026-06-26 (друга) — jade_protocol (8-й канал, авторовано) + lotus апдейт

### Що зроблено
1. **Промпти jade_protocol** (`prompts/jade_protocol.md`) — авторовано всі 3 блоки (outline / story / channel_profile). Канал ОБРАНО на движку **SLOW-UNRAVEL** (детектив), а не SinoShift-трилер.
2. **Файл ідей** (`ideas_jade_protocol.md`) — 2 трендові ідеї, обидві question-shaped.
3. **lotus_terminal** — channel_profile дозаписано (повний stock-finder профіль), outline+story перетягнуто на ~7500 знаків / 1200 слів (lean). prompts.md СВІДОМО не синхронізовано (вимога оператора «працюєм виключно з lotus»).

### Рішення по движку Jade (головне)
- Оператор: **SinoShift-движок (трилер-ескалація) йде слабо** на china-chip матеріалі. Діагноз: ескалація силує dread з дедуктивних фактів → Frankenstein-несумісність з нашою чесною фактологією.
- lotus уже ВОЛОДІЄ deflation-движком Eastern Engine (steelman + my-take + A/B CTA + мікро-дефляція). Клонувати не можна.
- Незайнята смуга = **«терплячий детектив» (Katherine Johnson school, але архітектура, не тики)**. Jade бере той самий чесний регістр, але іншу АРХІТЕКТУРУ.

### Jade Protocol — паспорт (de-fingerprint)
- **Движок:** ОДНЕ driving question у хуку, тримається весь скрипт; відповідь дається ТРИЧІ, кожна краща; фінал перевертає САМЕ ПИТАННЯ (воно було трохи не те).
  - Відмінність від lotus: lotus чистить ГЛИБШІ ШАРИ однієї правди (three nested reveals); Jade ПЕРЕВІДПОВІДАЄ на одне питання кращими відповідями, потім виправляє питання.
- **Наратор:** first-person слідчий. Cool, методичний, цікавий (не awe+dread як lotus, а інтрига+ясність).
- **Ритуал (підпис):** RETURN-QUESTION — питання повертається майже дослівно ПЕРЕД кожною новою відповіддю (замість callback-слова lotus).
- **Лексикон ВОЛОДІЄ:** LOCK-reading — «a restriction is a lock, and a lock tells you what was worth locking». Читаємо бан назад → він викриває намір. (НЕ «wall became a map» — то lotus.)
- **Метафора-родина:** lock / key / sealed door / decrypt (під назву Jade Protocol). Свіжа, нічия.
- **Закриття:** reframe-the-question (питання було не те → ось краще питання + відповідь). НЕ «wall became map» афоризм.
- **Довжина:** ~8000 знаків / 1300 слів / макс 9000 (трохи більше за lotus 7500 — slow-unravel треба простір тримати питання).
- **BANNED (чуже):** callback word / «not A but B» / three nested reveals / «but that isn't the real story» / «wall became map» (lotus); мікро-дефляція щореч (EE/lotus); «Round goes to X» (red_silicon); «Two. Two. Two.» + two-dates-delta (east_forge); «not X. It came from Y.» (neon); «establishes X / does not Y» + doc-двічі (eastbyte); cut-by-cut (silk); staccato sovereign-stack + «This was not X. This was Y.» (SinoShift — банимо, бо пробували, йде слабо).

### Ідеї Jade (`ideas_jade_protocol.md`)
- **A (пріоритет):** CXMT vs Samsung memory — рейс на ЖИВУ memory-shortage/AI-bottleneck хвилю (Eastern Engine щойно зробив це 2026-06-26 → ми робимо ТУ Ж хвилю іншим движком = authentic-but-viral «rewrite» хід). Питання: нащо наймолодший виробник ллє 5× нову потужність Samsung на піку циклу, що десятиліттями вбивав швидших?
- **B:** «Nobody banned Nvidia from China. Nvidia left anyway» (verified March 2026, з operator desktop file). Чистий puzzle: нащо Nvidia сама йде з ринку, на якому будувала імперію, до того як її змусили? Найкраща демонстрація reframe-close.

### Тренд-сигнал цієї сесії (новий скрипт Eastern Engine)
- «China's RAM Giant Adding 5X More Capacity Than Samsung — $4.3B IPO» (CXMT/DRAM). Підтверджує: EE-движок = deflation (закид→caveat→але важливо), explainer-сходи з питаннями-заголовками, «my take», A/B CTA, число-в-контраст-парі. Memory = новий AI bottleneck → найгарячіша свіжа рамка. Це паливо для Idea A.

### Відкритий крок
- Оператор САМ деплоїть jade_protocol + lotus_terminal у прод `channels.json` (локальний не чіпаємо).
- Перший прогон Jade рекомендовано на Idea A (валідує движок + same-trend-different-engine хід).

---

## Сесія 2026-06-26 — quantum_rivals (7-й канал, добудовано)

### Що зроблено
1. **Промпти quantum_rivals** (`prompts/quantum_rivals.md`) — додано «balance-as-trust» / clean-loss апгрейд у всі 3 блоки (outline beat 3, story VOICE, FINAL CHECKLIST item, JSON-схему weighings з полем `clean_loss`). Вимога: в ОДНОМУ зважуванні фаворит-ставка ПРОГРАЄ за конкретною названою метрикою (efficiency/fidelity/gate speed/logical-qubit overhead/reproducibility/cost), подано рівно, без відігравання назад. Це головний trust-механік Eastern Engine. Dry-run підтвердив, що b'ється органічно (weighing 3 у Zuchongzhi-vs-Willow).
2. **Файл ідей** (`ideas_quantum_rivals.md`) — СТВОРЕНО і провалідовано попитом. 9 ідей + 3 секції: DEMAND VALIDATION (vidiq), TREND ALIGNMENT (Eastern Engine 5 свіжих скриптів), BANNED-BUT-HIGH-DEMAND.

### Ключові висновки по попиту (vidiq, 2026-06-26)
- **«china quantum computer» = пошук ≈ 0.** Квант НЕ тягне сам. Демандовий двигун ніші = tech-war: **«china chip war» ≈ 5314/міс** + china-vs-America. Квант мусить їхати на цій рамці. Назви машин (Zuchongzhi тощо) шукають ≈ 0 → в anchor, НЕ в тайтл.
- **Топ breakout-сигнал = quantum-vs-AI-data-center** (≈248k+70k). Аудиторія ніші одержима Nvidia/GPU/data-центрами → це міст у квант. → ідея #8 (найвища стеля).
- **Microsoft топологічний/Majorana кубіт** = жива high-demand смуга (≈275k+258k). → ідея #9.
- **Q-Day / «зламати інтернет» (≈421k)** — НАЙВИЩИЙ квант-попит, але це заборонена decryption-рамка. Свідомо НЕ робимо (залоговано в BANNED-BUT-HIGH-DEMAND).
- Свіжі машини для anchor'ів (старі застаріли): Jiuzhang 4.0, Origin Wukong, Hanyuan dual-core / neutral-atom.

### Тренд ЗАРАЗ (Eastern Engine, 5 скриптів 2026-06-25)
Його найновіший хіт = **«No-GPU Supercomputer #1»** (Китай #1 за exaflops, обходить GPU, контраст-пара + caveat'и). Вектор тренду = «Китай обходить очевидний інструмент обчислень без нього» (no DUV / no GPU / no ASML) → прямо підсилює ідею #8. Плюс: дефляційний двигун довіри = механічно наш clean-loss; A-чи-B CTA = native для two-bets (закривати відкритим питанням, не вердиктом).

### Пріоритет продакшну
#1 (валідований dry-run) → #8 (стеля + у тренді) → #6 (keyword «chip war») → #9 → #5 → #3.

### Відкритий крок
- Оператор САМ деплоїть пару промптів quantum_rivals у прод `channels.json` (локальний channels.json НЕ чіпали — за вимогою оператора). Файл ідей готовий як вхід для авторингу скриптів.

---

## Сесія 2026-06-19 (6 базових каналів)

## Що зроблено цієї сесії

1. **Записано 9 повних SRT-скриптів конкурентів** у `competitors.md` — накопичено поверх попередніх самарі (не перезаписано), додано блок «ЗБАГАЧЕННЯ З ПОВНИХ СКРИПТІВ» з дослівними прийомами/епіграмами/числами + «НОВІ КРОС-ПАТЕРНИ» для де-фінгерпринту.
2. **Авторовано пер-канальні промпти для ВСІХ 6 каналів** → `prompts/*.md`. Кожен файл = шапка (скелет/наратор/ритуал/банні/намір) + ```-fenced `## prompts.outline`, `## prompts.story`, `## channel_profile`.
3. **Записано уроки** → `lessons.md` (блок «Авторинг 6 пер-канальних промптів»).
4. **Оновлено `channels.md`** — статус TODO + таблиця «ФАЙЛИ ПРОМПТІВ».
5. **Запушено на GitHub** (`Marchkkkk/AgentNiches`, main, commit `efff4c8`).

## Ключовий принцип де-фінгерпринту

Структурна різниця НЕ достатня — голос прози має розходитися на РІВНІ РЕЧЕННЯ. Найсильніший важіль = BANNED DEVICES (заборонити кожному каналу фірмові прийоми інших), не лише дозволи.

Промпт = 2 шари:
- **ІНВАРІАНТ ніші** (дослівно однаковий у всіх 6): FACT INTEGRITY, YOUTUBE CONTENT SAFETY, TTS-деабревіація, FINAL CHECKLIST, hook-anchor-first, теза «обмеження=карта/каталізатор».
- **ДИФЕРЕНЦІАЛ на канал**: VOICE/THESIS, скелет REQUIRED BEATS, ритуальне слово, RHYTHM, CTA, channel_profile-tilt.

## Матриця 6 каналів (один прийом = один власник)

| Файл | Двигун | Наратор | Ритуал | Головна заборона |
|---|---|---|---|---|
| `lotus_terminal.md` | ЕТАЛОН: 3 вкладені reveal + callback-слово | — | callback word | (базовий, дозволено «not A but B») |
| `red_silicon.md` | claim/counterclaim РАУНДИ, судить | analyst-judge 3-я особа | «Round goes to X» | callback, «not A but B», number-drumbeat, інверсія, антитеза |
| `silk_circuit.md` | розтин ОДНОГО обʼєкта cut-by-cut | клінічний | повні рівні речення (БЕЗ фрагментів) | фрагменти, раунди, callback, drumbeat, інверсія, антитеза, «not A but B» |
| `east_forge.md` | дві дати → ДЕЛЬТА | вимірювач | «Two. Two. Two.» (повтор числа) | раунди, callback, інверсія, антитеза, «not A but B», «per [source]» спам |
| `neon_frontier.md` | причинний ЛАНЦЮГ на драбині певності | репортер | «not X. It came from Y.» (інверсія) | callback, раунди, drumbeat, антитеза, «load-bearing» (вирізано) |
| `eastbyte.md` | ОДИН документ читається ДВІЧІ (каже / не каже) | документаліст | «establishes X / does not Y» (антитеза) | фрагменти, callback, раунди, drumbeat, інверсія, «structural» (вирізано) |

Власники прийомів: карбовані фрагменти → red_silicon + neon + east_forge(лише на дельті). «not A but B» → лише lotus. Довжина: neon найкоротший (~10000/11500), решта ~10500/12000.

EXECUTE-not-NAME: жоден story-промпт не називає прийом уголос («the hook», «the reveal» тощо).

## Ризики ніші (памʼятати)

- False precision: макс 5 твердих чисел/скрипт, кожне з хеджем; named-research з майбутніми датами = фактчек у коментах.
- Спільна метафора «барʼєр став X» протікає у всіх конкурентів — вимога свіжих родин метафор.
- TTS-деабревіація додає однорідності, але правило не ламати.

## Відкриті наступні кроки

1. Вставити 6 пар промптів у ClaudeAssist `channels.json` (`prompts.outline` + `prompts.story` + `channel_profile`).
2. Battle-validation: прогнати одну ідею через 2-3 канали, перевірити що голоси різні на рівні речення.
3. (Опц.) Файл «decisions rationale» — щоб наступний агент мав і «що», і «чому».

## Три школи конкурентів (орієнтири)

- SinoShift — геополітичний трилер (numeric contrast-fragment — їхній підпис).
- Katherine Johnson — нюансований лонгформ-аналітик.
- Eastern Engine ⭐ — чесний скептик, референс №1 оператора.
