# HANDOFF — china_tech

Передача контексту наступному агенту/собі. Repo — єдине джерело правди (Claude НЕ памʼятає між сесіями; усе, чого немає у файлах, втрачається).

---

## Сесія 2026-06-27/28 — Veyron (9-й) + AetherEast (10-й) авторовано + EE «два формати» + опис для lotus

### Що зроблено (усе запушено: commit `4df0f5c`, Marchkkkk/AgentNiches, main)
1. **Veyron** (`prompts/veyron.md`) — авторовано всі 3 блоки. Движок **THE RACE in legs**. Довжина піднята до **~14000 знаків / ~2300 слів / макс 15000 / ~15 хв** (новий стандарт довжини, більший за lotus 7500 та jade 8000 — оператор попросив «хватало на 15 хв»).
2. **ideas_veyron.md** — 3 ідеї (Intel / ASML / Nvidia), усі RACE-SHAPED. Idea A (Intel node race) = пріоритет.
3. **AetherEast** (`prompts/aether_east.md`) — авторовано всі 3 блоки. Движок **MAP OF THE INVISIBLE NETWORK**. Та сама довжина 14k/15хв. Файл ідей ШЕ НЕ створено (наступний крок, якщо треба).
4. **competitors.md** — дописано блок «EASTERN ENGINE — ВІДКРИТТЯ ДВА ФОРМАТИ (2026-06-27)»: EE має РОДИНУ форматів, не один.
5. **Опис для відео lotus_terminal** «Nvidia Won the Chip. China Bought the POWER PLANT» — видано в чат (повний + короткий варіант). НЕ збережено у файл (оператор не просив зберегти; теми описів поки живуть у чаті).

### Veyron — паспорт (de-fingerprint)
- **Движок:** контест ДВОХ ГОДИННИКІВ (named-гігант vs Китай), бігається по LEGS; кожен leg = вимір (design/manufacturing/materials/software/scale); кожен leg закривається на **SPLIT-TIME** (head-to-head читання часу/темпу: час Заходу, тоді Китаю, в одному граматичному фреймі); lead стискається leg-to-leg; один leg перевертає тренд (honest brake).
- **Наратор:** first-person race-caller / momentum analyst. Present tense, clipped, propulsive. Емоція = ШВИДКІСТЬ (не цікавість jade, не awe+dread lotus).
- **Ритуал:** SPLIT-TIME readout наприкінці кожного leg.
- **Лексикон ВОЛОДІЄ:** track-and-clock — the lead, the gap, gaining a lap, the split, who reaches the line first, years vs months.
- **Honest brake:** leg де годинник Китаю лише ЗДАЄТЬСЯ швидким (yield, frontier node, EUV, ecosystem lock-in).
- **Закриття:** FINISH-LINE FORECAST (12-міс call + forward-looking comment-bait + subscribe).

