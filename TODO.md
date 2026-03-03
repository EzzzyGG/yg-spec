# TODO (без "attempts")

> Работаем строго по этому списку: фиксируем, что уже сделано, и что осталось сделать.

## ✅ Done

- Собраны и сведены материалы из `yg research` репозиториев в единый файл:
  - `docs/yg-research-merged.md`
  - Источники: 
    - https://github.com/EzzzyGG/yg4-top-research
    - https://github.com/EzzzyGG/yg2-top-research

- Проверено, что в `yg-spec` нет упоминаний `attempts/ATTEMPT/Attempt` (по code search).

## 🟦 To do

### A) Спека / структура документации
- [x] Разнести `yg spec` в отдельный(е) документ(ы): что именно делаем в проекте (цель, платформа, ограничения).
- [ ] Зафиксировать версии/стек: Unity 2022.3 LTS, WebGL, YG SDK.

### B) Research → требования
- [ ] Заполнить `top_raw` таблицу (минимум Top 50 по Yandex Games RU/EN + внешние списки).
- [ ] Сделать кластеризацию по core loop / жанру / механикам.
- [ ] Сформировать shortlist: 5 endless + 5 campaign.

### C) Требования к монетизации/прогрессии (из shortlist)
- [ ] Для каждого из 10 направлений описать:
  - core loop
  - meta progression
  - rewarded video
  - interstitial
  - IAP (RUB; small/medium/large + remove ads + starter pack)
  - leaderboard (если нужен)

### D) Интеграции Yandex Games SDK
- [ ] Описать интеграции SDK как список модулей: ads, IAP, cloud saves, leaderboards, env/auth/lang.
- [ ] Для каждого модуля: события/ошибки/таймауты/UX.

### E) План реализации (по шагам)
- [ ] Сформировать план работ по репозиторию: порядок задач, критерии готовности, чек-лист тестов.
