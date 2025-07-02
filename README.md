# Totally Free APIs

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A curated collection of completely free APIs requiring no authentication. I find many of these APIs are interesting and useful for side projects, so I'm collecting them here.

## 🎯 Project Goal

This project focuses exclusively on APIs that are:
- ✅ **Completely Free** - No hidden costs or premium tiers
- ✅ **No Authentication Required** - No API keys, tokens, or registration needed
- ✅ **Stable & Reliable** - Production-ready services (no test/demo APIs)
- ✅ **Well-Documented** - Clear usage instructions and examples

## 📋 API Categories

### 🎲 Random Data
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| Random User | Generate random user data | ✅ | [Go!](https://randomuser.me/) |
| JSONPlaceholder | Fake JSON data for testing | ✅ | [Go!](https://jsonplaceholder.typicode.com/) |
| Lorem Picsum | Random placeholder images | ✅ | [Go!](https://picsum.photos/) |
| Random Quote | Inspirational quotes | ✅ | [Go!](https://api.quotable.io/) |

### 🔢 Utilities
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| QR Server | Generate QR codes | ✅ | [Go!](https://goqr.me/api/) |
| HTTP Status Codes | HTTP status code information | ✅ | [Go!](https://httpstat.us/) |
| UUID Generator | Generate UUIDs | ✅ | [Go!](https://www.uuidgenerator.net/api) |

### 🎨 Images & Media
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| Unsplash Source | Random high-quality photos | ✅ | [Go!](https://unsplash.com/) |
| Placeholder.com | Placeholder images | ✅ | [Go!](https://placeholder.co/) |
| Robohash | Generate robot/monster avatars | ✅ | [Go!](https://robohash.org/) |

### 📊 Data & Information
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| Numbers API | Facts about numbers | ✅ | [Go!](http://numbersapi.com/) |
| Cat Facts | Random cat facts | ✅ | [Go!](https://catfact.ninja/) |

### 🌍 Geography & Location
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| REST Countries | Get information about countries | ✅ | [Go!](https://restcountries.com/) |
| IP Geolocation | Get geolocation data from IP address | ✅ | [Go!](http://ip-api.com/) |
| Zippopotam.us | Postal and zip code data | ✅ | [Go!](http://www.zippopotam.us/) |

### 🌤️ Weather
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| Open-Meteo | Weather forecasts | ✅ | [Go!](https://open-meteo.com/) |

### 💰 Cryptocurrency
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| BitcoinCharts | Bitcoin market data and charts | ✅ | [Go!](https://bitcoincharts.com/about/markets-api/) |
| CoinCap | Real-time crypto pricing for 1000+ coins | ✅ | [Go!](https://docs.coincap.io/) |
| CoinGecko | Crypto prices, market data, and charts | ✅ | [Go!](https://www.coingecko.com/en/api) |
| Coinpaprika | Crypto prices and market research | ✅ | [Go!](https://api.coinpaprika.com/) |
| CryptoCompare | Crypto prices and historical data | ✅ | [Go!](https://min-api.cryptocompare.com/) |
| Cryptonator | Simple crypto prices and conversion | ✅ | [Go!](https://www.cryptonator.com/api/) |
| Mempool | Bitcoin mempool and blockchain data | ✅ | [Go!](https://mempool.space/docs/api/rest) |
| Mercado Bitcoin | Brazilian crypto exchange data | ✅ | [Go!](https://www.mercadobitcoin.com.br/api-doc/) |
| Messari | Crypto research, data, and news | ✅ | [Go!](https://messari.io/api) |

### 🏛️ Government & Open Data
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| Census.gov | US Census Bureau demographic data | ✅ | [Go!](https://www.census.gov/data/developers/data-sets.html) |
| Colorado Open Data | Colorado State Government data | ✅ | [Go!](https://data.colorado.gov/) |
| USAspending.gov | US federal spending data | ✅ | [Go!](https://api.usaspending.gov/) |
| Chronicling America | US newspaper archives 1777-1963 | ✅ | [Go!](http://chroniclingamerica.loc.gov/about/api/) |
| Open Library | Book information and library services | ✅ | [Go!](https://openlibrary.org/developers/api) |
| World Bank | Global development data | ✅ | [Go!](https://datahelpdesk.worldbank.org/knowledgebase/topics/125589) |

### 🌐 Internet & Tech
| API | Description | HTTPS | Link |
|-----|-------------|-------|------|
| HTTP Bin | HTTP request testing | ✅ | [Go!](https://httpbin.org/) |

## 📖 Usage Examples

### JavaScript/Fetch
```javascript
// Get a random user
fetch('https://randomuser.me/api/')
  .then(response => response.json())
  .then(data => console.log(data));

// Get country information
fetch('https://restcountries.com/v3.1/name/china')
  .then(response => response.json())
  .then(data => console.log(data));

// Get US Census data
fetch('https://api.census.gov/data/2019/acs/acs1?get=NAME&for=state:*')
  .then(response => response.json())
  .then(data => console.log(data));

// Get Bitcoin price
fetch('https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd')
  .then(response => response.json())
  .then(data => console.log(`Bitcoin: $${data.bitcoin.usd}`));
```

### Python/Requests
```python
import requests

# Get weather data
response = requests.get('https://api.open-meteo.com/v1/forecast?latitude=52.52&longitude=13.41&current_weather=true')
data = response.json()
print(data)

# Get a cat fact
response = requests.get('https://catfact.ninja/fact')
fact = response.json()
print(fact['fact'])

# Get World Bank country data
response = requests.get('https://api.worldbank.org/v2/countries?format=json')
countries = response.json()
print(countries)

# Get top cryptocurrencies
response = requests.get('https://api.coincap.io/v2/assets?limit=5')
crypto_data = response.json()
for asset in crypto_data['data']:
    print(f"{asset['name']}: ${float(asset['priceUsd']):.2f}")
```

### cURL
```bash
# Generate a QR code
curl "https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=Hello%20World"

# Get IP location
curl "http://ip-api.com/json/"

# Get US federal spending data
curl "https://api.usaspending.gov/api/v2/disaster/overview/"

# Get Bitcoin market data
curl "https://api.cryptonator.com/api/ticker/btc-usd"
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Quick Contribution Steps:
1. Fork this repository
2. Add your API to the appropriate category in README.md
3. Ensure the API meets our criteria (free, no auth, stable)
4. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⭐ Star History

If this project helps you, please consider giving it a star!

---

**Made with ❤️ for the indie developer community** 