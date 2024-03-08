![ಫಿಲಮೆಂಟ್ ನಿರ್ವಾಹಕ ಫಲಕದೊಂದಿಗೆ ಲಾರಾವೆಲ್ ಬ್ಲಾಗ್](../docs/social-preview-en.png)

_Read this in [other languages](./Translations.md)_

>This file is automatically translated. If you notice an error, please correct it yourself (by making a PR) or write about it in the [issues](https://github.com/gomzyakov/laravel-blog/issues).

# ಫಿಲಮೆಂಟ್ ನಿರ್ವಾಹಕ ಫಲಕದೊಂದಿಗೆ ಲಾರಾವೆಲ್ ಬ್ಲಾಗ್

ಇದು [Laravel](https://laravel.com) [Filament](https://filamentphp.com) ನಿರ್ವಾಹಕ ಫಲಕದೊಂದಿಗೆ ಬ್ಲಾಗ್ ಸ್ಟಾರ್ಟರ್ ಕಿಟ್ ಯೋಜನೆಯಾಗಿದೆ.

ಸರಳವಾದ ಅಪ್ಲಿಕೇಶನ್‌ನೊಂದಿಗೆ ಉತ್ತಮ [Laravel](https://laravel.com) ಅಭಿವೃದ್ಧಿ ಅಭ್ಯಾಸಗಳನ್ನು ಪ್ರದರ್ಶಿಸುವುದು ಈ ರೆಪೊಸಿಟರಿಯ ಗುರಿಯಾಗಿದೆ.

## ವೈಶಿಷ್ಟ್ಯಗಳು

- 📚 ಪೋಸ್ಟ್‌ಗಳನ್ನು ರಚಿಸುವುದು ಮತ್ತು ಸಂಪಾದಿಸುವುದು
- 🥑 ವರ್ಗಗಳು
- : ಬೆಂಕಿ: ಜನಪ್ರಿಯ ಪೋಸ್ಟ್‌ಗಳು
- 🎉 ನಿರ್ವಾಹಕ ಫಲಕವನ್ನು [ಫಿಲಮೆಂಟ್] (https://filamentphp.com) ನಲ್ಲಿ ನಿರ್ಮಿಸಲಾಗಿದೆ

## ವೈಶಿಷ್ಟ್ಯಗಳನ್ನು ವಿನಂತಿಸಲಾಗುತ್ತಿದೆ

ವೈಶಿಷ್ಟ್ಯವನ್ನು ವಿನಂತಿಸಲು [ಹೊಸ ಸಂಚಿಕೆ](https://github.com/gomzyakov/laravel-blog/issues/new) ತೆರೆಯಿರಿ (ಅಥವಾ ನೀವು ದೋಷವನ್ನು ಕಂಡುಕೊಂಡರೆ).

## ಬ್ಲಾಗ್ ಅನ್ನು ಸ್ಥಳೀಯವಾಗಿ ನಡೆಸುವುದು ಹೇಗೆ?

ಯೋಜನೆಯನ್ನು ಕ್ಲೋನ್ ಮಾಡಿ:

```ಬಾಷ್
git ಕ್ಲೋನ್ git@github.com:gomzyakov/laravel-blog.git
```

ನೀವು ಈಗಾಗಲೇ ಡಾಕರ್ ಅನ್ನು ಸ್ಥಾಪಿಸಿರುವಿರಿ ಎಂದು ನಾನು ನಂಬುತ್ತೇನೆ. ಇಲ್ಲದಿದ್ದರೆ, ಅದನ್ನು [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows) ನಲ್ಲಿ ಮಾಡಿ -install/) ಅಥವಾ [Linux](https://docs.docker.com/desktop/install/linux-install/).

ಕೆಳಗಿನ ಆಜ್ಞೆಯೊಂದಿಗೆ `laravel-blog` ಚಿತ್ರವನ್ನು ನಿರ್ಮಿಸಿ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಬಿಲ್ಡ್ --ನೋ-ಕ್ಯಾಶ್
```

> ಈ ಆಜ್ಞೆಯು ಪೂರ್ಣಗೊಳ್ಳಲು ಕೆಲವು ನಿಮಿಷಗಳನ್ನು ತೆಗೆದುಕೊಳ್ಳಬಹುದು.

ನಿರ್ಮಾಣ ಪೂರ್ಣಗೊಂಡಾಗ, ನೀವು ಇದರೊಂದಿಗೆ ಹಿನ್ನೆಲೆ ಮೋಡ್‌ನಲ್ಲಿ ಪರಿಸರವನ್ನು ಚಲಾಯಿಸಬಹುದು:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಅಪ್ -ಡಿ
```

ಅಪ್ಲಿಕೇಶನ್ ಅವಲಂಬನೆಗಳನ್ನು ಸ್ಥಾಪಿಸಲು ನಾವು ಈಗ "ಸಂಯೋಜಕ ಸ್ಥಾಪನೆ" ಅನ್ನು ರನ್ ಮಾಡುತ್ತೇವೆ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಎಕ್ಸಿಕ್ ಆಪ್ ಕಂಪೋಸರ್ ಇನ್‌ಸ್ಟಾಲ್
```

ಪರಿಸರ ಸೆಟ್ಟಿಂಗ್‌ಗಳನ್ನು ನಕಲಿಸಿ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಎಕ್ಸಿಕ್ ಅಪ್ಲಿಕೇಶನ್ cp .env.local .env
```

`ಕುಶಲಕರ್ಮಿ` ಲಾರಾವೆಲ್ ಕಮಾಂಡ್-ಲೈನ್ ಉಪಕರಣದೊಂದಿಗೆ ಎನ್‌ಕ್ರಿಪ್ಶನ್ ಕೀಯನ್ನು ಹೊಂದಿಸಿ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಎಕ್ಸಿಕ್ ಅಪ್ಲಿಕೇಶನ್ ./ಕುಶಲಕರ್ಮಿ ಕೀ:ಜನರೇಟ್ --ಆನ್ಸಿ
```

DB ಮತ್ತು ಬೀಜ ನಕಲಿ ಡೇಟಾವನ್ನು ಸ್ಥಳಾಂತರಿಸಿ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಎಕ್ಸಿಕ್ ಅಪ್ಲಿಕೇಶನ್ ./ಕುಶಲಕರ್ಮಿ ವಲಸೆ: ತಾಜಾ --ಬೀಜ
```

ಮತ್ತು ಫಿಲಮೆಂಟ್ ನಿರ್ವಾಹಕ ಬಳಕೆದಾರರನ್ನು ಸೇರಿಸಿ:

```ಬಾಷ್
ಡಾಕರ್ ಕಂಪೋಸ್ ಎಕ್ಸಿಕ್ ಅಪ್ಲಿಕೇಶನ್ ./ಆರ್ಟಿಸನ್ ಮೇಕ್: ಫಿಲಮೆಂಟ್-ಯೂಸರ್
```

ಮತ್ತು ನಿಮ್ಮ ಮೆಚ್ಚಿನ ಬ್ರೌಸರ್‌ನಲ್ಲಿ http://127.0.0.1:8000 ತೆರೆಯಿರಿ. ಲಾರಾವೆಲ್ ಬ್ಲಾಗ್ ಅನ್ನು ಬಳಸಲು ಸಂತೋಷವಾಗಿದೆ!

## ಕಂಟೇನರ್ ಒಳಗೆ ಹೋಗುವುದು ಹೇಗೆ?

ಡಾಕರ್ ಕಂಟೇನರ್‌ಗೆ ಪ್ರವೇಶ:

```ಬಾಷ್
ಡಾಕರ್ ಎಕ್ಸಿಕ್ -ಟಿ ಲಾರಾವೆಲ್-ಬ್ಲಾಗ್-ಅಪ್ಲಿಕೇಶನ್ ಬ್ಯಾಷ್
```

## ಪರವಾನಗಿ

ಇದು [MIT ಪರವಾನಗಿ](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE) ಅಡಿಯಲ್ಲಿ ಪರವಾನಗಿ ಪಡೆದಿರುವ ಓಪನ್ ಸೋರ್ಸ್ ಸಾಫ್ಟ್‌ವೇರ್ ಆಗಿದೆ.


[![GitHub ಬಿಡುಗಡೆ](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![ಪರವಾನಗಿ](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ ಲಾರಾವೆಲ್-ಬ್ಲಾಗ್)
