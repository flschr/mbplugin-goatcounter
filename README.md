# Privacy-optimized web analytics with GoatCounter for Micro.blog

<img src="logo.png" alt="GoatCounter for Micro.blog - Privacy-optimized">

This plugin adds privacy-friendly, lightweight analytics to your Micro.blog site using [GoatCounter](https://www.goatcounter.com). It includes the official GoatCounter JavaScript **locally** in the plugin, ensuring **zero external requests** to third-party servers. You can choose between full JavaScript tracking or a simple tracking pixel for maximum privacy. You need to have a free GoatCounter account to use this plugin.

## Features

- **Self-hosted JavaScript**: Official GoatCounter JS is included in the plugin (no external CDN requests)
- **Flexible tracking modes**: Choose between full JS tracking or tracking pixel-only
- **Tracking pixel fallback**: Works even when JavaScript is disabled
- **Full analytics data**: With JS enabled, you get browser, OS, location, screen size, and more
- **Fully GDPR-friendly**: No cookies, no third-party tracking, no fingerprinting

## How It Works
1. **With JavaScript enabled**: The locally hosted GoatCounter JS collects comprehensive analytics (browser, OS, referrer, screen size, location) and sends it to your GoatCounter instance.
2. **With JavaScript disabled** (or if you disable it in settings): A simple tracking pixel (`<img>`) tracks page views with path and title only.
3. **Complete privacy**: All JavaScript is served from your own domain - no external requests to GoatCounter CDN or other third parties.

## Setup
1. Register and setup your free [GoatCounter](https://www.goatcounter.com) account.
2. Create a free [GoatCounter vanity URL](https://www.goatcounter.com/help/faq#custom-domain).
3. Go to the Micro.blog plugin directory and install the plugin from there.
4. Go to the plugin settings and enter your tracking domain, e.g. `https://name.goatcounter.com` or `https://stats.example.com`. Ensure you enter the full URL including `https://` and without `/count`.
5. **Choose your tracking mode**:
   - **Enable JavaScript tracking** for full analytics (browser, OS, location, screen size, referrer, etc.) - all served locally from your domain
   - **Disable JavaScript tracking** for pixel-only mode (tracks only page path and title)
6. **Add the tracking code to your theme**:
   - Go to Design → Edit Custom Themes
   - Add `{{ partial "goatcounter.html" . }}` to one of these footer files (before `</body>`):
     - **Custom Footer** (in the Micro.blog design editor)
     - `layouts/partials/footer.html`
     - `layouts/partials/custom_footer.html`
   - Save and publish your changes

## What You Get

**With JavaScript enabled** (recommended):
- Full analytics suite from the official GoatCounter JS
- Browser types (Chrome, Firefox, Safari, etc.)
- Operating systems (Windows, macOS, Linux, iOS, Android)
- Screen sizes and device types
- Countries and languages
- Referrers (where visitors came from)
- Page paths and titles
- User sessions tracking

**With JavaScript disabled** (pixel-only mode):
- Page paths
- Page titles
- Basic pageview counting
- No browser/OS/location data

## Privacy & Technical Notes

- **No external requests**: The GoatCounter JavaScript is bundled with the plugin and served from your own Micro.blog domain
- **No cookies**: GoatCounter doesn't use cookies for tracking
- **No fingerprinting**: Privacy-focused analytics without invasive techniques
- **Open source**: Both GoatCounter and this plugin are open source (ISC License)
- **GDPR-friendly**: Fully compliant with European privacy regulations


## 👤 Author
René Fischer – [https://fischr.org](https://fischr.org)
