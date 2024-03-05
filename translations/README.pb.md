![ਫਿਲਾਮੈਂਟ ਐਡਮਿਨ ਪੈਨਲ ਵਾਲਾ ਲਾਰਵੇਲ ਬਲੌਗ](../docs/social-preview-en.png)

ਫਿਲਾਮੈਂਟ ਐਡਮਿਨ ਪੈਨਲ ਦੇ ਨਾਲ # ਲਾਰਵੇਲ ਬਲੌਗ

ਇਹ [Filament](https://filamentphp.com) ਐਡਮਿਨ ਪੈਨਲ ਵਾਲਾ [Laravel](https://laravel.com) ਬਲੌਗ ਸਟਾਰਟਰ ਕਿੱਟ ਪ੍ਰੋਜੈਕਟ ਹੈ।

ਇਸ ਰਿਪੋਜ਼ਟਰੀ ਦਾ ਟੀਚਾ ਇੱਕ ਸਧਾਰਨ ਐਪਲੀਕੇਸ਼ਨ ਨਾਲ ਚੰਗੇ [Laravel](https://laravel.com) ਵਿਕਾਸ ਅਭਿਆਸਾਂ ਦਾ ਪ੍ਰਦਰਸ਼ਨ ਕਰਨਾ ਹੈ।

## ਵਿਸ਼ੇਸ਼ਤਾਵਾਂ

- 📚 ਪੋਸਟਾਂ ਬਣਾਉਣਾ ਅਤੇ ਸੰਪਾਦਿਤ ਕਰਨਾ
- 🥑 ਸ਼੍ਰੇਣੀਆਂ
- :ਫਾਇਰ: ਪ੍ਰਸਿੱਧ ਪੋਸਟਾਂ
- :hatched_chick: [ਫਿਲਾਮੈਂਟ](https://filamentphp.com) 'ਤੇ ਬਣਿਆ ਐਡਮਿਨ ਪੈਨਲ

## ਵਿਸ਼ੇਸ਼ਤਾਵਾਂ ਦੀ ਬੇਨਤੀ ਕਰਨਾ

ਕਿਸੇ ਵਿਸ਼ੇਸ਼ਤਾ ਦੀ ਬੇਨਤੀ ਕਰਨ ਲਈ ਇੱਕ [ਨਵਾਂ ਮੁੱਦਾ](https://github.com/gomzyakov/laravel-blog/issues/new) ਖੋਲ੍ਹੋ (ਜਾਂ ਜੇਕਰ ਤੁਹਾਨੂੰ ਕੋਈ ਬੱਗ ਮਿਲਦਾ ਹੈ)।

## ਬਲੌਗ ਨੂੰ ਸਥਾਨਕ ਤੌਰ 'ਤੇ ਕਿਵੇਂ ਚਲਾਉਣਾ ਹੈ?

ਪ੍ਰੋਜੈਕਟ ਨੂੰ ਕਲੋਨ ਕਰੋ:

``ਬਾਸ਼
git clone git@github.com:gomzyakov/laravel-blog.git
``

ਮੇਰਾ ਮੰਨਣਾ ਹੈ ਕਿ ਤੁਹਾਡੇ ਕੋਲ ਪਹਿਲਾਂ ਹੀ ਡੌਕਰ ਸਥਾਪਤ ਹੈ. ਜੇ ਨਹੀਂ, ਤਾਂ ਇਸਨੂੰ [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows) 'ਤੇ ਕਰੋ -ਇੰਸਟਾਲ/) ਜਾਂ [ਲੀਨਕਸ](https://docs.docker.com/desktop/install/linux-install/)।

ਹੇਠ ਦਿੱਤੀ ਕਮਾਂਡ ਨਾਲ 'laravel-blog' ਚਿੱਤਰ ਬਣਾਓ:

``ਬਾਸ਼
docker ਕੰਪੋਜ਼ ਬਿਲਡ --no-cache
``

> ਇਸ ਕਮਾਂਡ ਨੂੰ ਪੂਰਾ ਹੋਣ ਵਿੱਚ ਕੁਝ ਮਿੰਟ ਲੱਗ ਸਕਦੇ ਹਨ।

ਜਦੋਂ ਬਿਲਡ ਪੂਰਾ ਹੋ ਜਾਂਦਾ ਹੈ, ਤੁਸੀਂ ਵਾਤਾਵਰਣ ਨੂੰ ਬੈਕਗ੍ਰਾਉਂਡ ਮੋਡ ਵਿੱਚ ਇਸ ਨਾਲ ਚਲਾ ਸਕਦੇ ਹੋ:

``ਬਾਸ਼
ਡੌਕਰ ਕੰਪੋਜ਼ ਅੱਪ -ਡੀ
``

ਅਸੀਂ ਹੁਣ ਐਪਲੀਕੇਸ਼ਨ ਨਿਰਭਰਤਾ ਨੂੰ ਸਥਾਪਤ ਕਰਨ ਲਈ 'ਕੰਪੋਜ਼ਰ ਇੰਸਟੌਲ' ਚਲਾਵਾਂਗੇ:

``ਬਾਸ਼
docker compose exec ਐਪ ਕੰਪੋਜ਼ਰ ਇੰਸਟੌਲ
``

ਵਾਤਾਵਰਣ ਸੈਟਿੰਗਾਂ ਦੀ ਨਕਲ ਕਰੋ:

``ਬਾਸ਼
docker compose exec app cp .env.local .env
``

'ਕਾਰੀਗਰ' Laravel ਕਮਾਂਡ-ਲਾਈਨ ਟੂਲ ਨਾਲ ਏਨਕ੍ਰਿਪਸ਼ਨ ਕੁੰਜੀ ਸੈਟ ਕਰੋ:

``ਬਾਸ਼
docker compose exec app./artisan key:generate --ansi
``

DB ਅਤੇ ਬੀਜ ਜਾਅਲੀ ਡੇਟਾ ਨੂੰ ਮਾਈਗਰੇਟ ਕਰੋ:

``ਬਾਸ਼
ਡੌਕਰ ਕੰਪੋਜ਼ ਐਗਜ਼ੀਕਿਊਸ਼ਨ ਐਪ ./ਆਰਟਿਸਨ ਮਾਈਗਰੇਟ: ਤਾਜ਼ਾ --ਸੀਡ
``

ਅਤੇ ਫਿਲਾਮੈਂਟ ਐਡਮਿਨ ਉਪਭੋਗਤਾ ਸ਼ਾਮਲ ਕਰੋ:

``ਬਾਸ਼
ਡੌਕਰ ਕੰਪੋਜ਼ ਐਗਜ਼ੀਕਿਊਸ਼ਨ ਐਪ ./ਆਰਟੀਸਨ ਮੇਕ: ਫਿਲਾਮੈਂਟ-ਯੂਜ਼ਰ
``

ਅਤੇ ਆਪਣੇ ਮਨਪਸੰਦ ਬ੍ਰਾਊਜ਼ਰ ਵਿੱਚ http://127.0.0.1:8000 ਖੋਲ੍ਹੋ। Laravel ਬਲੌਗ ਦੀ ਵਰਤੋਂ ਕਰਕੇ ਖੁਸ਼ੀ!

## ਡੱਬੇ ਦੇ ਅੰਦਰ ਕਿਵੇਂ ਜਾਣਾ ਹੈ?

ਡੌਕਰ ਕੰਟੇਨਰ ਤੱਕ ਪਹੁੰਚ:

``ਬਾਸ਼
docker exec -ti laravel-blog-app bash
``

## ਲਾਇਸੰਸ

ਇਹ [MIT ਲਾਇਸੈਂਸ](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE) ਦੇ ਅਧੀਨ ਲਾਇਸੰਸਸ਼ੁਦਾ ਓਪਨ-ਸੋਰਸਡ ਸੌਫਟਵੇਅਰ ਹੈ।


[![GitHub ਰਿਲੀਜ਼](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![ਲਾਈਸੈਂਸ](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ laravel-blog)