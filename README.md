# 🎯 Word Nexus

A challenging word grouping puzzle game inspired by Connections, with a unique twist!

## 🎮 Play Now

[**Play Word Nexus**](https://yourusername.github.io/word-nexus/)

## 🌟 Features

- **155+ Unique Categories** - Massive variety ensures puzzles rarely repeat
- **3 Difficulty Levels**
  - **Easy**: Simple everyday categories (Fruits, Colors, Animals, etc.)
  - **Medium**: Pop culture, geography, tech, and general knowledge
  - **Hard**: Advanced topics, Gen-Z slang, internet culture, and specialized knowledge
- **Chaos Tile Mechanic** - One random word doesn't belong to any category. Avoid it!
- **Sound Effects** - Satisfying audio feedback (toggleable)
- **Progress Tracking** - Best scores per difficulty and total games played
- **Share Results** - Wordle-style emoji sharing
- **Mobile-Friendly** - Responsive design works on all devices
- **Offline Support** - Fully playable without internet connection

## 🎯 How to Play

1. **Goal**: Group 16 words into 4 categories of 4 words each
2. **Select** 4 words you think belong together
3. **Check** your grouping
4. **Beware**: One word (the Chaos Tile) doesn't belong to ANY category
5. **Win**: Find all 4 groups with 4 or fewer mistakes

## 📊 Categories Include

- Animals, Food, Geography, Technology
- Movies, Gaming, Sports, Music
- Internet Culture, Memes, Gen-Z Slang
- Science, History, Literature, Philosophy
- And 130+ more!

## 🚀 Technology

- **Single HTML File** - No build process required
- **Vanilla JavaScript** - No frameworks or dependencies
- **localStorage** - Progress tracking persists across sessions
- **Web Audio API** - Optional sound effects
- **Seeded Random Generator** - For consistent puzzle generation

## 📦 Installation

### Play Locally

1. Clone this repository:
```bash
git clone https://github.com/yourusername/word-nexus.git
cd word-nexus
```

2. Open `index.html` in your browser:
```bash
open index.html
```

That's it! No build process needed.

### Deploy to GitHub Pages

1. Fork this repository
2. Go to Settings → Pages
3. Set Source to "main" branch
4. Your game will be live at `https://yourusername.github.io/word-nexus/`

## 🎨 Customization

The game is contained in a single HTML file, making it easy to customize:

- **Add Categories**: Edit the `PUZZLE_CATEGORIES` object in the `<script>` section
- **Adjust Difficulty**: Modify `CONFIG.MAX_MISTAKES` or category assignments
- **Change Colors**: Update CSS variables in the `<style>` section
- **Modify Chaos Tiles**: Edit the `CHAOS_TILES` array

## 🤝 Contributing

Contributions are welcome! To add new categories:

1. Fork the repository
2. Add categories to `PUZZLE_CATEGORIES` in `index.html`
3. Ensure each category has exactly 4 words
4. Test that words don't overlap with other categories
5. Submit a pull request

## 📄 License

MIT License - feel free to use this code for your own projects!

## 🙏 Acknowledgments

- Inspired by the New York Times Connections game
- Built with vanilla JavaScript for maximum compatibility and performance
- Emoji support for fun social sharing

## 📱 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🐛 Known Issues

None currently! Report bugs via [GitHub Issues](https://github.com/yourusername/word-nexus/issues).

---

Made with ❤️ for word puzzle enthusiasts everywhere!
