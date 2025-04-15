# Wanderlust - Your Ultimate Travel Blog 🌍✈️

WanderLust is a simple MERN travel blog website ✈ This project is aimed to help people to contribute in open source, upskill in react and also master git.

![Preview Image](https://github.com/krishnaacharyaa/wanderlust/assets/116620586/17ba9da6-225f-481d-87c0-5d5a010a9538)
#
### In this demo, we will see how to deploy an end to end three tier MERN stack application on EKS cluster.
#
### <mark>Project Architecture</mark>
<img src="https://github.com/DevMadhup/Wanderlust-Mega-Project/blob/main/Assets/DevSecOps%2BGitOps.gif" />

Pros:
     

#
![download](https://github.com/user-attachments/assets/deec9867-64aa-4ee5-a05b-7c93860b6773)

### 1.1 EKS vs. Self-Managed Kubernetes: Pros and Cons

1.1.1 EKS (Amazon Elastic Kubernetes Service)
Pros:
    
     Managed nodes

### 1.2 EKS vs. Self-Managed kubernetes: Pros and Cons




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
