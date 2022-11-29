
# REST-API MOVIE (Scrapping)

Api movie tanpa database, melainkan hasil Scrapping dari web cine.xxxx.com




## API Reference

#### Get New Release

```bash
  GET v1/app/new-release
```


#### Get Data Search

```bash
  GET v1/app/search/:keyword/:page
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `keyword`  | `string` | **Required** keyword yang ingin dicari      |
| `page`     | `string` | **Required** nomor page untuk pagination    |

 
#### Get Genre

```bash
  GET v1/app/genre
```
#### Get Data By Genre

```bash
  GET v1/app/genre/:slug/:page
```

| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `slug`     | `string` | **Required** slug pada item endpoint genre |
| `page`     | `string` | **Required** nomor page untuk pagination    |

#### Get Data Year

```bash
  GET v1/app/year
```

#### Get Data By Year

```bash
  GET v1/app/year/:slug/:page
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `slug`     | `string` | **Required** tahun yang ingin ditampilkan   |
| `page`     | `string` | **Required** nomor page untuk pagination    |

 
#### Get Data Movies

```bash
  GET v1/app/movies/:page
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `page`     | `string` | **Required** nomor page untuk pagination    |
 
#### Get Data Movies Detail

```bash
  GET v1/app/movies-detail/:slug/:title
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `slug`     | `string` | **Required** slug pada item endpoint movies |
| `title`    | `string` | **Required** title pada slug di item endpoint movies |

#### Get Data Movies Video

```bash
  GET v1/app/movies-video/:id
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `id`       | `string` | **Required** id yang diambil dari videoid di movies detail |


#### Get Data Series

```bash
  GET v1/app/series/:page
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `page`     | `string` | **Required** nomor page untuk pagination    |
 
#### Get Data Series Detail

```bash
  GET v1/app/series-detail/:slug/:title
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `slug`     | `string` | **Required** slug pada item endpoint series |
| `title`    | `string` | **Required** title pada slug di item endpoint series |

#### Get Data Episode Detail

```bash
  GET v1/app/series-eps/:slug/:title
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `slug`     | `string` | **Required** slug pada item endpoint series |
| `title`    | `string` | **Required** title pada slug di item endpoint series |

#### Get Data Series Video

```bash
  GET v1/app/series-video/:id
```
| Parameter  | Type     | Description                                 |
| :--------- | :------- | :------------------------------------------ |
| `id`       | `string` | **Required** id yang diambil dari videoid di episode detail |

 


## Features

- New Release
- Search
- Genre
- Data By Genre
- Year
- Data By Year
- List Movies
- List Series
- List Episode

