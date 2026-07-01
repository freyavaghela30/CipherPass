# 🔐 CipherPass — Password Strength Analyzer

A sleek, client-side password strength analyzer built with pure HTML, CSS, and JavaScript. No frameworks, no backend, no data stored — everything runs in your browser.

🌐 **Live Demo:** [freyavaghela30.github.io/CipherPass](https://freyavaghela30.github.io/CipherPass)

---

## ✨ Features

- 🔍 **Real-time strength analysis** — instant feedback as you type
- 📊 **5-level strength meter** — Very Weak → Very Strong with animated bars
- ✅ **Criteria checklist** — Length, Uppercase, Lowercase, Numbers, Symbols, No repeats
- 💡 **Smart suggestions** — tells you exactly what to improve
- ⚡ **Strong password generator** — cryptographically secure random passwords
- 📋 **One-click copy** — copy generated passwords instantly
- 🔢 **Entropy calculator** — shows bits of entropy and character pool size
- 👁️ **Show/hide toggle** — reveal or mask your password
- 🧠 **Personal info checker** — warns if your password contains your name or birthdate
- 🚫 **Common password detection** — flags weak patterns like "qwerty" or "password"
- 🔒 **Session-only** — passwords never stored or sent anywhere
- 📱 **Fully responsive** — works on mobile, tablet, and desktop

---

## 🛡️ Security & Privacy

- ✅ No database or backend
- ✅ No cookies or localStorage used
- ✅ Passwords exist only in memory during your session
- ✅ Everything runs 100% client-side in your browser
- ✅ Uses `crypto.getRandomValues()` for secure password generation
- ✅ Name and birthdate fields are optional
- ✅ Personal info is never stored or sent anywhere
- ✅ Used only locally to improve password suggestions
- ✅ Cleared automatically when you close the tab

---

## 🚀 Getting Started

### Option 1 — Use the Live Site
Visit: [freyavaghela30.github.io/CipherPass](https://freyavaghela30.github.io/CipherPass)

### Option 2 — Run Locally

```bash
# Clone the repository
git clone https://github.com/freyavaghela30/CipherPass.git

# Open the project
cd CipherPass

# Open index.html in your browser
# (or use Live Server in VS Code)
```

No installation or dependencies required — just open `index.html`!

---

## 🧠 How Strength Is Calculated

| Score | Label | Criteria |
|-------|-------|----------|
| 1 | Very Weak | Less than 8 characters |
| 2 | Weak | 8+ chars, basic variety |
| 3 | Fair | 12+ chars or mixed case + numbers |
| 4 | Strong | Mixed case + numbers + symbols |
| 5 | Very Strong | All criteria met, 12+ chars, no repeats |

Entropy is calculated as: `length × log₂(pool size)`

> ⚠️ Strength is also reduced if the password contains your name, birthdate, or common patterns.

---

## 🚫 Personal Info Detection

CipherPass checks your password against:

| Check | Example |
|-------|---------|
| Your name | `freya123` → ⚠️ Warning |
| Your birth year | `pass2005` → ⚠️ Warning |
| Common passwords | `qwerty`, `admin`, `password` → ⚠️ Warning |
| Keyboard patterns | `asdf`, `1234`, `zxcv` → ⚠️ Warning |

> 💡 Name and birth year fields are completely optional and never leave your device.

---

## 📁 Project Structure

```
CipherPass/
│
├── index.html        # Main file — all HTML, CSS, and JS in one place
├── README.md         # Project documentation
├── .cursorignore     # Tells Cursor to never delete README.md
└── .cursorrules      # Cursor AI rules — only edit index.html
```

## 🛠️ Built With

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure |
| CSS3 | Styling, animations, CSS variables |
| Vanilla JavaScript | Logic, DOM manipulation |
| Web Crypto API | Secure random password generation |
| Google Fonts | Space Grotesk + JetBrains Mono |
| GitHub Pages | Free hosting & deployment |

---

## 🖥️ Tools Used

- **[Cursor](https://cursor.com)** — AI-powered code editor for building features
- **[VS Code](https://code.visualstudio.com)** — Code editing with Live Server preview
- **[GitHub](https://github.com)** — Version control and repository hosting
- **[GitHub Pages](https://pages.github.com)** — Free static site deployment

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# Fork the repo on GitHub, then:
git clone https://github.com/YOUR_USERNAME/CipherPass.git
cd CipherPass

# Make your changes, then:
git add .
git commit -m "Add: your feature description"
git push origin main

# Open a Pull Request on GitHub
```

---

## 📋 Roadmap

- [ ] Password history panel (session-only, masked display)
- [ ] Dark/light theme toggle
- [ ] PWA support (installable on mobile)
- [ ] Password comparison mode
- [ ] Breach check via HaveIBeenPwned API
- [ ] More language support

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Freya Vaghela**
- GitHub: [@freyavaghela30](https://github.com/freyavaghela30)

---

> Built with 💜 using Cursor AI + GitHub Pages