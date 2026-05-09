# 🚀 FreeAPI

> A curated collection of **1000+ free public APIs** for developers, organized by category.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 📖 What is FreeAPI?

FreeAPI is a community-driven, open-source collection of free public APIs. It's designed to help developers quickly discover and integrate APIs into their projects — from weather data to machine learning, from anime to government open data.

**Why FreeAPI?**
- ✅ **1000+ APIs** across 50+ categories
- ✅ **Structured JSON** — machine-readable, easy to integrate
- ✅ **Always free** — only APIs with free tiers are listed
- ✅ **Community-driven** — contributions welcome

---

## 📊 Quick Stats

| Metric | Value |
|:---|:---|
| Total APIs | 1,092 |
| Categories | 51 |
| All Free | ✅ |
| JSON Format | ✅ |

---

## 🗂 Categories

| Category | Count | Category | Count |
|:---|:---|:---|:---|
| [Animals](#animals) | 26 | [Anime](#anime) | 16 |
| [Anti-Malware](#anti-malware) | 13 | [Art & Design](#art--design) | 20 |
| [Authentication & Authorization](#authentication--authorization) | 6 | [Blockchain](#blockchain) | 7 |
| [Books](#books) | 15 | [Business](#business) | 20 |
| [Calendar](#calendar) | 13 | [Cloud Storage & File Sharing](#cloud-storage--file-sharing) | 17 |
| [Continuous Integration](#continuous-integration) | 6 | [Cryptocurrency](#cryptocurrency) | 51 |
| [Currency Exchange](#currency-exchange) | 12 | [Data Validation](#data-validation) | 7 |
| [Development](#development) | 72 | [Dictionaries](#dictionaries) | 13 |
| [Documents & Productivity](#documents--productivity) | 21 | [Email](#email) | 14 |
| [Entertainment](#entertainment) | 6 | [Environment](#environment) | 12 |
| [Events](#events) | 3 | [Finance](#finance) | 29 |
| [Food & Drink](#food--drink) | 21 | [Games & Comics](#games--comics) | 65 |
| [Geocoding](#geocoding) | 58 | [Government](#government) | 84 |
| [Health](#health) | 23 | [Jobs](#jobs) | 14 |
| [Machine Learning](#machine-learning) | 13 | [Music](#music) | 23 |
| [News](#news) | 15 | [Open Data](#open-data) | 33 |
| [Open Source Projects](#open-source-projects) | 9 | [Patent](#patent) | 2 |
| [Personality](#personality) | 16 | [Phone](#phone) | 4 |
| [Photography](#photography) | 27 | [Programming](#programming) | 5 |
| [Science & Math](#science--math) | 31 | [Security](#security) | 29 |
| [Shopping](#shopping) | 10 | [Social](#social) | 33 |
| [Sports & Fitness](#sports--fitness) | 27 | [Test Data](#test-data) | 21 |
| [Text Analysis](#text-analysis) | 12 | [Tracking](#tracking) | 5 |
| [Transportation](#transportation) | 41 | [URL Shorteners](#url-shorteners) | 16 |
| [Vehicle](#vehicle) | 6 | [Video](#video) | 25 |
| [Weather](#weather) | 25 | | |

---

## 📦 Data Formats

### JSON (Recommended)

The full API collection is available as structured JSON:

```bash
curl -O https://raw.githubusercontent.com/AIPMAndy/FreeAPI/main/apis.json
```

**Schema:**

```json
{
  "source": "public-apis/public-apis",
  "total": 1092,
  "categories": {
    "Animals": [
      {
        "name": "Cat Facts",
        "url": "https://catfact.ninja/",
        "description": "Random cat facts",
        "auth": "No",
        "https": "Yes",
        "cors": "Yes"
      }
    ]
  }
}
```

### Markdown

Browse the full list directly in this README below, or check individual category files in the [`categories/`](categories/) directory.

---

## 🔍 Featured APIs

| API | Category | Description | Auth |
|:---|:---|:---|:---|
| [OpenWeatherMap](https://openweathermap.org/api) | Weather | Weather data for any location | `apiKey` |
| [NewsAPI](https://newsapi.org/) | News | Live news headlines & articles | `apiKey` |
| [CoinGecko](https://www.coingecko.com/api) | Cryptocurrency | Crypto prices, market data | No |
| [REST Countries](https://restcountries.com/) | Open Data | Country information | No |
| [JokeAPI](https://jokeapi.dev/) | Entertainment | Jokes in various categories | No |
| [PokeAPI](https://pokeapi.co/) | Games & Comics | Pokémon data | No |
| [JSONPlaceholder](https://jsonplaceholder.typicode.com/) | Development | Fake REST API for testing | No |
| [NASA API](https://api.nasa.gov/) | Science & Math | Space & earth science data | `apiKey` |
| [GitHub API](https://docs.github.com/rest) | Development | GitHub platform data | `OAuth` |
| [The Dog API](https://thedogapi.com/) | Animals | Dog pictures & facts | `apiKey` |

---

## 🛠 Usage Examples

### Python

```python
import requests
import json

# Load the full API catalog
with open('apis.json') as f:
    catalog = json.load(f)

# Get all weather APIs
weather_apis = catalog['categories']['Weather']
for api in weather_apis:
    print(f"{api['name']}: {api['url']}")

# Fetch random cat fact
response = requests.get('https://catfact.ninja/fact')
print(response.json()['fact'])
```

### JavaScript

```javascript
// Fetch a random joke
fetch('https://v2.jokeapi.dev/joke/Programming')
  .then(res => res.json())
  .then(data => console.log(data.joke || `${data.setup} ... ${data.delivery}`));

// Load API catalog
fetch('https://raw.githubusercontent.com/AIPMAndy/FreeAPI/main/apis.json')
  .then(res => res.json())
  .then(catalog => {
    console.log(`Total APIs: ${catalog.total}`);
    console.log(`Categories: ${Object.keys(catalog.categories).length}`);
  });
```

### cURL

```bash
# Random dog picture
curl https://dog.ceo/api/breeds/image/random

# Get Bitcoin price
curl https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd

# Random activity suggestion
curl https://www.boredapi.com/api/activity
```

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Quick way to contribute:**
1. Fork this repo
2. Add your API to `apis.json` under the appropriate category
3. Submit a Pull Request

---

## 📜 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgments

- Initial data sourced from [public-apis/public-apis](https://github.com/public-apis/public-apis) (433k+ ⭐)
- Built and maintained by [AIPMAndy](https://github.com/AIPMAndy)

---

<p align="center">
  <strong>⭐ Star this repo if you find it useful!</strong>
</p>
