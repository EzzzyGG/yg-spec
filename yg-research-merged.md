# yg research — merged into yg-spec

Собрано из репозиториев:
- https://github.com/EzzzyGG/yg4-top-research
- https://github.com/EzzzyGG/yg2-top-research

---

## yg4-top-research

### README.md

(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/README.md)

# yg4-top-research

Цель: собрать **воспроизводимый** список топ/популярных игровых проектов/популярных игр и механик (Яндекс Игры + внешние источники) и на его основе выбрать 10 направлений (5 endless + 5 campaign) для разработки Unity WebGL игр под **Яндекс Игры SDK**.

#### Версия топа
- `top_version`: **v0.1**
- `updated_at_utc`: 2026-03-03

### Источники (минимум)
- RU Popular: https://yandex.ru/games/category/editors_choice
- RU New: https://yandex.ru/games/category/new
- EN Popular: https://yandex.com/games/category/editors_choice
- EN New: https://yandex.com/games/category/new

### Методика
1. Фиксируем Top N (обычно 50) игр с каждой витрины: названия, ссылки, рейтинги (если есть), теги/жанры, тип (endless/campaign), 1–2 наблюдения по механикам.
2. Кластеризуем по механикам/жанрам (runner/obby/puzzle/merge/idle/survivor/td/driving/match/etc).
3. Считаем частоты и выбираем 10 направлений (5 endless + 5 campaign).
4. Документируем монетизацию/SDK-требования как инварианты.

### Артефакты (файлы)
- `data/top_sources.md` — источники (URL) и снимки
- `data/top_raw.md` — сырой список (таблица)
- `data/top_clusters.md` — кластеры и частоты
- `data/top_shortlist_10.md` — shortlist из 10 направлений + маппинг на SDK

#### data/top_sources.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_sources.md)

# Источники топа (yg4)
Дата фиксации: **2026-03-04 (MSK)**

| Source | URL | Captured at (MSK) | Captured at (UTC) |
|---|---|---:|---:|
| Yandex Games (RU) — Популярные | https://yandex.ru/games/category/editors_choice | 2026-03-04 | 2026-03-03 |
| Yandex Games (RU) — Новые | https://yandex.ru/games/category/new | 2026-03-04 | 2026-03-03 |
| Yandex Games (EN) — Popular | https://yandex.com/games/category/editors_choice | 2026-03-04 | 2026-03-03 |
| Yandex Games (EN) — New | https://yandex.com/games/category/new | 2026-03-04 | 2026-03-03 |

Внешние источники (кандидаты): Poki, CrazyGames, MSN Games, MMO13, Gameguru, mmoguider, hi-tech.mail.ru, FRVR, hakster, game-analytics.ru, mmobomb, gmodz, exputer, gfinity.

#### data/top_raw.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_raw.md)

# Сырой список top (yg4)
Шаблон таблицы (Top 50 / витрина):

| # | Game | URL | Source | Rating | Tags | Notes (genre/tags/mechanic) |
|---:|---|---|---|---:|---|---|

#### data/top_clusters.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_clusters.md)

# Кластеризация механик (yg4)

После заполнения `top_raw.md`:
- группируем игры по механикам
- считаем частоты
- отдельно отмечаем endless vs campaign

| Cluster | Examples | Count | Notes |
|---|---|---:|---|

#### data/top_shortlist_10.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_shortlist_10.md)

# Shortlist из 10 направлений (yg4)

Сюда попадает 10 направлений (5 endless + 5 campaign) после анализа `top_raw.md` и `top_clusters.md`.

| # | Direction | Type (endless/campaign) | Core loop | Meta progression | Monetization hooks (rewarded/interstitial/IAP) | Leaderboard? |
|---:|---|---|---|---|---|---|

---

## yg2-top-research

### README.md

(Источник: https://github.com/EzzzyGG/yg2-top-research/blob/main/README.md)

# yg2-top-research

Yandex Games: top lists snapshot + external comparisons + notes for replication (Unity 2022.3 LTS / YG SDK).
