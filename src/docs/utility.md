# Utility & Meta APIs

Various utility endpoints ported from `anime-api` for quotes, facts, and image recognition.

## 1. Random Quotes

Get random quotes or quotes by specific anime. (Not Working)

- **URL**: `/anime-api/quotes/random`
- **Method**: `GET`
- **Query Params**: `anime` (optional)

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime-api/quotes/random?anime=Naruto"
```

## 2. Anime Facts

Get facts about a specific anime.

- **URL**: `/anime-api/facts/:anime`
- **Method**: `GET`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime-api/facts/naruto"
```

## 3. Image Trace (trace.moe)

Trace back an anime scene from an image URL.

- **URL**: `/anime-api/trace`
- **Method**: `POST`
- **Body**: `{ "imageUrl": "..." }`

### 🧪 Test Module

```bash
curl -X POST "http://localhost:4000/api/v1/anime-api/trace" \
     -H "Content-Type: application/json" \
     -d '{"imageUrl": "https://images.plurk.com/32B15UXxymfSMwKGTObY5e.jpg"}'
```

## 4. Anime Images (Nekos.best)

Get various types of anime images (waifu, neko, shinobu, etc.).

- **URL**: `/anime-api/images/:type`
- **Method**: `GET`

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime-api/images/neko"
```

## 5. Advanced Waifu Search (waifu.im)

Search specifically for waifu images with tag filtering.

- **URL**: `/anime-api/waifu`
- **Method**: `GET`
- **Query Params**: `tags` (optional, e.g. `maid`)

### 🧪 Test Module

```bash
curl -X GET "http://localhost:4000/api/v1/anime-api/waifu?tags=maid"
```