### AetherEast — паспорт (de-fingerprint)
- **Движок:** КАРТА прихованої мережі залежностей, малюється наживо. Трасуємо лінії node-to-node поки не впремося в **CHOKEPOINT** (один матеріал/інструмент/софт, контрольований однією компанією/країною); на кожному вузлі читаємо чи є **BYPASS**.
- **Наратор:** first-person картограф мережі / систем-мапер. Спокійний, методичний, ПРОСТОРОВИЙ (мислить зв'язками/структурою, не швидкістю — це головна різниця з Veyron).
- **Ритуал:** TRACE THE LINE — кожен сегмент закінчується NODE READOUT (назва вузла + статус bypass: немає / будується / вже обійдено) в одному фреймі.
- **Лексикон ВОЛОДІЄ:** node, line, chokepoint, junction, valve, web, single point of failure, bypass, dead-end, the far end of the line.
- **Topic tilt (УНІКАЛЬНИЙ шар):** МАТЕРІАЛИ + ІНСТРУМЕНТИ + СОФТ під чіпом — літографія (ASML), photoresist, гази, підкладки, deposition/etch (Applied Materials, Lam, Tokyo Electron), EDA (Synopsys, Cadence), Shin-Etsu. Named-гіганти тут = toolmakers, не chipmakers. Це окремий тематичний шар від решти каналів.
- **Honest brake:** THE DEAD-END — вузол, який Китай реально не може обійти (EUV, специфічний photoresist, EDA-софт).
- **Закриття:** MAP-COMPLETE reading (що обійдено / що лишилось + call + питання + subscribe).
- **КРИТИЧНІ банни для AetherEast:** Veyron split-time/race-мова; lotus «wall became a map» (бо AetherEast юзає БУКВАЛЬНІ карти — фігуральна метафора-бар'єр заборонена); silk «upstream» (каже «the far end of the line»); + НОВЕ: **spoken chapter headers** (див. нижче).

### EE «ДВА ФОРМАТИ» — головне відкриття сесії (для competitors.md + de-fingerprint)
Оператор залив 2 EE-скрипти (Qualcomm HBM-Free + China Banned Nvidia). Висновок: EE = РОДИНА форматів зі спільним «honest-broker» ДНК:
- **Формат 1 (драматичний реверс):** імператив-hook, АКТ-структура вголос («Act one belonged to America… then the twist»), народні метафори гронами, «three forces», A/B divisive CTA. Стиль SinoShift.
- **Формат 2 (грунтовний пояснювач):** тиха тех-аксіома-hook, **РОЗДІЛОВІ ЗАГОЛОВКИ ВГОЛОС** («Why China matters», «The honest catch», «My take») = головний fingerprint цього режиму, ОДНА центральна аналогія (не рефрен), надважке хеджування скрізь, нумерований «four caveats», «My take» блок. Стиль Katherine Johnson.
- **Спільне ДНК обох (МАШИНЕРІЯ, яку ютуб любить — беремо формат, не текст):** нумеровані caveats, «my take», A/B CTA, аутро «subscribe to Eastern Engine».
- **НОВИЙ БАН для всіх наших каналів:** spoken chapter headers (озвучені назви розділів). Наша навігація — тільки в ритуалі (split-time / trace-the-line / раунди), ніколи вголос названі секції. Додано в banned-блоки Veyron + AetherEast.

### Нова тематична хвиля (idea-sourcing, verify-at-script-time)
- HBM / memory-wall / near-memory compute (HBC) / LPDDR «телефонна память» в дата-центрі — гаряча. Перетин: jade Idea A (CXMT) + Veyron Idea C (HBM honest brake).
- НОВИЙ КУТ named-гіганта: **Qualcomm = ЗАХІДНИЙ гігант, що ВХОДИТЬ у Китай** під експорт-контролем (а не «Китай б'є Захід»). Свіжий ракурс.
- Microsoft/Meta = credibility-якорі; CUDA software moat = універсальний honest-brake матеріал.

### Стандарт довжини ЗМІНИВСЯ
Veyron + AetherEast = **14000 знаків / ~15 хв** (попередні канали: lotus ~7500, jade ~8000, решта ~10500-12000). Якщо оператор захоче єдиний стандарт — це відкрите питання, поки що нові канали довші.

### Notion
Оператор спитав про підключення Notion. Стан: конекторів НЕ встановлено, в реєстрі Notion нема. Підключає оператор САМ (`claude mcp add --transport http notion https://mcp.notion.com/mcp` + OAuth). Я НЕ можу додати конектор. Відкрите питання оператору: нащо саме Notion (дублювати описи/ідеї VS вести весь стан замість файлів) — застеріг, що розмазувати стан між Notion і git шкодить принципу «repo = єдине джерело правди».

### Відкриті кроки
1. (Якщо треба) `ideas_aether_east.md` — 3 ідеї (кандидати: ASML/EUV chokepoint, EDA Synopsys/Cadence, photoresist/гази Shin-Etsu/JSR).
2. Музичні промпти для Veyron (offered) + AetherEast — не зроблено.
3. Оператор САМ деплоїть нові промпти в прод `channels.json`.
4. Лишилось каналів без авторингу: перевірити `channels.md` (Veyron + AetherEast тепер готові; рахунок каналів = 10 з паспортами).

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
