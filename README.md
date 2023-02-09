
# API_MOVIE_WITH_DB  

API movie dengan database mongo, yang di scrapping dari web brazil cine.xxxx.com. data video menggunakan dubbing bahasa portugis. jadi semua info movie beserta file video nya disimpan ke dalam database.



## Features

- Search
- Genre
- All Movie
- All Series
- Year ( Movie & Series by Year)
- New Release



## API Reference

#### Get New Release

```bash
  GET /new-release
```

#### Get Genre

```bash
  GET /genre
```

#### Get Year

```bash
  GET /year
```

#### Get Data Search

```bash
  GET /search?keyword={title}&page={pages}
```

| Parameter | Type     | Description                              |
| :-------- | :------- | :--------------------------------------- |
| `title`   | `string` | **Required** Judul Movie & Series        |
| `pages`   | `string` | **Required** nomor page untuk pagination |

#### Get Data By Genre

```bash
  GET /genre/{genre}?page={pages}
```

| Parameter | Type     | Description                                               |
| :-------- | :------- | :-------------------------------------------------------- |
| `genre    | `string` | **Required** nama genre yang diambil dari endpoint /genre |
| `pages`   | `string` | **Required** nomor page untuk pagination                  |

#### Get Data By Year

```bash
  GET /year/{year}?page={pages}
```

| Parameter | Type     | Description                               |
| :-------- | :------- | :---------------------------------------- |
| `year`    | `string` | **Required** tahun yang ingin ditampilkan |
| `page`    | `string` | **Required** nomor page untuk pagination  |

#### Get Data Movies

```bash
  GET /movies/:page
```

| Parameter | Type     | Description                              |
| :-------- | :------- | :--------------------------------------- |
| `page`    | `string` | **Required** nomor page untuk pagination |

#### Get Data Series

```bash
  GET /series/:page
```

| Parameter | Type     | Description                              |
| :-------- | :------- | :--------------------------------------- |
| `page`    | `string` | **Required** nomor page untuk pagination |

#### Get Data Detail

```bash
  GET  /detail/{type}?id={id}
```

| Parameter | Type     | Description                                                                            |
| :-------- | :------- | :------------------------------------------------------------------------------------- |
| `type`    | `string` | **Required** type sesuai dengan data id yang di ambil contoh : `series/movies/episode` |
| `id`      | `string` | **Required** id merupakan id movie/series/episode                                      |

#### Get Data Video

```bash
  POST  /Video
```

| Parameter | Type     | Description                                                             |
| :-------- | :------- | :---------------------------------------------------------------------- |
| `id`      | `string` | **Required** id video yang ingin di tampilkan, dapat dari movie/episode |
| `token`   | `string` | **Required** token yang didapatkan dari sinop                           |
