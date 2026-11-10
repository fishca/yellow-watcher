# yellow-watcher

Fork of [sdf1979/yellow-watcher](https://github.com/sdf1979/yellow-watcher).

Утилита для Windows: следит за технологическим журналом 1С, парсит события,
агрегирует их и отправляет JSON в HTTP-сервис расширения 1С
(`IntegrationService/Load`).

## Состав

- `yellow-watcher/` — исходники C++ (парсер техжурнала, watcher каталога, агрегаторы, отправитель)
- `1c-extention/YellowWatcher.cfe` — расширение 1С (скомпилированное, без исходников)
- `x64/Release/` — сборка под Windows

Зависимости: Boost (header-only, `boost::json`), OpenSSL, libcurl. В репозитории
не лежат — тянутся извне.

## Лицензия

Apache License 2.0, см. [LICENSE](LICENSE). Сведения об авторе оригинала — в [NOTICE](NOTICE).
