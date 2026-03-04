# TODO (без "attempts")

> Структура этого репо — единая точка правды. Старые отдельные research-репозитории удалены; ссылки на них вычищены.

## ✅ Done

- Собраны и сведены материалы по Yandex Games (исследование/снапшот лежат в `research/`).
- Проверена совместимость требований: Unity 2022.3 LTS, WebGL, YG SDK.
- Сформированы базовые требования к core loop / жанру / механикам (см. `requirements/core_loop_requirements.md`).
- Подготовлен шаблон feature-matrix для shortlist-10 (см. `requirements/shortlist_10_feature_matrix.md`).
- Подготовлен high-level чеклист интеграции YG SDK (см. `spec/06-yg-sdk-integration.md`).

## 📌 To do

### A) Выбор 10 игр (результат ресерча)
- Заполнить `requirements/shortlist_10_feature_matrix.md` реальными 10 тайтлами.
- Зафиксировать для каждой игры: тип (endless/campaign), core loop, мета, монетизация (rewarded/interstitial/IAP), лидерборд.

### B) Delivery
- Разбить работу на milestones и задачи (GitHub milestones + issues).
- Определить Definition of Done на 1 игру (чеклист релиза) и применять его ко всем 10.

### C) YG SDK (детализация)
- Законспектить конкретные API/обёртки и примеры кода (как минимум: ads, iap, cloud, leaderboards, auth/lang).

---

## Research (браузерные референсы / shortlist 10)

Ссылки на рабочие файлы:

- Sources: `research/00-sources.md`
- Capture template: `research/10-capture-template.md`
- Candidates: `research/20-candidates-raw.md`
- Clusters: `research/30-clusters.md`
- Shortlist 10: `research/40-shortlist-10.md`

### 1) Снятие витрин и топов (накопление сырья)

- [ ] Пройтись по витринам: Yandex Games / Poki / CrazyGames / MSN Play (минимум 30–50 игр суммарно)
- [ ] Пройтись по внешним топам/подборкам из `00-sources.md` (ещё 20–40 игр)
- [ ] Для каждой игры заполнить строку по шаблону (URL, жанр, core mechanic, loop, мета, монетизация, leaderboard)
- [ ] Перенести все находки в `20-candidates-raw.md` и проставить `status=new`

### 2) Нормализация данных (чтобы можно было сравнивать)

- [ ] Привести названия механик к единому словарю (пример: merge / match / shooter / runner / idle / sim / puzzle)
- [ ] В `20-candidates-raw.md` проставить `endless/campaign` и `meta (да/нет/?)`
- [ ] Для спорных кейсов: отметить `?` и добавить заметку «нужно проверить в игре»

### 3) Кластеризация

- [ ] Сформировать кластеры в `30-clusters.md`: `(mode) + (core mechanic)`
- [ ] В каждом кластере перечислить 3–10 игр (ссылки/названия)
- [ ] Пометить кластеры, которые лучше всего соответствуют целевому core loop

### 4) Проверка обязательных фич (по требованиям)

Ориентиры: `requirements/monetization_requirements.md`, `requirements/meta_requirements.md`, `requirements/shortlist_10_feature_matrix.md`.

- [ ] Для топ-кандидатов запустить игру и верифицировать:
  - [ ] rewarded ads
  - [ ] interstitial ads
  - [ ] IAP
  - [ ] leaderboard
  - [ ] meta progression
- [ ] Обновить строки в `20-candidates-raw.md` и `40-shortlist-10.md`

### 5) Сбор shortlist 10

- [ ] Выбрать **5 endless + 5 campaign** (разные кластеры, без дублей по механике)
- [ ] Заполнить `40-shortlist-10.md` + итоговую матрицу 10x5
- [ ] Для каждой игры добавить 1–2 предложения: «почему это сильный референс»

### 6) Фиксация результата

- [ ] Обновить `research/yg-research-merged.md` (короткий human-readable summary + ссылки на таблицы)
- [ ] Сделать снапшот в `research/yg-research-merged-snapshot.md` (дата MSK, ref/commit, заметки)
