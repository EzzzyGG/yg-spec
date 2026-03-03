# yg4 — мастер-спека (Яндекс Игры / Unity 2022.3 LTS)

Этот репозиторий фиксирует исходный запрос/требования к пакету из 10 браузерных игр под Яндекс Игры.

## 0) Цель

- Взять **топ/популярные игры** на Яндекс Играх и по мотивам механик сделать **10 оригинальных игр**.
- Все игры: **Unity 2022.3 LTS**, WebGL, браузер, **мобилка + тач**.
- Критерий готовности: **играбельно**, контента/прогрессии на **45–60 минут**.
- Ты (заказчик) загружаешь на платформу; я готовлю проект, ассеты, интеграции, инструкции.

## 1) Репозитории и нумерация

- Каждая игра — **отдельный приватный репозиторий**.
- Нейминг игр: `yg<ATTEMPT>-unity-01-<slug>` … `yg<ATTEMPT>-unity-10-<slug>`.
- Номер попытки определяется по существующим `yg1`, `yg2`, … в GitHub.
- Топ-исследование (если нужно отдельным репо): `yg<ATTEMPT>-top-research`.

## 2) Игровой план (10 игр)

- **5 игр**: бесконечная прогрессия (endless / score / upgrades / meta).
- **5 игр**: кампания с уровнями.
- Жанр/стилистика — на усмотрение исполнителя, но по мотивам популярных механик.

## 3) Обязательные UX/экраны

В каждой игре (если уместно):
- главное меню
- пауза
- настройки (звук и т.п.)
- туториал/обучение
- экран `Game Over`
- баланс/экономика

## 4) Монетизация (строго через SDK Яндекс Игр)

**Баннеры: да (разрешено).**

### 4.1 Реклама

- **Rewarded Video** — мягкая монетизация, всегда по желанию игрока.
- **Видео/Interstitial по смерти** (принудительное) — разрешено.
- Покупка **"убрать рекламу"** отключает только **принудительные** показы; rewarded остаётся.

### 4.2 Внутриигровые покупки (IAP)

- Валюта: **RUB**.
- Пакеты на игру (примерная структура):
  - `Small` / `Medium` / `Large` — **повторяемые**
  - `Remove forced ads` — **одноразовая**
  - `Starter pack` — **одноразовая**
- Восстановление покупок при повторном заходе — обязательно.

## 5) Прогресс, сейвы и облако

- **Сейв в каждой игре**.
- Сейвы: **через облако Яндекс Игр**, где возможно.
- Авторизация игрока: **молчаливая**.
  - Если игрок не авторизован, работаем в гостевом режиме.
  - При появлении авторизации делаем **мягкий merge** данных.

## 6) Лидерборды

- Только там, где есть измеримый результат: **score / distance / time**.
- Без "друзей вокруг меня".
- Достаточно: **Top + мой результат**.

## 7) Ассеты и лицензии

- Ассеты должны иметь **разрешённую коммерческую лицензию** (или быть с явной лицензией/условиями использования).
- Если ассеты без лицензии — предпочтительно не использовать.
- Допустимо генерировать свои изображения через бесплатные нейросети **без твоих API-ключей**.
- В каждом репо нужен список ассетов и лицензий.

## 8) Публикация

Для каждой игры подготовить:
- иконки
- скриншоты
- описания
- теги
- RU + EN тексты

## 9) SDK Яндекс Игр — официальная интеграция

Требуется официальная интеграция по докам:
- инициализация SDK
- реклама (rewarded/video)
- IAP
- облачные сохранения
- лидерборды
- авторизация

### Ссылки на документацию (Unity)

- Install / init: https://yandex.ru/dev/games/doc/ru/sdk/unity/install
- Ads: https://yandex.ru/dev/games/doc/ru/sdk/unity/advertisement
- IAP: https://yandex.ru/dev/games/doc/ru/sdk/unity/inaps
- Cloud saves: https://yandex.ru/dev/games/doc/ru/sdk/unity/progress-saving
- Leaderboards: https://yandex.ru/dev/games/doc/ru/sdk/unity/leaderboards
- Env/Auth/Lang: https://yandex.ru/dev/games/doc/ru/sdk/unity/env-auth-lang

## 10) Ограничения и процесс

- Нет SerpAPI.
- Работать **пошагово**, не делать всё сразу.
- Перед каждым большим этапом — просить в чате слово **"ок"**.
- Целевой фреймрейт: **30 FPS**.
- Репозитории пушим в: `EzzzyGG/*`.

---

## Приложение A — источники топов/внешней аналитики (из запроса)

- Яндекс Игры: https://yandex.ru/games
- Poki: https://poki.com/
- CrazyGames: https://www.crazygames.com/
- MSN Games: https://www.msn.com/ru-ru/play

- MMO13 топ: https://mmo13.ru/games/top/platform-71/year-2026
- Gameguru: https://gameguru.ru/publication/luchshie-brauzernye-igry-2026-goda-da-oni-vse-eshe-zhivy/
- mmoguider: https://mmoguider.ru/articles/top-15-luchshih-brauzernyh-igr-dlya-pk
- hi-tech mail: https://hi-tech.mail.ru/compilations/100467-brauzernye-igry/
- FRVR: https://frvr.com/blog/guides/best-browser-games/

- game-analytics.ru: https://game-analytics.ru/
- hakster: https://hakster.ru/development/articles/top-yandex-games-with-high-ratings/
- mmobomb: https://www.mmobomb.com/
- gmodz: https://gmodz.ru/top-10-igr-v-kotorye-mojno-poigrat-na-platformah-msn-games-v-2026-gody/
- exputer: https://exputer.ru/top-10-igr-dlya-igry-na-igrovoj-platforme-msn-v-2026-godu/
- gfinity: https://www.gfinityesports.com/article/top-10-games-to-play-on-msn-games-platforms-2026
