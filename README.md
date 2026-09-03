# 🚀 Eat Token Generator

A modern, high-performance web-based tool to help developers extract **EAT Tokens** and generate **Garena Free Fire access tokens** from authentication callback URLs.

⚠️ **Educational and research purposes only** - Demonstrates how authentication flows work.

---

## 🌐 Live Website

🔗 **[Open Live Website](https://zevricplayx.github.io/eat_token/)**

```
https://zevricplayx.github.io/eat_token/
```

---

## ✨ Features

- 🎨 **Modern Dark UI** - Beautiful neon-gradient design with smooth animations
- ⚡ **Instant Token Extraction** - Automatically parse EAT tokens from URLs
- 🔐 **Multiple Providers** - Google, Facebook, Apple, X (Twitter), VK
- 📋 **One-Click Copy** - Copy full JSON response with single click
- 📱 **Fully Responsive** - Works perfectly on mobile, tablet, and desktop
- 🎯 **Real-time Status** - Get instant feedback on every action
- 💾 **No Data Storage** - All processing happens locally in your browser
- ⚙️ **JSON Output** - Structured token response for easy integration

---

## 📖 How To Use

### Step 1️⃣: Select Provider & Login
Visit the website and choose your preferred login provider:
- Google
- Facebook  
- Apple
- X (Twitter)
- VK

Click the icon and login with your Garena account.

### Step 2️⃣: Complete Authentication
- You'll be redirected to official Garena authentication
- Complete the login process

### Step 3️⃣: Find Your Callback URL
After successful login, look for URLs in your browser history containing:

```
/callback/?eat=
?eat=
api-ticket.ff.gameid.garena.co.id
ticket.kiosgamer.co.id
```

### Step 4️⃣: Example Callback URLs

**Garena Official:**
```
https://api-ticket.ff.gameid.garena.co.id/oauth/callback/?eat={YOUR_EAT_TOKEN}&lang=en&region={region}&account_id={uid}&nickname={name}
```

**Kiosgamer:**
```
https://ticket.kiosgamer.co.id/?eat={YOUR_EAT_TOKEN}&lang=en&region={region}&account_id={uid}&nickname={name}
```

### Step 5️⃣: Generate Access Token
1. Copy the entire callback URL
2. Paste it into the input box on the website
3. Click **GENERATE TOKEN**
4. The tool automatically extracts the EAT token and generates the access token response

### Step 6️⃣: Copy & Use
- Click **COPY FULL RESPONSE**
- Use the JSON response for testing or development
- Integrate into your project

---

## 🎯 Features Explained

### Real-time Extraction
The tool automatically detects and extracts:
- ✅ EAT Token
- ✅ Account ID
- ✅ Region
- ✅ Nickname
- ✅ Language

### JSON Response Format
```json
{
  "access_token": "your_eat_token_here",
  "token_type": "Bearer",
  "expires_in": 3600,
  "account_id": "your_account_id",
  "region": "your_region",
  "nickname": "your_nickname",
  "language": "en",
  "created_at": "2026-09-03T12:36:54Z",
  "platform": "selected_provider"
}
```

---

## 🔧 Technical Details

- **Language**: HTML5 + CSS3 + Vanilla JavaScript
- **Framework**: None (Zero dependencies)
- **Size**: ~22KB (single file)
- **Performance**: Instant processing
- **Security**: All data processed locally, no server uploads
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

---

## 📦 Installation & Setup

### Option 1: GitHub Pages (Recommended)
The repository is already configured for GitHub Pages.

1. Go to your repository settings
2. Under "Pages" → Select "Deploy from a branch"
3. Select "main" branch
4. Your site will be live at: `https://zevricplayx.github.io/eat_token/`

### Option 2: Local Development
```bash
# Clone the repository
git clone https://github.com/zevricplayx/eat_token.git

# Navigate to directory
cd eat_token

# Open in browser
open index.html
# or use a local server:
python -m http.server 8000
```

Then visit: `http://localhost:8000`

---

## 🎨 Customization

### Change Colors
Edit the CSS variables in `index.html`:

```css
:root {
    --primary: #ff006e;      /* Main color */
    --secondary: #8338ec;    /* Secondary color */
    --accent: #3a86ff;       /* Accent color */
    --dark: #0a0e27;         /* Dark background */
}
```

### Add Custom Title
Replace in the `<title>` tag:
```html
<title>Your Custom Title | Eat Token</title>
```

### Modify Social Links
Update footer links:
```html
<a href="YOUR_GITHUB_URL">GitHub</a>
<a href="YOUR_TELEGRAM_URL">Telegram</a>
```

---

## ⚖️ Important Notice

- ⚠️ **Educational Purpose Only** - This tool is for learning authentication flows
- ⚠️ **Terms of Service** - Do not violate Garena Terms & Conditions
- ⚠️ **Responsible Use** - Avoid automated abuse of the system
- ⚠️ **User Risk** - Use at your own risk; developer not responsible for misuse
- ⚠️ **No Token Storage** - The website does NOT store your data
- ✅ **Privacy** - Only local processing, no external uploads

---

## 🔐 Security

- ✅ No backend server
- ✅ No data sent to external servers
- ✅ All processing happens in your browser
- ✅ HTTPS connection (GitHub Pages)
- ✅ No cookies or tracking

---

## 📝 Files Structure

```
eat_token/
├── index.html          # Main application (single file)
├── README.md          # This file
└── LICENSE            # License information
```

---

## 🤝 Contributing

Found a bug or have a suggestion? 
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

---

## 📞 Support & Contact

**Developer**: Killer Sharma (Aditya)

- 🔗 **GitHub**: [github.com/KillerSharmaBot](https://github.com/KillerSharmaBot)
- 📱 **Telegram**: [@KillerSharmaBot](https://t.me/KillerSharmaBot)
- 🎥 **YouTube**: [@KillerSharmaBot](https://youtube.com/@KillerSharmaBot)
- 📸 **Instagram**: [@KillerSharmaBot](https://instagram.com/KillerSharmaBot)

**Improved By**: zevricplayx

---

## 📄 Terms & Conditions

By using this website, you agree to:
- Use for educational purposes only
- Not violate any ToS of third-party services
- Take full responsibility for your actions
- Not hold the developer liable for misuse

The website is provided "AS IS" without any warranty.

---

## 📜 License

This project is open source and available under the MIT License.

---

## 🎉 Changelog

### v2.0 (Current - Improved Version)
- ✨ Complete UI redesign with modern neon aesthetics
- ✨ Smooth animations and transitions
- ✨ Better responsive design
- ✨ Enhanced token extraction logic
- ✨ Improved error handling
- ✨ Status messages and notifications
- ✨ Copy to clipboard functionality
- ✨ Keyboard shortcuts (Ctrl+Enter to generate)

### v1.0 (Original)
- Basic token extraction
- Simple UI
- Core functionality

---

## ⭐ Show Your Support

If you find this tool helpful:
- ⭐ Star this repository
- 🍴 Fork and improve it
- 📢 Share with others
- 💬 Give feedback

---

**Made with ❤️ by Killer Sharma & Improved by zevricplayx**

*Last Updated: September 2026*