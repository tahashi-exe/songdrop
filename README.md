# 🎵 SongDrop

**Share music, personally.**

SongDrop transforms song links into beautiful, retro-styled shareable cards. Add personal notes, customize the look, and send meaningful music moments to friends — all with a nostalgic iPod twist.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://yourusername.github.io/songdrop/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## ✨ Features

- 🎧 **Retro iPod Design** — Beautifully crafted iPod interface with working click wheel, LCD screen, and wired earphones
- 🎨 **10 iPod Colors** — Classic White, Space Black, Blush Pink, Powder Blue, Mint, Sunflower, Lavender, Flame, Silver, and Copper
- 🌈 **8 Background Vibes** — Midnight, Dusk, Ember, Ocean, Forest, Rose, Ivory, and Paper themes
- 📝 **Sticky Notes** — Add handwritten-style personal messages with authentic sticky note design
- 🔗 **Private Shareable Links** — Generate unique URLs that work instantly, no signup required
- 📱 **Fully Responsive** — Works perfectly on desktop, tablet, and mobile
- ⚡ **Zero Backend** — Pure client-side app, no servers, no databases, no tracking
- 🎵 **Platform Support** — Works with Spotify and Apple Music links

---

## 🚀 Live Demo

**[Try SongDrop Now →](https://yourusername.github.io/songdrop/)**

---

## 📸 Screenshots

### Creator Interface
![Creator Interface](screenshots/creator.png)

### iPod Card View
![iPod Card](screenshots/ipod-card.png)

---

## 🎯 How It Works

1. **Paste a Song Link**  
   Drop in a Spotify or Apple Music URL

2. **Add Your Touch**  
   - Write a personal note on the sticky note (optional)
   - Pick a background vibe
   - Choose your iPod color

3. **Generate & Share**  
   Get a unique private link to send to anyone

4. **They See Your Creation**  
   Your friend opens the link and sees a beautiful retro iPod displaying the song with your note

---

## 💻 Usage

### For Senders

```
1. Visit https://yourusername.github.io/songdrop/
2. Paste your Spotify or Apple Music link
3. Toggle "Add a sticky note" if you want to include a message
4. Choose your background vibe and iPod color
5. Click "✦ Create & Share"
6. Copy the generated link and send it to your friend!
```

### For Recipients

```
Simply click the link you received — the song card loads instantly.
Click the platform badge to open the song in Spotify or Apple Music.
```

---

## 🛠️ Technical Details

- **Framework:** Vanilla JavaScript (no dependencies)
- **Styling:** Custom CSS with CSS Variables for theming
- **Fonts:** Google Fonts (Playfair Display, Lora, Caveat, VT323)
- **Data Storage:** URL hash encoding (Base64 + JSON)
- **APIs:** Spotify & Apple Music oEmbed (with manual fallback)
- **Hosting:** GitHub Pages (static site)

---

## 🏗️ Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/songdrop.git
   cd songdrop
   ```

2. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   open index.html
   
   # Or use a local server (recommended)
   python -m http.server 8000
   # Visit http://localhost:8000
   ```

3. **Make changes**  
   All code is in `index.html` — edit and refresh to see changes

---

## 📁 Project Structure

```
songdrop/
├── index.html          # Main application file (HTML + CSS + JS)
├── README.md           # This file
├── LICENSE             # MIT License
├── SETUP.md            # Detailed GitHub Pages setup guide
└── screenshots/        # Demo images (optional)
    ├── creator.png
    └── ipod-card.png
```

---

## 🎨 Customization

### Change Default Theme
Edit the CSS variables in `index.html`:
```css
:root {
  --bg: #0d0d0f;
  --accent: #e8c47a;
  --sticky: #f5e96b;
}
```

### Add More iPod Colors
Add entries to the `IPOD_COLORS` array in the JavaScript:
```javascript
const IPOD_COLORS = [
  { hex: '#your-color', name: 'Your Color Name' },
  // ...
];
```

### Modify Background Options
Edit the `BACKGROUNDS` array:
```javascript
const BACKGROUNDS = [
  { id:'bg-custom', label:'Custom', style:'background:your-gradient' },
  // ...
];
```

---

## 🐛 Known Issues & Limitations

- **CORS Blocking:** Spotify and Apple Music oEmbed APIs are blocked by browser CORS policies, so manual song entry is required in most cases
- **No Playback:** The iPod is visual only — clicking the platform badge opens the song in the respective app
- **No Server:** All data is encoded in the URL, so extremely long notes may hit URL length limits (rare)

---

## 🗺️ Roadmap

- [ ] Add more music platform support (YouTube Music, SoundCloud, Bandcamp)
- [ ] Audio preview integration
- [ ] More retro device themes (Walkman, boombox, radio)
- [ ] Playlist support (multiple songs in one link)
- [ ] QR code generation
- [ ] Export as image feature

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- 🐛 Report bugs
- 💡 Suggest features
- 🎨 Submit design improvements
- 📝 Improve documentation

**To contribute:**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 💖 Acknowledgments

- Inspired by the iconic iPod Classic design
- Built with love for music sharing and nostalgia

---

## 📬 Contact

Have questions or feedback? Open an issue or reach out!

**Made with 🎵 and ✨**

---

## ⭐ Star this repo if you like it!

If SongDrop helped you share a meaningful song, consider giving it a star ⭐ — it helps others discover the project!
