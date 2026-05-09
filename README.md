<div align="center">

# 🚀 FreeAPI

### **The Ultimate Collection of Free Public APIs**

**1,000+ APIs · 51 Categories · JSON + Markdown · Always Free**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)
[![APIs](https://img.shields.io/badge/APIs-1092-blue.svg?style=for-the-badge)](apis.json)
[![Categories](https://img.shields.io/badge/Categories-51-green.svg?style=for-the-badge)](#-categories)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen.svg?style=for-the-badge)](CONTRIBUTING.md)

<br />

**Stop wasting hours searching for APIs.**

FreeAPI is a developer-first, community-curated collection of free public APIs.
Structured data you can actually use — not just a giant README nobody reads.

[Quick Start](#-quick-start) · [Browse APIs](#-categories) · [JSON Download](#-json-download) · [Contribute](#-contributing)

<br />

</div>

---

## ⚡ Quick Start

**3 steps. 30 seconds.**

```bash
# 1. Download the API catalog
curl -O https://raw.githubusercontent.com/AIPMAndy/FreeAPI/main/apis.json

# 2. Pick a category
cat apis.json | python3 -c "import sys,json; d=json.load(sys.stdin); [print(f'{k}: {len(v)} APIs') for k,v in d['categories'].items()]"

# 3. Start building
curl https://catfact.ninja/fact
```

That's it. You now have access to 1,092 free APIs.

---

## 🎯 Why FreeAPI?

| Problem | FreeAPI Solution |
|:---|:---|
| 🔍 APIs scattered across 100s of sites | ✅ One structured JSON file |
| 📖 Giant README nobody can search | ✅ Machine-readable + per-category files |
| 💀 Dead APIs everywhere | ✅ Community-maintained, PRs fix broken links |
| 🔐 "Free" APIs that aren't really free | ✅ Only APIs with genuine free tiers |

---

## 📦 JSON Download

The real power of FreeAPI is the **structured JSON** — use it in your apps, scripts, or tools.

```bash
curl -O https://raw.githubusercontent.com/AIPMAndy/FreeAPI/main/apis.json
```

<details>
<summary><strong>📋 JSON Schema</strong></summary>

```json
{
  "total": 1092,
  "categories": {
    "Category Name": [
      {
        "name": "API Name",
        "url": "https://docs-url.com",
        "description": "What it does",
        "auth": "No | apiKey | OAuth | token",
        "https": "Yes | No",
        "cors": "Yes | No | Unknown"
      }
    ]
  }
}
```

Each field:
- **`auth`** — `No` (free, no key), `apiKey` (free key required), `OAuth`, or `token`
- **`https`** — Whether the API supports HTTPS
- **`cors`** — Whether CORS is enabled (important for browser apps)

</details>

---

## 🗂 Categories

<table>
<tr>
<td width="50%">

| Emoji | Category | Count |
|:---|:---|:---|
| 🐾 | [Animals](categories/animals.md) | 26 |
| 🎌 | [Anime](categories/anime.md) | 16 |
| 🛡️ | [Anti-Malware](categories/anti-malware.md) | 13 |
| 🎨 | [Art & Design](categories/art-design.md) | 20 |
| 🔐 | [Auth & Authorization](categories/authentication-authorization.md) | 6 |
| ⛓️ | [Blockchain](categories/blockchain.md) | 7 |
| 📚 | [Books](categories/books.md) | 15 |
| 💼 | [Business](categories/business.md) | 20 |
| 📅 | [Calendar](categories/calendar.md) | 13 |
| ☁️ | [Cloud Storage](categories/cloud-storage-file-sharing.md) | 17 |
| 🔄 | [Continuous Integration](categories/continuous-integration.md) | 6 |
| 🪙 | [Cryptocurrency](categories/cryptocurrency.md) | 51 |
| 💱 | [Currency Exchange](categories/currency-exchange.md) | 12 |
| ✅ | [Data Validation](categories/data-validation.md) | 7 |
| 👨‍💻 | [Development](categories/development.md) | 72 |
| 📖 | [Dictionaries](categories/dictionaries.md) | 13 |
| 📝 | [Documents & Productivity](categories/documents-productivity.md) | 21 |
| 📧 | [Email](categories/email.md) | 14 |
| 🎮 | [Entertainment](categories/entertainment.md) | 6 |
| 🌍 | [Environment](categories/environment.md) | 12 |
| 🎉 | [Events](categories/events.md) | 3 |
| 💰 | [Finance](categories/finance.md) | 29 |

</td>
<td width="50%">

| Emoji | Category | Count |
|:---|:---|:---|
| 🍔 | [Food & Drink](categories/food-drink.md) | 21 |
| 🎲 | [Games & Comics](categories/games-comics.md) | 65 |
| 📍 | [Geocoding](categories/geocoding.md) | 58 |
| 🏛️ | [Government](categories/government.md) | 84 |
| ❤️ | [Health](categories/health.md) | 23 |
| 💼 | [Jobs](categories/jobs.md) | 14 |
| 🤖 | [Machine Learning](categories/machine-learning.md) | 13 |
| 🎵 | [Music](categories/music.md) | 23 |
| 📰 | [News](categories/news.md) | 15 |
| 📊 | [Open Data](categories/open-data.md) | 33 |
| 🔓 | [Open Source Projects](categories/open-source-projects.md) | 9 |
| 📋 | [Patent](categories/patent.md) | 2 |
| 🧠 | [Personality](categories/personality.md) | 16 |
| 📱 | [Phone](categories/phone.md) | 4 |
| 📷 | [Photography](categories/photography.md) | 27 |
| 💻 | [Programming](categories/programming.md) | 5 |
| 🔬 | [Science & Math](categories/science-math.md) | 31 |
| 🔒 | [Security](categories/security.md) | 29 |
| 🛍️ | [Shopping](categories/shopping.md) | 10 |
| 👥 | [Social](categories/social.md) | 33 |
| ⚽ | [Sports & Fitness](categories/sports-fitness.md) | 27 |
| 🧪 | [Test Data](categories/test-data.md) | 21 |
| 📝 | [Text Analysis](categories/text-analysis.md) | 12 |
| 📌 | [Tracking](categories/tracking.md) | 5 |
| 🚗 | [Transportation](categories/transportation.md) | 41 |
| 🔗 | [URL Shorteners](categories/url-shorteners.md) | 16 |
| 🚘 | [Vehicle](categories/vehicle.md) | 6 |
| 🎬 | [Video](categories/video.md) | 25 |
| 🌤️ | [Weather](categories/weather.md) | 25 |

</td>
</tr>
</table>

---

## ⭐ Top 10 APIs to Start With

| API | What It Does | Auth | Try It |
|:---|:---|:---|:---|
| 🐱 [The Cat API](https://thecatapi.com/) | Random cat images | `apiKey` | `curl https://api.thecatapi.com/v1/images/search` |
| 🐕 [Dog CEO](https://dog.ceo/dog-api/) | Random dog images | None | `curl https://dog.ceo/api/breeds/image/random` |
| 😂 [JokeAPI](https://jokeapi.dev/) | Programming jokes | None | `curl https://v2.jokeapi.dev/joke/Programming` |
| 🌦️ [wttr.in](https://wttr.in) | Weather in terminal | None | `curl wttr.in/Shanghai` |
| 🪙 [CoinGecko](https://www.coingecko.com/api) | Crypto prices | None | `curl https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd` |
| 🌍 [REST Countries](https://restcountries.com/) | Country data | None | `curl https://restcountries.com/v3.1/name/china` |
| 🎲 [Bored API](https://www.boredapi.com/) | Random activities | None | `curl https://www.boredapi.com/api/activity` |
| 🚀 [NASA](https://api.nasa.gov/) | Space imagery & data | `apiKey` | [Get free key](https://api.nasa.gov/) |
| 📰 [NewsAPI](https://newsapi.org/) | Live news | `apiKey` | [Get free key](https://newsapi.org/register) |
| 🐾 [PokeAPI](https://pokeapi.co/) | Pokémon data | None | `curl https://pokeapi.co/api/v2/pokemon/pikachu` |

---

## 💻 Code Examples

### Python — Browse APIs Programmatically

```python
import json, requests

# Load the catalog
with open('apis.json') as f:
    catalog = json.load(f)

# List all Weather APIs
for api in catalog['categories']['Weather']:
    print(f"  {api['name']:25} {api['auth']:10} {api['url']}")

# Find all APIs that need NO authentication
no_auth = [
    api for apis in catalog['categories'].values() 
    for api in apis if api['auth'] == 'No'
]
print(f"\n{len(no_auth)} APIs need no authentication — just call them!")
```

### JavaScript — Fetch & Use

```javascript
// Get a random programming joke
const res = await fetch('https://v2.jokeapi.dev/joke/Programming');
const data = await res.json();
console.log(data.joke || `${data.setup} ... ${data.delivery}`);

// Load the catalog and find all crypto APIs
const catalog = await fetch(
  'https://raw.githubusercontent.com/AIPMAndy/FreeAPI/main/apis.json'
).then(r => r.json());

console.log(`Crypto APIs: ${catalog.categories.Cryptocurrency.length}`);
```

### cURL — Instant Gratification

```bash
# Random cat fact
curl https://catfact.ninja/fact

# Bitcoin price in USD
curl https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd

# Random activity if you're bored
curl https://www.boredapi.com/api/activity

# Weather for any city (terminal-friendly)
curl wttr.in/Tokyo?format=3
```

---

## 🔧 Use Cases

- **🎨 Side Projects** — Find APIs for your next hackathon project
- **📚 Learning** — Practice API integration with real endpoints
- **🤖 AI/ML** — Feed structured API data to your LLM agents
- **📱 App Development** — Discover data sources for your app
- **📊 Data Science** — Access free data endpoints for analysis

---

## 🤝 Contributing

Found a great free API? Spotted a broken link? **We want your PR!**

```bash
# Quick contribution
1. Fork → 2. Edit apis.json → 3. Submit PR
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines.

**What makes a good API entry:**
- ✅ Has a free tier (not just a free trial)
- ✅ Has documentation
- ✅ Is currently working
- ❌ No paid-only APIs
- ❌ No dead/deprecated APIs

---

## 📜 License

[MIT](LICENSE) — Use it however you want.

---

## 🙏 Acknowledgments

- Initial data from [public-apis/public-apis](https://github.com/public-apis/public-apis) — the OG (433k+ ⭐)
- Built by [AIPMAndy](https://github.com/AIPMAndy)

---

<div align="center">

**⭐ Star this repo if it saved you time!**

*The more stars, the more APIs we'll add.*

[![Star History Chart](https://api.star-history.com/svg?repos=AIPMAndy/FreeAPI&type=Date)](https://star-history.com/#AIPMAndy/FreeAPI&Date)

</div>
