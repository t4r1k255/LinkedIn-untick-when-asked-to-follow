NOT TO BE CONTINUED! Tüm linkedin script projelerimi https://github.com/t4r1k255/LinkedIn-Guvenli-Toolkit-Reklam-Filtreleri-Easy-Apply adresindeki repo'da topladım. hepsini tek yerden kullanıma sunuyorum.

# DontFollow for LinkedIn

Automatically unticks the "Follow company for more updates" checkbox in LinkedIn's Easy Apply job application modal.

## 🎯 What It Does

When applying for jobs on LinkedIn using Easy Apply, you're often presented with a pre-checked checkbox to follow the company. This userscript automatically unchecks that box for you, saving you an extra click on every application.

## 📦 Installation

### Prerequisites
- A userscript manager extension:
  - [Tampermonkey](https://www.tampermonkey.net/) (Chrome, Firefox, Safari, Edge)
  - [Violentmonkey](https://violentmonkey.github.io/) (Chrome, Firefox, Edge)
  - [Greasemonkey](https://www.greasespot.net/) (Firefox)

### Steps
1. Install one of the userscript managers above
2. Click on the raw userscript file: [`dontfollow-linkedin.user.js`](./dontfollow-linkedin.user.js)
3. Your userscript manager should prompt you to install it
4. Click "Install"
5. Navigate to [LinkedIn Jobs](https://www.linkedin.com/jobs/) and start applying!

## 🚀 How It Works

The script:
- Monitors the page for LinkedIn's Easy Apply modals
- Detects when the "Follow company" checkbox appears
- Automatically unchecks it if it's pre-checked
- Uses multiple fallback methods to ensure it works reliably
- Includes debouncing to prevent excessive checking

## ✨ Features

- **Automatic**: Works silently in the background
- **Non-intrusive**: Only runs on LinkedIn job pages
- **Reliable**: Multiple detection methods with fallbacks
- **Efficient**: Debounced to avoid performance issues
- **Debug-friendly**: Console logging for troubleshooting

## 🛠️ Technical Details

- Watches for DOM mutations using `MutationObserver`
- Targets checkbox by ID: `follow-company-checkbox`
- Triggers multiple events (change, click) for compatibility
- Includes retry logic with progressive delays (300ms, 600ms, 1000ms)

## ⚠️ Disclaimer

This script is provided as-is for educational purposes. Use at your own discretion. LinkedIn's interface may change over time, which could affect functionality.

## 📝 License

MIT License - feel free to modify and distribute!

## 👏 Credits

- Original Author: t4r1k255

## 🤝 Contributing

Issues and pull requests are welcome! If LinkedIn changes their interface and breaks the script, please open an issue.

**Star ⭐ this repo if it saves you time!**
