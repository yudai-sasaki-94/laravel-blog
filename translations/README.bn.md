![ফিলামেন্ট অ্যাডমিন প্যানেল সহ লারাভেল ব্লগ](../docs/social-preview-en.png)

# ফিলামেন্ট অ্যাডমিন প্যানেল সহ লারাভেল ব্লগ

এটি হল [Laravel](https://laravel.com) [Filament](https://filamentphp.com) অ্যাডমিন প্যানেলের সাথে ব্লগ স্টার্টার কিট প্রকল্প।

এই রিপোজিটরির লক্ষ্য হল একটি সহজ অ্যাপ্লিকেশনের মাধ্যমে ভালো [Laravel](https://laravel.com) উন্নয়ন অনুশীলন দেখানো।

## বৈশিষ্ট্য

- 📚 পোস্ট তৈরি করা এবং সম্পাদনা করা
- 🥑 বিভাগ
- :fire: জনপ্রিয় পোস্ট
- :hatched_chick: [ফিলামেন্ট](https://filamentphp.com) এ তৈরি অ্যাডমিন প্যানেল

## বৈশিষ্ট্যগুলি অনুরোধ করা

একটি বৈশিষ্ট্যের অনুরোধ করতে একটি [নতুন সমস্যা](https://github.com/gomzyakov/laravel-blog/issues/new) খুলুন (অথবা যদি আপনি একটি বাগ খুঁজে পান)।

## কিভাবে স্থানীয়ভাবে ব্লগ চালাবেন?

প্রকল্প ক্লোন করুন:

``বাশ
git ক্লোন git@github.com:gomzyakov/laravel-blog.git
```

আমি বিশ্বাস করি আপনি ইতিমধ্যে ডকার ইনস্টল করেছেন। যদি না হয়, শুধু [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows) এ এটি করুন -ইনস্টল/) বা [লিনাক্স](https://docs.docker.com/desktop/install/linux-install/)।

নিম্নলিখিত কমান্ড দিয়ে `laravel-blog` ইমেজ তৈরি করুন:

``বাশ
ডকার কম্পোজ বিল্ড --নো-ক্যাশে
```

> এই কমান্ডটি সম্পূর্ণ হতে কয়েক মিনিট সময় লাগতে পারে।

বিল্ড শেষ হলে, আপনি এর সাথে পটভূমি মোডে পরিবেশ চালাতে পারেন:

``বাশ
ডকার রচনা আপ -d
```

আমরা এখন অ্যাপ্লিকেশন নির্ভরতা ইনস্টল করতে `কম্পোজার ইনস্টল` চালাব:

``বাশ
ডকার কম্পোজ exec অ্যাপ কম্পোজার ইনস্টল করুন
```

পরিবেশ সেটিংস অনুলিপি করুন:

``বাশ
ডকার কম্পোজ exec অ্যাপ cp .env.local .env
```

'কারিগর' লারাভেল কমান্ড-লাইন টুল দিয়ে এনক্রিপশন কী সেট করুন:

``বাশ
ডকার কম্পোজ exec অ্যাপ ./artisan key: জেনারেট --ansi
```

DB এবং বীজ জাল ডেটা মাইগ্রেট করুন:

``বাশ
ডকার কম্পোজ এক্সেক অ্যাপ।/শিল্পী মাইগ্রেট: ফ্রেশ --বীজ
```

এবং ফিলামেন্ট অ্যাডমিন ব্যবহারকারী যোগ করুন:

``বাশ
ডকার কম্পোজ exec অ্যাপ ./artisan make:filament-user
```

এবং আপনার প্রিয় ব্রাউজারে http://127.0.0.1:8000 খুলুন। Laravel ব্লগ ব্যবহার করে খুশি!

## কন্টেইনারের ভিতরে কিভাবে প্রবেশ করবেন?

ডকার কন্টেইনারে অ্যাক্সেস:

``বাশ
docker exec -ti laravel-blog-app bash
```

## লাইসেন্স

এটি [MIT লাইসেন্স](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE) এর অধীনে লাইসেন্সকৃত ওপেন-সোর্স সফ্টওয়্যার।


[![GitHub প্রকাশ](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![লাইসেন্স](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ লারাভেল-ব্লগ)