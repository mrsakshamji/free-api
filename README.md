
# 📰 Hindu News API

A lightweight API that delivers real-time news headlines from The Hindu, updated every 15 minutes via GitHub Actions.

---

## 🔗 Production URL

```
https://hindu-news-vz9h8s4is-sakshams-projects-f7a121ff.vercel.app/api/news
```

---

## 🔐 Authentication

All API requests must include a valid API key in the request headers.

### ✅ Required Header

```
x-api-key: saksham-api-news-11-04-2005-protected-paid
```

---

## 📦 Response Format

```json
[
  {
    "title": "Sample News Headline",
    "link": "https://example.com/news-article",
    "published": "Mon, 14 Jul 2025 23:12:32 +0530",
    "author": ""
  }
]
```

---

## 🔄 Update Frequency

- 🕒 **Every 5 minutes**
- 🔄 Automated by **GitHub Actions**
- 📁 Source JSON: [hindu-main-news.json](https://mrsakshamji.github.io/hindu-news-scraper/hindu-main-news.json)

---

## ⚠️ Error Responses

| Status | Message      | Reason                        |
|--------|--------------|-------------------------------|
| 200    | OK           | Request succeeded              |
| 401    | Unauthorized | Invalid or missing API key     |
| 500    | Server Error | News source unreachable        |

---

## 🧪 Example Usage

### curl

```bash
curl -H "x-api-key: saksham-api-news-11-04-2005-protected-paid" \
https://hindu-news-vz9h8s4is-sakshams-projects-f7a121ff.vercel.app/api/news
```

### JavaScript (Fetch)

```js
fetch("https://hindu-news-vz9h8s4is-sakshams-projects-f7a121ff.vercel.app/api/news", {
  headers: {
    "x-api-key": "saksham-api-news-11-04-2005-protected-paid"
  }
})
.then(res => res.json())
.then(data => console.log(data));
```

---

## 🧪 Postman Setup

- Method: `GET`
- URL: `https://hindu-news-vz9h8s4is-sakshams-projects-f7a121ff.vercel.app/api/news`
- Headers:
  ```
  Key: x-api-key
  Value: saksham-api-news-11-04-2005-protected-paid
  ```

---

## 🛠 Tech Stack

- 🐍 **Node.js (API handler)**
- ⚡ **Vercel Hosting**
- 📂 **GitHub Pages** for public JSON
- 🤖 **GitHub Actions** for automated scraping

---

## 📜 License

This project is for educational and personal use only.  
Please contact for commercial or high-volume access.

---

> Built with ❤️ by [@mrsakshamji](https://github.com/mrsakshamji)
