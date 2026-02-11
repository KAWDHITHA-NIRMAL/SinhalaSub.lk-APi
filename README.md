
<p align="center">
  <img src="https://sinhalasub.lk/wp-content/uploads/2025/10/icon-1.png" alt="Main Icon" />
</p>

# 🎬 SinhalaSub Scraper API

> A simple API to search, browse, and fetch movies & TV shows from **SinhalaSub.lk**.
> Built by **K. Nirmal** | `CodeXSL Developer`

---

## 🌟 Base URL

```
https://sinhalasub-lk.netlify.app
```

All endpoints are prefixed with `https://sinhalasub-lk.netlify.app`.

---

## 📚 Endpoints

### 1️⃣ Search Content

Search for movies or TV shows globally.

**Endpoint:**

```
GET /api/search?query=<Film Or Tv Show Name>
```

**Query Parameters:**

| Parameter | Description                 | Default |
| --------- | --------------------------- | ------- |
| query     | Movie or TV show name/term  | -       |

**Example Request:**

```bash
GET https://sinhalasub-lk.netlify.app/api/search?query=Night
```

**Example Response:**

```json
{
  "success": true,
  "creator": "Kawdhitha Nirmal",
  "search": "Night",
  "totalPages": 4,
  "totalResults": 61,
  "results": [
    {
      "title": "Nellikkampoyil Night Riders (2025) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
      "link": "https://sinhalasub.lk/movies/nellikkampoyil-night-riders-2025-sinhala-subtitles/",
      "thumbnail": "https://image.tmdb.org/t/p/w500/fni5RRvoJ4PIQnqW3vICXamB1Uw.jpg",
      "type": "movie"
    },
    {
      "title": "A Knight of the Seven Kingdoms (2026) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
      "link": "https://sinhalasub.lk/tvshows/a-knight-of-the-seven-kingdoms-sinhala-subtitles/",
      "thumbnail": "https://image.tmdb.org/t/p/w500/6igvNs5VJB4ryBLgjjXksDVs0Fm.jpg",
      "type": "tvshow"
    },
    {
      "title": "Night Watch (2004) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
      "link": "https://sinhalasub.lk/movies/night-watch-2004-sinhala-subtitles/",
      "thumbnail": "https://image.tmdb.org/t/p/w500/hRDJRgb7wEubLhPWFrl6sS816Tm.jpg",
      "type": "movie"
    },
    {
      "title": "Meesha (2025) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
      "link": "https://sinhalasub.lk/movies/meesha-2025-sinhala-subtitles/",
      "thumbnail": "https://image.tmdb.org/t/p/w500/12UtqB9sCmDmeYHeSGsyPYHcHfrSH7GuiX.jpg",
      "type": "movie"
    }
  ]
}
```

---

### 2️⃣ Get Movie Details

Fetch movie details and download links.

**Endpoint:**

```
GET /api/movie?url=<movie_url>
```

**Example Request:**

```bash
GET https://sinhalasub-lk.netlify.app//api/movie?url=https://sinhalasub.lk/movies/the-curse-of-the-necklace-2024-sinhala-subtitles/
```

**Example Response:**

