![Blog của Laravel với bảng quản trị Filament](../docs/social-preview-en.png)

_Read this in [other languages](./Translations.md)_

>This file is automatically translated. If you notice an error, please correct it yourself (by making a PR) or write about it in the [issues](https://github.com/gomzyakov/laravel-blog/issues).

# Blog Laravel với bảng quản trị Filament

Đây là dự án bộ công cụ khởi đầu blog [Laravel](https://laravel.com) với bảng quản trị [Filament](https://filavel.com).

Mục tiêu của kho lưu trữ này là giới thiệu các phương pháp phát triển [Laravel](https://laravel.com) tốt với một ứng dụng đơn giản.

## Đặc trưng

- 📚 Tạo và chỉnh sửa bài viết
- 🥑 Danh mục
- 🔥 Bài viết phổ biến
- 🎉 Bảng quản trị được xây dựng trên [Filament](https://filaphp.com)

## Yêu cầu tính năng

Mở [vấn đề mới](https://github.com/gomzykov/laravel-blog/issues/new) để yêu cầu một tính năng (hoặc nếu bạn tìm thấy lỗi).

## Làm cách nào để chạy blog cục bộ?

Sao chép dự án:

``` bash
git clone git@github.com:gomzykov/laravel-blog.git
```

Tôi tin rằng bạn đã cài đặt Docker. Nếu không, chỉ cần thực hiện trên [Mac](https://docs.docker.com/desktop/install/mac-install/), [Windows](https://docs.docker.com/desktop/install/windows -install/) hoặc [Linux](https://docs.docker.com/desktop/install/linux-install/).

Xây dựng hình ảnh `laravel-blog` bằng lệnh sau:

``` bash
docker soạn bản dựng --no-cache
```

>Lệnh này có thể mất vài phút để hoàn thành.

Khi quá trình xây dựng hoàn tất, bạn có thể chạy môi trường ở chế độ nền với:

``` bash
docker soạn thảo -d
```

Bây giờ chúng ta sẽ chạy `composer install` để cài đặt các phần phụ thuộc của ứng dụng:

``` bash
docker soạn ứng dụng thực thi cài đặt trình soạn thảo
```

Sao chép cài đặt môi trường:

``` bash
docker soạn ứng dụng thực thi cp .env.local .env
```

Đặt khóa mã hóa bằng công cụ dòng lệnh `artisan` Laravel:

``` bash
docker soạn ứng dụng thực thi ./artisan key:generate --ansi
```

Di chuyển DB và tạo dữ liệu giả:

``` bash
docker soạn ứng dụng thực thi ./artisan Migrate:fresh --seed
```

Và thêm người dùng quản trị Filament:

``` bash
docker soạn ứng dụng thực thi ./artisan make: fil-user
```

Và mở http://127.0.0.1:8000 trong trình duyệt yêu thích của bạn. Chúc bạn sử dụng Blog Laravel vui vẻ!

## Làm cách nào để vào trong container?

Truy cập vào vùng chứa Docker:

``` bash
docker exec -ti laravel-blog-app bash
```

## Giấy phép

Đây là phần mềm nguồn mở được cấp phép theo [Giấy phép MIT](https://github.com/gomzykov/php-code-style/blob/main/LICENSE).


[![Bản phát hành GitHub](https://img.shields.io/github/release/gomzykov/laravel-blog.svg)](https://github.com/gomzykov/laravel-blog/releases/latest)
[![giấy phép](https://img.shields.io/badge/Lince-MIT-green.svg)](https://github.com/gomzykov/laravel-blog/blob/development/LICENSE)
[![codecov](https://codecov.io/gh/gomzykov/laravel-blog/branch/main/graph/badge.svg?token=4CYTVMVUYV)](https://codecov.io/gh/gomzykov/ blog laravel)
