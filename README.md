# Link Generator

**Link Generator** is a high-performance web utility and **Progressive Web App (PWA)** custom-built for **St Pauls Multimedia**. It streamlines the creation of daily service announcements by integrating with the YouTube Data API to fetch live stream links and formatting them perfectly for WhatsApp.



---

## 🌟 Key Features

* **YouTube API Integration:** Fetch live or upcoming stream links instantly using a Channel ID.
* **One-Click Formatting:** Automatically generates WhatsApp-ready text with bold headers (`*SERVICE*`) and details (`*Led by*`, `*Theme*`).
* **Security & Privacy:**
    * **Masked Inputs:** API Keys and Channel IDs are treated as password fields.
    * **Anti-Copy/Cut:** Sensitive fields are protected to prevent credential theft.
    * **Local Storage:** Configuration data is stored only in the user's browser, never on a server.
* **Progressive Web App (PWA):**
    * **Offline Access:** Works without internet after the first load via **Service Worker (`sw.js`)**.
    * **Mobile Install:** Can be added to the home screen as a standalone app.
* **Custom Presets:** Save recurring service schedules (times and theme settings) for different events.

---

## 🛡️ Security: Preventing API Leaks

> [!IMPORTANT]
> **DO NOT** paste your API Key or Channel ID directly into the code (`index.html`) before uploading to a public repository. GitHub's security scanners will flag this as a leak.

**The Secure Setup Process:**
1. Upload the code with empty values for `DEFAULT_API_KEY` and `DEFAULT_CHANNEL_ID`.
2. Open your live **GitHub Pages URL**.
3. Click the **⚙ Gear Icon**.
4. Enter your **API Key** and **Channel ID**.
5. Check the **"Lock API & Channel ID"** box. This ensures that even if a team member clears the service presets, the connection to YouTube remains intact.

---

## 🚀 Getting Started

### 1. File Structure
For the PWA to function, ensure your repository contains these 4 files in the root folder:
* `index.html` — Main application logic and UI
* `sw.js` — Service Worker for offline support
* `manifest.json` — PWA configuration for mobile

### 2. Deployment (GitHub Pages)
1. Go to your Repository **Settings** > **Pages**.
2. Under **Build and deployment**, select `Deploy from a branch`.
3. Choose the `main` branch and `/root` folder, then click **Save**.
4. Wait a few minutes for GitHub to provide your live **HTTPS** link.



---

## 🛠️ Tech Stack

* **HTML5 / CSS3:** Custom luxury theme (Gold & Matte Black).
* **Vanilla JavaScript:** Lightweight logic with no external dependencies.
* **YouTube Data API v3:** Real-time stream fetching.
* **Google Fonts:** Cinzel (Headers) and Segoe UI (Body).

---

## 📱 Mobile Installation

Access the site via **HTTPS** on your mobile device to enable installation.

### **On Android (Chrome)**
* Open your live URL.
* Tap the **three-dot menu** and select **Install App** or **Add to Home Screen**.

### **On iOS (Safari)**
* Open your live URL.
* Tap the **Share** icon (square with an arrow).
* Scroll down and select **"Add to Home Screen."**

---

## 📄 License
This project is proprietary and intended for the internal use of **St Pauls Multimedia**.