```json
{
  "success": true,
  "creator": "Kawdhitha Nirmal",
  "source": "https://sinhalasub.lk/movies/the-curse-of-the-necklace-2024-sinhala-subtitles",
  "title": "The Curse of the Necklace (2024) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
  "poster": "https://image.tmdb.org/t/p/w500/tWrYpICZChiPwRnc8SkvxBFBE3y.jpg",
  "rating": "4",
  "imdb": "4.5",
  "duration": "95 min",
  "quality": "WEB-DL",
  "views": "1299 views",
  "genres": [
    "Horror",
    "Mystery",
    "Thriller"
  ],
  "description": "After separating due to his unpredictable alcohol infused temper, Frank try to win his wife Laura back by giving her a beautiful antique necklace he finds in an old 1938 evidence bag at the station. Unfortunately, the necklace is a conduit for the tormented soul of an evil boy from long ago, and Laura and her daughters find themselves in terrible danger from a little boy who no longer exists.",
  "stars": [
    "Brynne Kurland",
    "Christina Moore",
    "Danielia Maximillian-Almeda",
    "Felix Solis",
    "Henry Thomas",
    "Jacob Moran",
    "Madeleine McGraw",
    "Roma Maffia",
    "Sarah Lind",
    "Violet McGraw"
  ],
  "cast": [
    {
      "name": "Brynne Kurland",
      "image": "https://image.tmdb.org/t/p/w185/k3cCbOQzihpznXEe1bNk5H26vEK.jpg"
    },
    {
      "name": "Christina Moore",
      "image": "https://sinhalasub.lk/wp-content/themes/zetaflix/assets/img/avatars/default.png"
    },
    {
      "name": "Danielia Maximillian-Almeda",
      "image": "https://image.tmdb.org/t/p/w185/7Jsf7YJqD0GzBB5btKoDnxY1bJU.jpg"
    },
    {
      "name": "Felix Solis",
      "image": "https://image.tmdb.org/t/p/w185/hEiRxsPybmlmoynqw3UeA9AiSEY.jpg"
    },
    {
      "name": "Henry Thomas",
      "image": "https://image.tmdb.org/t/p/w185/l5OZ4qrrRGnEPeNhZ8PcL5vhwOI.jpg"
    },
    {
      "name": "Jacob Moran",
      "image": "https://image.tmdb.org/t/p/w185/krzzHeA8dEJTqeIgcf6NimxTeLe.jpg"
    },
    {
      "name": "Madeleine McGraw",
      "image": "https://image.tmdb.org/t/p/w300/vdd0a58A1272zB6lvYuK5OEjO6.jpg"
    },
    {
      "name": "Roma Maffia",
      "image": "https://image.tmdb.org/t/p/w185/oEfa2NUJJNo4zg74eB5oY86tyip.jpg"
    },
    {
      "name": "Sarah Lind",
      "image": "https://image.tmdb.org/t/p/w185/v4EGfayvyrgq2y53xb9qWwrvqx.jpg"
    },
    {
      "name": "Violet McGraw",
      "image": "https://image.tmdb.org/t/p/w185/9o0uBCFg7ridSREaXLvReWzggUz.jpg"
    }
  ],
  "downloads": [
    {
      "server": "AkiraBox",
      "url": "https://sinhalasub.lk/links/veup52v1yw/",
      "quality": "FHD 1080p",
      "size": "2.39 GB"
    },
    {
      "server": "AkiraBox",
      "url": "https://sinhalasub.lk/links/1czzhb4xlh/",
      "quality": "HD 720p",
      "size": "1.24 GB"
    },
    {
      "server": "AkiraBox",
      "url": "https://sinhalasub.lk/links/a7pijivkl7/",
      "quality": "SD 480p",
      "size": "640 MB"
    },
    {
      "server": "DLServer-01",
      "url": "https://sinhalasub.lk/links/donyx8tlma/",
      "quality": "FHD 1080p",
      "size": "2.39 GB"
    },
    {
      "server": "DLServer-01",
      "url": "https://sinhalasub.lk/links/md6nnyflrw/",
      "quality": "HD 720p",
      "size": "1.24 GB"
    },
    {
      "server": "DLServer-01",
      "url": "https://sinhalasub.lk/links/wbdpoiozc3/",
      "quality": "SD 480p",
      "size": "640 MB"
    },
    {
      "server": "DLServer-02",
      "url": "https://sinhalasub.lk/links/rqodzi8stg/",
      "quality": "FHD 1080p",
      "size": "2.39 GB"
    },
    {
      "server": "DLServer-02",
      "url": "https://sinhalasub.lk/links/6aukokbisd/",
      "quality": "HD 720p",
      "size": "1.24 GB"
    },
    {
      "server": "DLServer-02",
      "url": "https://sinhalasub.lk/links/uc9ttdkx7o/",
      "quality": "SD 480p",
      "size": "640 MB"
    },
    {
      "server": "Telagram",
      "url": "https://sinhalasub.lk/links/sv4ns9cl7i/",
      "quality": "FHD 1080p",
      "size": "2.39 GB"
    },
    {
      "server": "Telagram",
      "url": "https://sinhalasub.lk/links/t6stbbscie/",
      "quality": "HD 720p",
      "size": "1.24 GB"
    },
    {
      "server": "Telagram",
      "url": "https://sinhalasub.lk/links/up9o1ualk3/",
      "quality": "SD 480p",
      "size": "640 MB"
    },
    {
      "server": "Subtitles",
      "url": "https://sinhalasub.lk/links/die2m5esr1/",
      "quality": "SRT",
      "size": "----"
    }
  ],
  "gallery": [
    "https://image.tmdb.org/t/p/w300/rqH9e1SVLPEY6jcoXvVKAKxwIwJ.jpg",
    "https://image.tmdb.org/t/p/w300/4Gyp48lFkmcxu20Fs7ukhTIuzSn.jpg",
    "https://image.tmdb.org/t/p/w300/OCyzgg47inyeMUcXttrsT9xKbe.jpg",
    "https://image.tmdb.org/t/p/w300/yewIlMzj9vzGvlh0EDzjNsdNdRx.jpg",
    "https://image.tmdb.org/t/p/w300/8uFSl2oHyUNikI93nRar6ZZVnSG.jpg",
    "https://image.tmdb.org/t/p/w300/98NNABrVq3vep3UYPfB0xq05j6R.jpg",
    "https://image.tmdb.org/t/p/w300/kpgRg4AtSF8sB0ZNFj4XM3IoTR5.jpg",
    "https://image.tmdb.org/t/p/w300/m38DGcV9hebIPQivOm4w1mKXRS1.jpg",
    "https://image.tmdb.org/t/p/w300/rAa55JWEP2Iu1DQ40iQJpox2xBT.jpg",
    "https://image.tmdb.org/t/p/w300/gPv6clvUShX02IZ1p9scgUYRs3w.jpg"
  ]
}
```

