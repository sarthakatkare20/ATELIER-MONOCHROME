# ATELIER MONOCHROME — Digital Flagship (Under Development)

A minimalist luxury "Under Development / Coming Soon" landing page for **ATELIER MONOCHROME** (Haute Menswear & Tailoring).

---

## ✨ Features

- **Luxury Monochrome Aesthetic:** Clean editorial design with Bodoni / Cormorant Garamond serif typography and Plus Jakarta Sans.
- **Connected Inline Email Capture:** Seamless rectangular email signup bar (`Enter your email` + `NOTIFY ME →`) integrated with Web3Forms.
- **Web3Forms Direct Email Delivery:** Automatic real-time notification to your inbox when a user subscribes to the waitlist (no backend server required).
- **Enlarged 45-Day Countdown Timer:** Centered floating glass pill capsule counting down real-time to the SS26 launch.
- **Dark Mode Autofill Override:** Prevents browser's default light-blue autofill background, keeping the dark luxury theme intact.
- **Pixel-Perfect Brand Navigation & Footer:** Top luxury navbar and bottom social links (`Instagram`, `Facebook`, `Pinterest`, `YouTube`).
- **100% Responsive:** Optimized for Mobile, Tablet, and Ultra-wide Desktop displays.

---

## 📁 File Structure

```text
ATELIER MONOCHROME/
├── assets/
│   └── hero_editorial.jpg     # High-resolution monochrome fashion editorial background
├── index.html                 # Main landing page (HTML5, CSS3, Vanilla JS)
└── README.md                  # Project documentation
```

---

## 🚀 How to Run Locally

1. Simply double-click `index.html` to open it in any web browser.
2. Or use any static file server:
   ```bash
   # Using VS Code Live Server extension or Python
   python -m http.server 3000
   ```
3. Open `http://localhost:3000` in your browser.

---

## ⚙️ Configuration & Customization

### 1. Web3Forms Email Notifications
The form is currently connected with your Web3Forms Access Key:
```javascript
const WEB3FORMS_KEY = "bb2c8b05-79b2-4f07-8570-9776029ae524";
```
To change the recipient inbox, generate a new free key at [web3forms.com](https://web3forms.com) and replace the key in `index.html`.

### 2. Adjusting Countdown Days
By default, the timer counts down **45 days** from first visit. To change the duration, modify the days multiplier in `index.html`:
```javascript
targetTimestamp = new Date().getTime() + (45 * 24 * 60 * 60 * 1000); // Change 45 to any number of days
```

### 3. Updating Social Media Links
Find the `.social-cluster` section in `index.html` and update the `href` attributes:
```html
<a href="https://instagram.com/yourhandle" class="social-icon-link" title="Instagram">...</a>
```

---

## 🌐 Deployment

This is a standalone static site. You can deploy it for free on:
- **Vercel / Netlify:** Drag and drop the folder.
- **GitHub Pages:** Push to repository and enable GitHub Pages in Settings.
- **Custom Domain / CPanel:** Upload `index.html` and the `assets/` folder to `public_html`.

---

&copy; ATELIER MONOCHROME. All Rights Reserved.
