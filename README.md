# 📊 GoatCounter Privacy-optimized Web Analytics for Micro.blog

This plugin adds privacy-friendly, lightweight analytics to your Micro.blog site using [GoatCounter](https://www.goatcounter.com). It uses a static tracking pixel with optional JavaScript to include the HTTP referrer — no cookies, no external JavaScript required.

## ✅ Features

- Static tracking pixel (`<img>`) with page path and title
- Optional JavaScript-enhanced tracking with the HTTP referrer
- Works with [GoatCounter vanity URLs](https://www.goatcounter.com/help/faq#custom-domain)
- Fully GDPR-friendly: No cookies, no profiling, no external scripts

## 🛠 How It Works
1. The plugin injects a `<script>` block that sends a tracking request to your GoatCounter domain including:
   - The page path
   - The page title
   - The referrer (only if it’s external)
2. For users without JavaScript, a fallback `<noscript>` pixel tracks page views with path and title only.

## ⚙️ Configuration
Specify your **GoatCounter tracking domain** in the configuration, (e.g. `https://name.goatcounter.com/`).

> 🦊 **Vanity URLs** (e.g. `https://name.goatcounter.com/`) are fully supported — just enter your full base URL **without** `/count` in the plugin settings.

## 📦 Installation
Go to the Micro.blog plugin directory and install the plugin from there.


## 👤 Author
René Fischer – [https://fischr.org](https://fischr.org)
