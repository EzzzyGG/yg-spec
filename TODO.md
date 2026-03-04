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
