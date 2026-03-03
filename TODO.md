# TODO (yg-spec)

Этот список — единственный источник правды по работе: без “attempts”, без параллельных вариантов.

## ✅ Done

- Найдены и определены репозитории:
  - Спека: https://github.com/EzzzyGG/yg-spec
  - Research: https://github.com/EzzzyGG/yg4-top-research , https://github.com/EzzzyGG/yg2-top-research
- Собран единый файл с research-материалами в `yg-spec`:
  - `yg-research-merged.md`

## 🟦 To do

### 1) Спека (yg spec)
- [ ] Разбить текущий `README.md` на структуру спек (минимум):
  - [ ] `SPEC.md` (или `spec/overview.md`): цель, термины, ограничения платформы
  - [ ] `spec/ads.md`: rewarded/interstitial требования, частоты, UX
  - [ ] `spec/iap.md`: SKU, цены, повторяемые/одноразовые покупки
  - [ ] `spec/saves.md`: прогресс/облачные сейвы
  - [ ] `spec/leaderboards.md`: лидерборды
  - [ ] `spec/env-auth-lang.md`: окружение, авторизация, язык
- [ ] Убрать из текста любые следы “attempts”/итераций (если где-то появятся) — работаем строго по этому TODO.

### 2) Research → решения
- [ ] Заполнить `yg4-top-research/data/top_raw.md` (Top 50 + витрины Yandex RU/EN).
- [ ] Заполнить `yg4-top-research/data/top_clusters.md` (кластеры + частоты).
- [ ] Заполнить `yg4-top-research/data/top_shortlist_10.md` (итоговые 10 направлений).
- [ ] Зафиксировать выбранные 10 направлений уже в `yg-spec` (отдельный раздел/файл), чтобы стало частью спеки.

### 3) Контрольный список интеграции SDK
- [ ] Составить чек-лист интеграции Yandex Games SDK для Unity WebGL:
  - [ ] init/install
  - [ ] ads
  - [ ] iap
  - [ ] saves
  - [ ] leaderboards
  - [ ] events/analytics (если нужно)

