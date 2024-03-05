![Блог Laravel с панелью администратора Filament](../docs/social-preview-en.png)

# Блог Laravel с админ-панелью Filament

Это проект стартового набора блога [Laravel](https://laravel.com) с панелью администратора [Filament](https://filamentphp.com).

Цель этого репозитория — продемонстрировать хорошие практики разработки [Laravel](https://laravel.com) с помощью простого приложения.

## Функции

- 📚 Создание и редактирование публикаций
- 🥑 Категории
- :fire: Популярные посты
- :hatched_chick: Панель администратора, построенная на [Filament](https://filamentphp.com)

## Запрос функций

Откройте [новую проблему](https://github.com/gomzykov/laravel-blog/issues/new), чтобы запросить функцию (или если вы обнаружили ошибку).

## Как запустить блог локально?

Клонируйте проект:

``` баш
git clone git@github.com:gomzykov/laravel-blog.git
```

Я полагаю, что у вас уже установлен Docker. Если нет, просто сделайте это на [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows -install/) или [Linux](https://docs.docker.com/desktop/install/linux-install/).

Создайте образ `laravel-blog` с помощью следующей команды:

``` баш
Docker Compose build --no-cache
```

>Выполнение этой команды может занять несколько минут.

Когда сборка завершена, вы можете запустить среду в фоновом режиме с помощью:

``` баш
докер составить -d
```

Теперь мы запустим `composer install`, чтобы установить зависимости приложения:

``` баш
установка Docker Compose Exec App Composer
```

Скопируйте настройки среды:

``` баш
Docker Compose Exec App cp .env.local .env
```

Установите ключ шифрования с помощью инструмента командной строки `artisan` Laravel:

``` баш
docker compose exec app ./artisan key:generate --ansi
```

Миграция БД и заполнение поддельных данных:

``` баш
docker Compose Exec App ./artisan Migrate: Fresh --seed
```

И добавьте пользователя-администратора Filament:

``` баш
приложение docker compose exec ./artisan make:filament-user
```

И откройте http://127.0.0.1:8000 в своем любимом браузере. Приятного использования блога Laravel!

## Как попасть внутрь контейнера?

Доступ к Docker-контейнеру:

``` баш
docker exec -ti laravel-blog-app bash
```

## Лицензия

Это программное обеспечение с открытым исходным кодом, лицензированное по [Лицензии MIT](https://github.com/gomzykov/php-code-style/blob/main/LICENSE).


[![Выпуск GitHub](https://img.shields.io/github/release/gomzykov/laravel-blog.svg)](https://github.com/gomzykov/laravel-blog/releases/latest)
[![лицензия](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzykov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzykov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzykov/ laravel-блог)