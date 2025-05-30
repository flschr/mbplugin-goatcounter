# Privacy optimized web analytics with GoatCounter for Micro.blog

This plugin adds privacy-friendly, lightweight analytics to your Micro.blog site using [GoatCounter](https://www.goatcounter.com). It uses a tracking pixel and optionally includes inline JavaScript to enhance the tracking with HTTP referrer data, without relying on cookies or any third-party scripts.

## ✅ Features

- Static tracking pixel (`<img>`) with page path and title
- Optional inline JavaScript to include the HTTP referrer
- Works with [GoatCounter vanity URLs](https://www.goatcounter.com/help/faq#custom-domain)
- Fully GDPR-friendly: No cookies, no third-party tracking, no fingerprinting

## 🛠 How It Works

1. A tracking request is sent to your GoatCounter domain with the current page path and title.
2. If JavaScript tracking is enabled and the visitor came from an external site, the referrer is added.
3. If JavaScript is disabled or blocked, a `<noscript>` fallback ensures basic page view tracking still works.

## ⚙️ Plugin Settings

This plugin provides two configuration options in Micro.blog:
- GoatCounter Domain: Your tracking domain, e.g. `https://name.goatcounter.com/` or `https://stats.example.com` (without `/count`)
- Enable inline JavaScript: Enable or disable inline JavaScript for sending the referrer

> 🦊 **Vanity URLs** (e.g. `https://yourdomain.com/count`) are fully supported, just enter the full base URL.

## 📦 Installation
Go to the Micro.blog plugin directory and install the plugin from there.

## 👤 Author
René Fischer – [https://fischr.org](https://fischr.org)
