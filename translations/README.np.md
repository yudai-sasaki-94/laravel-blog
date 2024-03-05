![फिलामेन्ट एडमिन प्यानलको साथ लारावेल ब्लग](../docs/social-preview-en.png)

फिलामेन्ट एडमिन प्यानलको साथ # Laravel ब्लग

यो [Laravel](https://laravel.com) [Filament](https://filamentphp.com) एडमिन प्यानल भएको ब्लग स्टार्टर किट परियोजना हो।

यस भण्डारको लक्ष्य एक साधारण अनुप्रयोगको साथ राम्रो [Laravel](https://laravel.com) विकास अभ्यासहरू प्रदर्शन गर्नु हो।

## विशेषताहरु

- 📚 पोस्टहरू सिर्जना र सम्पादन गर्दै
- 🥑 कोटीहरू
- :fire: लोकप्रिय पोस्टहरू
- :hatched_chick: एडमिन प्यानल [फिलामेन्ट](https://filamentphp.com) मा निर्मित

## सुविधाहरू अनुरोध गर्दै

कुनै सुविधाको अनुरोध गर्न (वा तपाईंले बग फेला पार्नुभयो भने) [नयाँ मुद्दा](https://github.com/gomzyakov/laravel-blog/issues/new) खोल्नुहोस्।

## स्थानीय रूपमा ब्लग कसरी चलाउने?

परियोजना क्लोन गर्नुहोस्:

``बाश
git clone git@github.com:gomzyakov/laravel-blog.git
```

मलाई विश्वास छ कि तपाईंले पहिले नै डकर स्थापना गर्नुभएको छ। यदि होइन भने, [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows) मा मात्र गर्नुहोस्। -install/) वा [Linux](https://docs.docker.com/desktop/install/linux-install/)।

निम्न आदेशको साथ `laravel-blog` छवि बनाउनुहोस्:

``बाश
डकर कम्पोज बिल्ड --नो-क्यास
```

> यो आदेश पूरा हुन केही मिनेट लाग्न सक्छ।

जब निर्माण समाप्त हुन्छ, तपाईले वातावरणलाई पृष्ठभूमि मोडमा चलाउन सक्नुहुन्छ:

``बाश
डकर कम्पोज अप -d
```

हामी अब एप्लिकेसन निर्भरताहरू स्थापना गर्न 'कम्पोजर स्थापना' चलाउनेछौं:

``बाश
docker कम्पोज exec एप कम्पोजर स्थापना
```

वातावरण सेटिङहरू प्रतिलिपि गर्नुहोस्:

``बाश
डकर रचना exec एप cp .env.local .env
```

'कारीगर' Laravel कमाण्ड-लाइन उपकरणसँग इन्क्रिप्शन कुञ्जी सेट गर्नुहोस्:

``बाश
docker कम्पोज exec एप।/artisan key:generate --ansi
```

DB र बीज नकली डाटा माइग्रेट:

``बाश
docker कम्पोज exec एप।/artisan migrate:fresh --seed
```

र फिलामेन्ट प्रशासक प्रयोगकर्ता थप्नुहोस्:

``बाश
docker कम्पोज exec एप।/artisan make:filament-user
```

र आफ्नो मनपर्ने ब्राउजरमा http://127.0.0.1:8000 खोल्नुहोस्। Laravel ब्लग प्रयोग गरेर खुसी!

## कन्टेनर भित्र कसरी प्रवेश गर्ने?

डकर कन्टेनरमा पहुँच:

``बाश
docker exec -ti laravel-blog-app bash
```

## लाइसेन्स

यो [MIT लाइसेन्स](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE) अन्तर्गत इजाजतपत्र प्राप्त खुला स्रोत सफ्टवेयर हो।


[![GitHub रिलीज](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![लाइसेन्स](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ laravel-blog)