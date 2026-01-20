# Classic External Scrapers

Reliable ports of legacy anime scrapers for broad content coverage.

## 1. GogoAnime

Search GogoAnime (gogoanime3.co) for anime. (Not Working)

- **URL**: `/anime/gogoanime/:query`
- **Method**: `GET`
- **Response**: Array of `{ title, link, img, released }`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime/gogoanime/naruto"
```

## 2. Chia-Anime

Search Chia-Anime (chia-anime.su).(Not Working)

- **URL**: `/anime/chia-anime/:query`
- **Method**: `GET`
- **Response**: Array of `{ title, link, img }`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime/chia-anime/bleach"
```

## 3. Anime-Freak

Search Anime-Freak (animefreak.video).(Not Working)

- **URL**: `/anime/anime-freak/:query`
- **Method**: `GET`
- **Response**: Array of `{ title, link, img }`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime/anime-freak/one%20piece"
```

## 4. Animeland

Search Animeland (animeland.tv).

- **URL**: `/anime/animeland/:query`
- **Method**: `GET`
- **Response**: Array of `{ title, link }`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime/animeland/dragon%20ball"
```
