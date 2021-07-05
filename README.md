# Penggunaan SSO PNJ di Aplikasi Desktop

Aplikasi ini merupakan aplikasi desktop yang dibuat menggunakan electro, dan menggunakan library [AppAuth-JS](https://github.com/openid/AppAuth-JS) untuk flow Open ID Connect.


## Development

Aplikasi ini dibuat dengan menggunakan bahasa pemrograman [TypeScript](https://typescriptlang.org).


## Quick Start

Karena dasar dari protokol OAuth 2.0 menggunakan browser redirect, maka aplikasi desktop dapat menggunakan beberapa library user agent yang dapat mengalihkan user ke SSO PNJ.

Client yang akan digunakan untuk aplikasi desktop tidak memiliki `client_secret`
```dotenv
CLIENT_ID=d3927f75-909e-xxxx-46fdd9157e6c
```

Karena tidak memiliki `client_secret` maka mohon dijaga kerahasian `client_id` yang Anda dapatkan.

### Menjalankan Aplikasi Demo Ini

* Install versi terbaru dari [Node](https://nodejs.org/en/) (atau melalui
  [NVM](https://github.com/creationix/nvm)
  Node Version Manager).

* Gunakan `nvm install` untuk menginstall versi node yang direkomendasikan.

* Install [Yarn](https://yarnpkg.com/en/docs/install) package manager.

### Instalasi dependency
* `yarn install` atau `npm install` untuk instalasi dependency (terdapat dalam `package.json`).

Anda dapat memulai aplikasi ini sekarang.

### Development Workflow

Jalankan script berikut untuk menjalankan program.

* `yarn run dev` atau `npm run-script dev` akan menjalankan aplikasi ini. Script ini juga akan memulai compiler TypeScript dalam mode `watch`, dan secara otomatis akan meng-compile ulang aplikasi saat Anda membuat perubahan. Cukup reload aplikasi elektron untuk melihat perubahan yang Anda buat.

* `yarn start` atau `npm start` untuk menjalankan aplikasi secara normal.
