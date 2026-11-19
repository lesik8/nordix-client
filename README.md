# Nordix

Nordix — кроссплатформенный VPN-клиент (Windows, macOS, Linux, Android, iOS) для частной инфраструктуры VLESS + REALITY.

Этот репозиторий является форком [hiddify/hiddify-app](https://github.com/hiddify/hiddify-app) и распространяется по лицензии [Hiddify Extended GNU GPL v3](LICENSE.md), включая все дополнительные условия оригинального проекта.

## Attribution

- Оригинальный проект: **Hiddify** — https://github.com/hiddify/hiddify-app
- Оригинальная лицензия: [LICENSE.md](LICENSE.md)
- Ядро: [sing-box](https://github.com/SagerNet/sing-box), [Xray-core](https://github.com/XTLS/Xray-core)

## Изменения относительно upstream

1. **Ребрендинг**: приложение переименовано в Nordix (название окна, имя бинарника, метаданные Windows/macOS, ссылки в `lib/core/model/constants.dart`), новые иконки приложения и трея, новый логотип (`assets/images/logo.svg`).
2. **Встроенная подписка**: при первом запуске (когда нет ни одного профиля) приложение автоматически добавляет подписку по умолчанию — `Constants.defaultSubscriptionUrl` (`lib/features/profile/data/profile_repository.dart`, метод `init`). Ошибка загрузки подписки логируется и не мешает работе.
3. Ссылки поддержки заменены на контакты проекта Nordix.

Все релизы собираются через GitHub Actions (см. `.github/workflows`), как того требует лицензия.

## Сборка

Сборка выполняется в GitHub Actions: вкладка **Actions → CI → Run workflow**. Артефакты для Windows и macOS публикуются в разделе Releases (draft).
