# 🕸️ Puppeteer Scraper + Flask Server

A multi-stage Docker application that scrapes a webpage using Puppeteer (Node.js) and serves the result via Flask (Python).

---

## 🚀 Features

- Uses **Node.js** and **Chromium** to scrape web pages.
- Uses **Python Flask** to serve the data.
- Multi-stage **Dockerfile** for a lean image.
- Easy to configure with environment variables.

---

## 🛠️ Build Instructions

```bash
docker build --build-arg SCRAPE_URL="https://example.com" -t puppeteer-flask-app .
```

## ▶️ Run Instructions

```bash
docker run -p 5000:5000 puppeteer-flask-app
```

## 🌐 Access the Scraped Content
Visit: http://localhost:5000


## ✅ How It Works
1. You provide a URL (via an environment variable at build time).

2. Node.js with Puppeteer:
 
Launches a headless Chromium browser.

Navigates to the given URL.

Extracts:

The <title> of the page.

The first <h1> element (if available).

Saves this info to scraped_data.json.

Python Flask App:

Reads that JSON file.

Serves it at http://localhost:5000/ as JSON over HTTP.

Docker Multi-Stage Build:

Keeps final image minimal by excluding Chromium/Puppeteer from the runtime.
