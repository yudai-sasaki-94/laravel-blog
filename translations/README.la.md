![Laravel blog with Filament admin panel]../docs/social-preview-en.png)

# Laravel blog ກັບ Filament admin panel

ນີ້​ແມ່ນ [Laravel](https://laravel.com) ໂຄງ​ການ​ຊຸດ​ການ​ເລີ່ມ​ຕົ້ນ​ຂອງ blog ກັບ [Filament](https://filamentphp.com) ກະ​ດານ​ບໍ​ລິ​ຫານ.

ເປົ້າໝາຍຂອງບ່ອນເກັບມ້ຽນນີ້ແມ່ນເພື່ອສະແດງການປະຕິບັດການພັດທະນາ [Laravel](https://laravel.com) ທີ່ດີດ້ວຍແອັບພລິເຄຊັນທີ່ງ່າຍດາຍ.

## ຄຸນ​ລັກ​ສະ​ນະ

- 📚ສ້າງແລະແກ້ໄຂຂໍ້ຄວາມ
- 🥑 ໝວດໝູ່
- :fire: ໂພສຍອດນິຍົມ
- :hatched_chick: ແຜງຄວບຄຸມທີ່ສ້າງຂຶ້ນໃນ [Filament](https://filamentphp.com)

## ລັກສະນະການຮ້ອງຂໍ

ເປີດ [ບັນຫາໃໝ່](https://github.com/gomzyakov/laravel-blog/issues/new) ເພື່ອຮ້ອງຂໍຄຸນສົມບັດ (ຫຼືຫາກທ່ານພົບຂໍ້ບົກພ່ອງ).

## ວິທີການດໍາເນີນການ blog ໃນທ້ອງຖິ່ນ?

Clone ໂຄງ​ການ​:

``ບັກ
git clone git@github.com:gomzyakov/laravel-blog.git
```

ຂ້ອຍເຊື່ອວ່າເຈົ້າໄດ້ຕິດຕັ້ງ Docker ແລ້ວ. ຖ້າບໍ່, ພຽງແຕ່ເຮັດມັນຢູ່ໃນ [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows -install/) ຫຼື [Linux](https://docs.docker.com/desktop/install/linux-install/).

ສ້າງຮູບພາບ 'laravel-blog' ດ້ວຍຄໍາສັ່ງຕໍ່ໄປນີ້:

``ບັກ
docker ຂຽນ build --no-cache
```

> ຄຳສັ່ງນີ້ອາດຈະໃຊ້ເວລາສອງສາມນາທີເພື່ອໃຫ້ສຳເລັດ.

ເມື່ອ​ການ​ກໍ່​ສ້າງ​ສໍາ​ເລັດ​, ທ່ານ​ສາ​ມາດ​ດໍາ​ເນີນ​ການ​ສະ​ພາບ​ແວດ​ລ້ອມ​ໃນ​ຮູບ​ແບບ​ພື້ນ​ຖານ​ທີ່​ມີ​:

``ບັກ
docker ປະກອບ -d
```

ຕອນນີ້ພວກເຮົາຈະດໍາເນີນການ 'ຕິດຕັ້ງ composer' ເພື່ອຕິດຕັ້ງການຂຶ້ນກັບແອັບພລິເຄຊັນ:

``ບັກ
docker ຕິດຕັ້ງ exec app composer
```

ສຳເນົາການຕັ້ງຄ່າສະພາບແວດລ້ອມ:

``ບັກ
docker ປະກອບ exec app cp .env.local .env
```

ຕັ້ງລະຫັດການເຂົ້າລະຫັດດ້ວຍເຄື່ອງມືເສັ້ນຄໍາສັ່ງ `ຊ່າງຝີມື` Laravel:

``ບັກ
docker ປະກອບ exec app ./artisan key:generate --ansi
```

ຍ້າຍຂໍ້ມູນປອມ DB ແລະແກ່ນ:

``ບັກ
docker ປະກອບ exec app ./artisan migrate:fresh --seed
```

ແລະເພີ່ມ Filament admin user:

``ບັກ
docker ປະກອບ exec app ./artisan make:filament-user
```

ແລະເປີດ http://127.0.0.1:8000 ໃນຕົວທ່ອງເວັບທີ່ທ່ານມັກ. ມີຄວາມສຸກກັບການໃຊ້ Laravel Blog!

## ວິທີການເຂົ້າໄປໃນຖັງ?

ການເຂົ້າເຖິງກ່ອງບັນຈຸ Docker:

``ບັກ
docker exec -ti laravel-blog-app bash
```

## ໃບອະນຸຍາດ

ນີ້ແມ່ນຊອບແວແຫຼ່ງເປີດທີ່ໄດ້ຮັບອະນຸຍາດພາຍໃຕ້ [ໃບອະນຸຍາດ MIT](https://github.com/gomzyakov/php-code-style/blob/main/LICENSE).


[![ການປ່ອຍ GitHub](https://img.shields.io/github/release/gomzyakov/laravel-blog.svg)](https://github.com/gomzyakov/laravel-blog/releases/latest)
[![license](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/gomzyakov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzyakov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzyakov/ laravel-blog)