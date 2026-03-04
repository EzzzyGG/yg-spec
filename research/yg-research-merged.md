# yg research — merged into yg-spec

Собрано из репозиториев:
- https://github.com/EzzzyGG/yg4-top-research
- https://github.com/EzzzyGG/yg2-top-research

---

## yg4-top-research

### README.md

(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/README.md)

# yg4-top-research

Цель: собрать **воспроизводимый** список топ/популярных игровых проектов/популярных игровых игр и механик (Яндекс Игры + внешние источники) и на его основе выбрать 10 направлений (5 endless + 5 campaign) для разработки Unity WebGL игр под **Яндекс Игры SDK**.

#### Версия топа
- `top_version`: **v0.1**
- `updated_at_utc`: 2026-03-03

### Источники (минимум)
- RU Popular: https://yandex.ru/games/category/editors_choice
- RU New: https://yandex.ru/games/category/new
- EN Popular: https://yandex.com/games/category/editors_choice
- EN New: https://yandex.com/games/category/new

### Методика
1. Фиксируем Top N (обычно 50) игр с каждой витрины: название, ссылка, рейтинг (если есть), теги (если есть), примечания.
2. Классифицируем по механикам/жанрам/типу (endless/campaign).
3. Составляем shortlist 10 направлений (5 endless + 5 campaign).
4. Документируем монетизацию/SDK-требования.

#### Артефакты (файлы)
- `data/top_sources.md` — источники (URL) и снимок времени
- `data/top_raw.md` — сырая таблица top
- `data/top_clusters.md` — кластера по механикам
- `data/top_shortlist_10.md` — shortlist 10 направлений

### data/top_sources.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_sources.md)

# Источники топа (yg4)
Дата фиксации: **2026-03-04 (MSK)**

| Source | URL | Captured at (MSK) | Captured at (UTC) |
|---|---|---:|---:|
| Yandex Games (RU) — Популярные | https://yandex.ru/games/category/editors_choice | 2026-03-04 | 2026-03-03 |
| Yandex Games (RU) — Новые | https://yandex.ru/games/category/new | 2026-03-04 | 2026-03-03 |
| Yandex Games (EN) — Popular | https://yandex.com/games/category/editors_choice | 2026-03-04 | 2026-03-03 |
| Yandex Games (EN) — New | https://yandex.com/games/category/new | 2026-03-04 | 2026-03-03 |

Внешние источники (кандидаты):

| Source | URL | Notes |
|---|---|---|
| Poki | https://poki.com/ | Top/Popular browser games |
| CrazyGames | https://www.crazygames.com/ | Top/Trending browser games |
| MSN Games | https://www.msn.com/ru-ru/play | Browser catalog |
| MMO13 (browser, 2026) | https://mmo13.ru/games/top/platform-71/year-2026 | External list |
| Gameguru (browser 2026) | https://gameguru.ru/publication/luchshie-brauzernye-igry-2026-goda-da-oni-vse-eshe-zhivy/ | External list |
| mmoguider | https://mmoguider.ru/articles/top-15-luchshih-brauzernyh-igr-dlya-pk | External list |
| hi-tech.mail.ru | https://hi-tech.mail.ru/compilations/100467-brauzernye-igry/ | External list |
| FRVR | https://frvr.com/blog/guides/best-browser-games/ | External list |
| hackster | https://hackster.ru/development/articles/top-yandex-games-with-high-ratings/ | Yandex related |
| game-analytics.ru | https://game-analytics.ru/ | Analytics portal |
| mmobomb | https://www.mmobomb.com/ | External catalog |
| gmodz | https://gmodz.ru/top-10-igr-v-kotorye-mozhno-poigrat-na-platformah-msn-games-v-2026-gody/ | External list |
| exputer | https://exputer.ru/top-10-igr-dlya-igry-na-igrovoj-platforme-msn-v-2026-godu/ | External list |
| gfinity | https://www.gfinityesports.com/article/top-10-games-to-play-on-msn-games-platforms-2026 | External list |

### data/top_raw.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_raw.md)

# Сырой список top (yg4)
Шаблон таблицы (Top 50 / витрина):

| # | Game | URL | Source | Rating | Tags | Notes (genre/tags/mechanic) |
|---:|---|---|---|---:|---|---|

### data/top_clusters.md
(Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_clusters.md)

# Кластера (yg4)
Ключевые идеи:
- после заполнения `top_raw.md` сгруппировать игры по механикам/петлям
- выделить типы: **endless** и **campaign**

| Cluster | Examples | Count | Notes |
|---|---|---:|---|

### data/top_shortlist_10.md
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