---

### 3️⃣ Get TV Show Details

Fetch TV show information and episodes.

**Endpoint:**

```
GET /api/tv?url=<tv_show_url>
```

**Example Request:**

```bash
GET https://sinhalasub-lk.netlify.app/api/tv?url=https://sinhalasub.lk/tvshows/stranger-things-2016-sinhala-subtitles
```

**Example Response:**

```json
{
  "success": true,
  "creator": "Kawdhitha Nirmal",
  "title": "Stranger Things (2016-2025) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
  "poster": "https://image.tmdb.org/t/p/w500/cVxVGwHce6xnW8UaVUggaPXbmoE.jpg",
  "trailer": "PssKpzB0Ah0",
  "genres": [
    "Action & Adventure",
    "Mystery",
    "Sci-Fi & Fantasy"
  ],
  "description": "When a young boy vanishes, a small town uncovers a mystery involving secret experiments, terrifying supernatural forces, and one strange little girl.",
  "rating": 4,
  "votes": 4,
  "views": 39854,
  "total_seasons": 5,
  "total_episodes": 8,
  "seasons": {
    "1": [
      {
        "episode_number": 1,
        "title": "Episode 01",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/uLES7sRpy7Ih6Kr6XCaYj1GyfTw.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e01/"
      },
      {
        "episode_number": 2,
        "title": "Episode 02",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/8iA56ugQyHZmX81wSsNqwXjCE6F.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e02/"
      },
      {
        "episode_number": 3,
        "title": "Episode 03",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/5snULpWQWp7aqFto7UbRcEkEyyS.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e03/"
      },
      {
        "episode_number": 4,
        "title": "Episode 04",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/60wmC1e20HV8gu688GAhsWxqxPx.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e04/"
      },
      {
        "episode_number": 5,
        "title": "Episode 05",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/exT4NW9EdXG1qLZHKJnRpq3gh1H.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e05/"
      },
      {
        "episode_number": 6,
        "title": "Episode 06",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/lNS6qycyucewz3duTr1tf1LU688.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e06/"
      },
      {
        "episode_number": 7,
        "title": "Episode 07",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/fjsTVEnqTKUO0GJSpiWKBZRUBcx.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e07/"
      },
      {
        "episode_number": 8,
        "title": "Episode 08 [S01 Last]",
        "date": "Jul. 15, 2016",
        "thumbnail": "https://image.tmdb.org/t/p/w500/1teJ5dbuepfqOOs9uYhYTUjr2qs.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s01e08/"
      }
    ],
    "2": [
      {
        "episode_number": 1,
        "title": "Episode 01",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/efz0MgPAxPw11PIeAJNgKKg3Paa.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e01/"
      },
      {
        "episode_number": 2,
        "title": "Episode 02",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/3gzPnRilyASmcoSyUKXhaD5ofhr.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e02/"
      },
      {
        "episode_number": 3,
        "title": "Episode 03",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/792NQjFydcr5ucb1sga55LS6Vt3.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e03/"
      },
      {
        "episode_number": 4,
        "title": "Episode 04",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/wZXeV5cWC1RuaCls2mm6imzchnN.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e04/"
      },
      {
        "episode_number": 5,
        "title": "Episode 05",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/oshY3LAwQRzhcjmEEr7EbOnypuU.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e05/"
      },
      {
        "episode_number": 6,
        "title": "Episode 06",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/d90nCiTEACFEUd3fcX8DrLBi5DL.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e06/"
      },
      {
        "episode_number": 7,
        "title": "Episode 07",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/kgOaaTbAutwAoA7tkVzYCfTjPXn.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e07/"
      },
      {
        "episode_number": 8,
        "title": "Episode 08",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/vuLea0DA9rYc9Y4M2Ic28CXL4Al.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e08/"
      },
      {
        "episode_number": 9,
        "title": "Episode 09 [S02 Last]",
        "date": "Oct. 27, 2017",
        "thumbnail": "https://image.tmdb.org/t/p/w500/cxCf7O5WPHfyXb7PLSJCG6EvXc3.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s02e09/"
      }
    ],
    "3": [
      {
        "episode_number": 1,
        "title": "Episode 01",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/g1iZmyn42qSFkXhw6gjoNE0diKb.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e01/"
      },
      {
        "episode_number": 2,
        "title": "Episode 02",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/qDlMvdlRGzIGtKYdV9lktEUM4vj.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e02/"
      },
      {
        "episode_number": 3,
        "title": "Episode 03",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/oaYdVvYwnvoQ7SLelKUcaAt0HKJ.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e03/"
      },
      {
        "episode_number": 4,
        "title": "Episode 04",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/tEgd6fXKngAG8eC92dH7ey6Y4eA.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e04/"
      },
      {
        "episode_number": 5,
        "title": "Episode 05",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/cxIZ4btU6h9GQM1Fn0kotuaXlwo.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e05/"
      },
      {
        "episode_number": 6,
        "title": "Episode 06",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/dZKsMHJm8DPdBuqFcZxdIulrpNs.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e06/"
      },
      {
        "episode_number": 7,
        "title": "Episode 07",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/6QA91GJK2ze1EaGPEKhil9MJIXx.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e07/"
      },
      {
        "episode_number": 8,
        "title": "Episode 08 [S03 Last]",
        "date": "Jul. 04, 2019",
        "thumbnail": "https://image.tmdb.org/t/p/w500/5YcjTWas07RteM9lssOzL9UhmJh.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s03e08/"
      }
    ],
    "4": [
      {
        "episode_number": 1,
        "title": "Episode 01",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/xeNKubDmPiMraW4hXqzEBrN6f4A.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e01/"
      },
      {
        "episode_number": 2,
        "title": "Episode 02",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/lSSWqv7XrO51uY2uc4lql9Hub3f.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e02/"
      },
      {
        "episode_number": 3,
        "title": "Episode 03",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/6q1UM63T5tiQcWrbsJvY3bunkyZ.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e03/"
      },
      {
        "episode_number": 4,
        "title": "Episode 04",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/u3LeFRR7AhyPp4y0Ii7hpkD488b.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e04/"
      },
      {
        "episode_number": 5,
        "title": "Episode 05",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/yvXXeBv4zfDgwcZyxqH5LJAe4oV.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e05/"
      },
      {
        "episode_number": 6,
        "title": "Episode 06",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/9EbhReDcbfmqLhDBg0Rn97z4lT.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e06/"
      },
      {
        "episode_number": 7,
        "title": "Episode 07",
        "date": "May. 27, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/n64hMYFaVunT8jqSVgYq5qt0Vbn.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e07/"
      },
      {
        "episode_number": 8,
        "title": "Episode 08",
        "date": "Jul. 01, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/sdNa4Z49RTZDkezFAMg00hciFZZ.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e08/"
      },
      {
        "episode_number": 9,
        "title": "Episode 09 [S04 Last]",
        "date": "Jul. 01, 2022",
        "thumbnail": "https://image.tmdb.org/t/p/w500/fvoa0Hosu4yK7TUiHglV8TvjMUB.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s04e09/"
      }
    ],
    "5": [
      {
        "episode_number": 1,
        "title": "Episode 01",
        "date": "Nov. 26, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/jnpSxSMdFAj4dtF59agzgmKM9fg.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e01/"
      },
      {
        "episode_number": 2,
        "title": "Episode 02",
        "date": "Nov. 26, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/dI8N4IQpZNKloK4Dw6MugpSrwMS.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e02/"
      },
      {
        "episode_number": 3,
        "title": "Episode 03",
        "date": "Nov. 26, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/iCsM4oeBM9PIESD6PJw7mWO1xbl.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e03/"
      },
      {
        "episode_number": 4,
        "title": "Episode 04",
        "date": "Nov. 26, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/mp6nFiganZCbieJ0wSjIHz7bS8r.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e04/"
      },
      {
        "episode_number": 5,
        "title": "Episode 05",
        "date": "Dec. 25, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/4dnRX3S1II3NGkrnwCFZkYpgK83.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e05/"
      },
      {
        "episode_number": 6,
        "title": "Episode 06",
        "date": "Dec. 25, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/gGrxsT3YBcYhX4RfqXUn1xHL1p1.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e06/"
      },
      {
        "episode_number": 7,
        "title": "Episode 07",
        "date": "Dec. 25, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/WHdrgCxqNDuOIf65cW9It3XSZW.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e07/"
      },
      {
        "episode_number": 8,
        "title": "Episode 08 [End]",
        "date": "Dec. 31, 2025",
        "thumbnail": "https://image.tmdb.org/t/p/w500/qYSB9DA25yveOfw7HUgkw7vXCjv.jpg",
        "url": "https://sinhalasub.lk/episodes/stranger-things-s05e08/"
      }
    ]
  },
  "gallery": [
    "https://image.tmdb.org/t/p/original/4wOb6k75YGl68wUrMcPAvFJxiyq.jpg",
    "https://image.tmdb.org/t/p/original/8zbAoryWbtH0DKdev8abFAjdufy.jpg",
    "https://image.tmdb.org/t/p/original/56v2KjBlU4XaOv9rVYEQypROD7P.jpg",
    "https://image.tmdb.org/t/p/original/fBL749MrsPqCMsiRaWBFExT3Fwp.jpg",
    "https://image.tmdb.org/t/p/original/kiFJZHRyTV207BhLRtUu3sAsJKh.jpg",
    "https://image.tmdb.org/t/p/original/8CbWGYaIPRPVL9UGiV310CII8WC.jpg",
    "https://image.tmdb.org/t/p/original/ekLmP9wccC47PC83eJuklEy0twf.jpg",
    "https://image.tmdb.org/t/p/original/2MaumbgBlW1NoPo3ZJO38A6v7OS.jpg",
    "https://image.tmdb.org/t/p/original/sqVXe7s3QAvr9WObl8Xo88GGoL0.jpg",
    "https://image.tmdb.org/t/p/original/nvMoOlC7HHZ9U4WknwwGOVefvnI.jpg"
  ]
}
```

