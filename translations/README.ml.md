![ഫിലമെൻ്റ് അഡ്മിൻ പാനലുള്ള ലാറവൽ ബ്ലോഗ്](../docs/social-preview-en.png)

_Read this in [other languages](./Translations.md)_

>This file is automatically translated. If you notice an error, please correct it yourself (by making a PR) or write about it in the [issues](https://github.com/gomzyakov/laravel-blog/issues).

# ഫിലമെൻ്റ് അഡ്‌മിൻ പാനലുള്ള ലാറവെൽ ബ്ലോഗ്

ഇതാണ് [Laravel](https://laravel.com) [Filament](https://filamentphp.com) അഡ്മിൻ പാനലുള്ള ബ്ലോഗ് സ്റ്റാർട്ടർ കിറ്റ് പ്രോജക്റ്റ്.

ഒരു ലളിതമായ ആപ്ലിക്കേഷൻ ഉപയോഗിച്ച് നല്ല [Laravel](https://laravel.com) വികസന രീതികൾ പ്രദർശിപ്പിക്കുക എന്നതാണ് ഈ ശേഖരണത്തിൻ്റെ ലക്ഷ്യം.

## ഫീച്ചറുകൾ

- 📚 പോസ്റ്റുകൾ സൃഷ്‌ടിക്കുകയും എഡിറ്റുചെയ്യുകയും ചെയ്യുന്നു
- 🥑 വിഭാഗങ്ങൾ
- :തീ: ജനപ്രിയ പോസ്റ്റുകൾ
- 🎉 [Filament](https://filamentphp.com)-ൽ നിർമ്മിച്ച അഡ്‌മിൻ പാനൽ

## സവിശേഷതകൾ അഭ്യർത്ഥിക്കുന്നു

ഒരു ഫീച്ചർ അഭ്യർത്ഥിക്കുന്നതിന് (അല്ലെങ്കിൽ നിങ്ങൾ ഒരു ബഗ് കണ്ടെത്തിയാൽ) [പുതിയ ലക്കം](https://github.com/gomzyakov/laravel-blog/issues/new) തുറക്കുക.

## ബ്ലോഗ് പ്രാദേശികമായി എങ്ങനെ പ്രവർത്തിപ്പിക്കാം?

പ്രോജക്റ്റ് ക്ലോൺ ചെയ്യുക:

``` ബാഷ്
git clone git@github.com:gomzyakov/laravel-blog.git
```

നിങ്ങൾ ഇതിനകം ഡോക്കർ ഇൻസ്റ്റാൾ ചെയ്തിട്ടുണ്ടെന്ന് ഞാൻ വിശ്വസിക്കുന്നു. ഇല്ലെങ്കിൽ, [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows) എന്നതിൽ ഇത് ചെയ്യുക -install/) അല്ലെങ്കിൽ [Linux](https://docs.docker.com/desktop/install/linux-install/).

ഇനിപ്പറയുന്ന കമാൻഡ് ഉപയോഗിച്ച് 'laravel-blog' ഇമേജ് നിർമ്മിക്കുക:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് ബിൽഡ് --നോ-കാഷെ
```

> ഈ കമാൻഡ് പൂർത്തിയാക്കാൻ കുറച്ച് മിനിറ്റുകൾ എടുത്തേക്കാം.

നിർമ്മാണം പൂർത്തിയാകുമ്പോൾ, നിങ്ങൾക്ക് പശ്ചാത്തല മോഡിൽ പരിസ്ഥിതി പ്രവർത്തിപ്പിക്കാൻ കഴിയും:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് അപ്പ് -ഡി
```

ആപ്ലിക്കേഷൻ ഡിപൻഡൻസികൾ ഇൻസ്‌റ്റാൾ ചെയ്യുന്നതിന് ഞങ്ങൾ ഇപ്പോൾ `കമ്പോസർ ഇൻസ്റ്റാൾ' പ്രവർത്തിപ്പിക്കും:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് എക്‌സിക് ആപ്പ് കമ്പോസർ ഇൻസ്റ്റാൾ ചെയ്യുക
```

പരിസ്ഥിതി ക്രമീകരണങ്ങൾ പകർത്തുക:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് എക്‌സിക് ആപ്പ് cp .env.local .env
```

`ആർട്ടിസാൻ` Laravel കമാൻഡ്-ലൈൻ ടൂൾ ഉപയോഗിച്ച് എൻക്രിപ്ഷൻ കീ സജ്ജമാക്കുക:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് എക്‌സിക് ആപ്പ് ./ആർട്ടിസാൻ കീ:ജനറേറ്റ് --ആൻസി
```

DB & വിത്ത് വ്യാജ ഡാറ്റ മൈഗ്രേറ്റ് ചെയ്യുക:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് എക്‌സിക് ആപ്പ് ./ആർട്ടിസാൻ മൈഗ്രേറ്റ്:ഫ്രഷ് --സീഡ്
```

ഒപ്പം ഫിലമെൻ്റ് അഡ്മിൻ ഉപയോക്താവിനെ ചേർക്കുക:

``` ബാഷ്
ഡോക്കർ കമ്പോസ് എക്‌സിക് ആപ്പ് ./ആർട്ടിസാൻ മേക്ക്:ഫിലമെൻ്റ്-യൂസർ
```

നിങ്ങളുടെ പ്രിയപ്പെട്ട ബ്രൗസറിൽ http://127.0.0.1:8000 തുറക്കുക. Laravel ബ്ലോഗ് ഉപയോഗിക്കുന്നതിൽ സന്തോഷമുണ്ട്!

## കണ്ടെയ്നറിനുള്ളിൽ എങ്ങനെ കയറാം?

ഡോക്കർ കണ്ടെയ്‌നറിലേക്കുള്ള ആക്‌സസ്:

``` ബാഷ്
docker exec -ti laravel-blog-app bash
```

## ലൈസൻസ്

ഇത് [MIT ലൈസൻസ്](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE) പ്രകാരം ലൈസൻസുള്ള ഓപ്പൺ സോഴ്‌സ് സോഫ്‌റ്റ്‌വെയറാണ്.


[![GitHub റിലീസ്](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![license](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ laravel-blog)
