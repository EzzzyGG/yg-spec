# YG Research — merged snapshot

Собрано из репозиториев:
- https://github.com/EzzzyGG/yg4-top-research
- https://github.com/EzzzyGG/yg2-top-research

> Примечание: этот файл — консолидированная выжимка/снимок материалов research, чтобы вести работу по единому TODO-листу в `yg-spec`.

---

## yg4-top-research

Источник: https://github.com/EzzzyGG/yg4-top-research

### README (кратко)
- Цель: собрать воспроизводимый “топ/популярность” (Yandex Games + внешние) и сделать план/спек для реализации (Unity WebGL + YG SDK).
- Артефакты в `data/`:
  - `data/top_sources.md` — источники/URL и время снятия
  - `data/top_raw.md` — сырой шаблон таблицы top
  - `data/top_clusters.md` — кластеризация/группировка (endless/campaign)
  - `data/top_shortlist_10.md` — shortlist из 10 направлений и мета-полей (монетизация/прогресс/лидерборды)

### data/top_sources.md
Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_sources.md

Содержимое (как есть):

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
| hakster | https://hakster.ru/development/articles/top-yandex-games-with-high-ratings/ | Yandex related |
| game-analytics.ru | https://game-analytics.ru/ | Analytics portal |
| mmobomb | https://www.mmobomb.com/ | External catalog |
| gmodz | https://gmodz.ru/top-10-igr-v-kotorye-mojno-poigrat-na-platformah-msn-games-v-2026-gody/ | External list |
| exputer | https://exputer.ru/top-10-igr-dlya-igry-na-igrovoj-platforme-msn-v-2026-godu/ | External list |
| gfinity | https://www.gfinityesports.com/article/top-10-games-to-play-on-msn-games-platforms-2026 | External list |

### data/top_raw.md
Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_raw.md

Заготовка таблицы:

| # | Game | URL | Source | Rating | Tags | Notes (genre/tags/mechanic) |
|--:|---|---|---|---:|---|---|

### data/top_clusters.md
Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_clusters.md

Ключевая идея:
- после заполнения `top_raw.md` сгруппировать игры по механикам/петлям
- выделить типы: **endless** и **campaign**

### data/top_shortlist_10.md
Источник: https://github.com/EzzzyGG/yg4-top-research/blob/main/data/top_shortlist_10.md

Смысл:
- собрать shortlist из 10 направлений (5 endless + 5 campaign)
- таблица “каркаса”: направление, тип, core loop, мета, монетизация (rewarded/interstitial/IAP), лидерборды

---

## yg2-top-research

Источник: https://github.com/EzzzyGG/yg2-top-research

### README
Источник: https://github.com/EzzzyGG/yg2-top-research/blob/main/README.md

Кратко:
- “Yandex Games: top lists snapshot + external comparisons + notes for replication (Unity 2022.3 LTS / YG SDK)”.

---

## Вывод (что переносим в работу по spec)

- Исходники и таблицы из `yg4-top-research/data/*` — база для составления короткого списка и требований к мета/монетизации.
- `yg2-top-research` — контекст и формулировка цели (снимок топов + сравнения + заметки).