---

### 4️⃣ Get Episode Embed / Streaming Link

Fetch episode streaming URLs or embed links.

**Endpoint:**

```
GET /api/episode?url=<episode_url>
```

**Example Request:**

```bash
GET https://sinhalasub-lk.netlify.app/api/episode?url=https://sinhalasub.lk/episodes/stranger-things-s05e01
```

**Example Response:**

```json
{
  "success": true,
  "creator": "Kawdhitha Nirmal",
  "title": "Stranger Things:- S05:E01",
  "episode_title": "Episode 01",
  "serie_name": "Stranger Things",
  "rating": 5,
  "votes": 1,
  "quality": "WEB-DL",
  "views": "5092 views",
  "description": null,
  "gallery": [
    "https://image.tmdb.org/t/p/original/jnpSxSMdFAj4dtF59agzgmKM9fg.jpg",
    "https://image.tmdb.org/t/p/original/mSbNRxwtFPBb3rhzJgHyTDePz6v.jpg",
    "https://image.tmdb.org/t/p/original/mjoJIjtYpbwMoncMqykHJLiGENl.jpg",
    "https://image.tmdb.org/t/p/original/aOOOdhkmhncbikMVqXfVxwQ6lQw.jpg"
  ],
  "downloads": {
    "DLServer-01": [
      {
        "name": "DLServer-01",
        "link": "https://sinhalasub.lk/links/88krmhny4n/",
        "quality": "FHD 1080p",
        "size": "1.70 GB",
        "clicks": "189"
      },
      {
        "name": "DLServer-01",
        "link": "https://sinhalasub.lk/links/fh0fwthone/",
        "quality": "HD 720p",
        "size": "844 MB",
        "clicks": "262"
      },
      {
        "name": "DLServer-01",
        "link": "https://sinhalasub.lk/links/in5dag6eok/",
        "quality": "SD 480p",
        "size": "436 MB",
        "clicks": "237"
      }
    ],
    "DLServer-02": [
      {
        "name": "DLServer-02",
        "link": "https://sinhalasub.lk/links/zgjjjivrcu/",
        "quality": "FHD 1080p",
        "size": "1.70 GB",
        "clicks": "67"
      },
      {
        "name": "DLServer-02",
        "link": "https://sinhalasub.lk/links/y62mldhuzv/",
        "quality": "HD 720p",
        "size": "844 MB",
        "clicks": "84"
      },
      {
        "name": "DLServer-02",
        "link": "https://sinhalasub.lk/links/9wfkeiw1gn/",
        "quality": "SD 480p",
        "size": "436 MB",
        "clicks": "79"
      }
    ],
    "telagram": [
      {
        "name": "Telagram",
        "link": "https://sinhalasub.lk/links/d52byfzbyj/",
        "quality": "FHD 1080p",
        "size": "1.70 GB",
        "clicks": "111"
      },
      {
        "name": "Telagram",
        "link": "https://sinhalasub.lk/links/m57tklno71/",
        "quality": "HD 720p",
        "size": "844 MB",
        "clicks": "197"
      },
      {
        "name": "Telagram",
        "link": "https://sinhalasub.lk/links/eus24edfi5/",
        "quality": "SD 480p",
        "size": "436 MB",
        "clicks": "171"
      }
    ]
  }
}
```

---

### 5️⃣ Download Movie or Episode

Fetch direct download links.

**Endpoint:**

```
GET /api/dl?url=<movie_or_episode_Dl-url>
```

**Example Request:**

```bash
GET https://sinhalasub-lk.netlify.app/api/dl?url=https://sinhalasub.lk/links/88krmhny4n/
```

**Example Response:**

```json
{
  "success": true,
  "creator": "Kawdhitha Nirmal",
  "title": "Continue",
  "url": "https://cdn.sinhalasub.net/4095/Stranger.Things.S05E01%201080p.mp4"
}
```

---

## ⚡ Features

* ✅ Search movies & TV shows
* ✅ Fetch movie details + download links
* ✅ Get TV show seasons & episodes
* ✅ Stream or embed episode links
* ✅ Download movies or episodes directly
* 🌍 CORS enabled (works on any website)

---

## 👨‍💻 Creator Info

```json
{
  "creator": "K. Nirmal",
  "role": "CodeXSL Developer"
}
```

---

## 📝 Notes

* All URLs are **directly fetchable** via API.
* Works for **movies, TV shows, and individual episodes**.
* Can be used in **web apps, mobile apps, dashboards**.
* Full Project Develope By K.Nirmal🚀.
