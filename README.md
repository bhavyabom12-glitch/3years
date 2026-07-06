# 🍊 Santero Island · A Love Mystery

A cozy visual novel mystery game for two. Investigate a disappearance, interrogate quirky island residents, solve puzzles, and uncover a romantic resolution.

![Game Screenshot](https://via.placeholder.com/780x460/fcf5c8/d9a066?text=Santero+Island+Mystery)

---

## 🎮 Play the Game

Visit: `https://yourusername.github.io/repo-name/`

(Replace `yourusername` and `repo-name` with your actual GitHub username and repository name.)

---

## 🕹️ How to Play

1. **Read the dialogue** and click **Next** to advance the story.
2. When a **puzzle** appears, type your answer and click **Check**.
3. Use the **Resident List** and **Case File** to track evidence and suspects.
4. At the finale, **click the 7 fruits** on the tree to reveal anniversary gifts.
5. **Press Space or Enter** as a keyboard shortcut to advance dialogue.

---

## 📂 File Structure

```
/
├── index.html              # The complete game
├── README.md               # This file
└── assets/
    └── sprites/            # Place your character PNGs here
        ├── agent_b-removebg-preview.png
        ├── agent_b2-removebg-preview.png
        ├── agent_b3-removebg-preview.png
        ├── sierra-removebg-preview.png
        ├── luz-removebg-preview.png
        ├── amity-removebg-preview.png
        ├── soyona-removebg-preview.png
        ├── brooklynn-removebg-preview.png
        ├── naruto-removebg-preview.png
        ├── sasuke-removebg-preview.png
        ├── jax-removebg-preview.png
        ├── ragatha-removebg-preview.png
        ├── ellie-removebg-preview.png
        └── abby-removebg-preview.png
```

---

## 🖼️ Adding Sprites

1. Create an `assets/sprites/` folder in your repository.
2. Add **transparent PNG images** with these exact filenames:

| Character | Filename | Fallback Emoji |
|-----------|----------|----------------|
| Agent B (normal) | `agent_b-removebg-preview.png` | 🕵️ |
| Agent B (van explanation) | `agent_b2-removebg-preview.png` | 🕵️‍♀️ |
| Agent B (blushing) | `agent_b3-removebg-preview.png` | 🥰 |
| Sierra Santero | `sierra-removebg-preview.png` | 👧 |
| Luz Noceda | `luz-removebg-preview.png` | 🦉 |
| Amity Blight | `amity-removebg-preview.png` | 📝 |
| Soyona Santos | `soyona-removebg-preview.png` | 🦖 |
| Brooklynn | `brooklynn-removebg-preview.png` | 📡 |
| Naruto Uzumaki | `naruto-removebg-preview.png` | 🍥 |
| Sasuke Uchiha | `sasuke-removebg-preview.png` | ⚔️ |
| Jax | `jax-removebg-preview.png` | 🎪 |
| Ragatha | `ragatha-removebg-preview.png` | 🎀 |
| Ellie Williams | `ellie-removebg-preview.png` | 🎸 |
| Abby Anderson | `abby-removebg-preview.png` | 🏹 |

> **💡 Tip:** Use [remove.bg](https://remove.bg) or Canva to remove backgrounds from your sprites. If a sprite is missing, the game will display the fallback emoji instead.

---

## 🎨 Customizing Fruit Links

Edit the `FRUIT_URLS` array in `index.html` (around line 950):

```javascript
const FRUIT_URLS = [
    '#', // Fruit 1 – Sweet memory (digital message)
    'https://open.spotify.com/playlist/YOUR_PLAYLIST_ID', // Fruit 2 – Playlist
    '#', // Fruit 3 – Poem (handled internally)
    'https://example.com/photos', // Fruit 4 – Photo collage
    'https://example.com/coupons', // Fruit 5 – Coupons
    'https://example.com/confession', // Fruit 6 – Confession
    'https://example.com/drawing.png' // Fruit 7 – Drawing
];
```

### Fruit Details

| Fruit | Content | Notes |
| :--- | :--- | :--- |
| 🍊 Fruit 1 | Sweet digital message | Customize the text in the `pluckFruit` function |
| 🍎 Fruit 2 | Spotify playlist | Change the URL to your own playlist |
| 🍇 Fruit 3 | Love poem letter | Content is inside the `pluckFruit` function |
| 🍉 Fruit 4 | External link | Change URL to your photo collage |
| 🍑 Fruit 5 | External link | Change URL to your coupons |
| 🍒 Fruit 6 | External link | Change URL to your confession |
| 🥝 Fruit 7 | External link | Change URL to your drawing/image |

---

## 🧩 Puzzle Solutions

| Puzzle | Solution |
|--------|----------|
| Footprint | `luz amity` |
| Spotify Hidden Message | `tyler, do you know? missing girls are found by dinosaurs on empty beaches` |
| Shuriken Count | `7` |
| Glitch Unscramble | `balance` |
| Van Plate | `nyc419` |

---

## 🚀 Deploy to GitHub Pages

1. **Create a repository** on GitHub (e.g., `santero-mystery`).
2. **Upload `index.html`** and the `assets/` folder.
3. Go to **Settings → Pages**.
4. Select **Deploy from branch** → `main` → `/ (root)`.
5. Your game will be live at `https://yourusername.github.io/repo-name/`.

### Quick Deployment

```bash
git clone https://github.com/yourusername/santero-mystery.git
cd santero-mystery
# Add index.html and assets folder
git add .
git commit -m "Initial commit"
git push origin main
```

Then enable GitHub Pages in the repository settings.

---

## 🎨 Customizing Colors

The game uses a warm pastel palette. Edit these CSS variables in the `<style>` section:

```css
body {
    background: #fcf5c8;  /* Main background */
    background-image: radial-gradient(circle at 20% 30%, #fde8d0 0%, #fcf5c8 60%, #d4e6f5 100%);
}

.game-container {
    background: rgba(255, 251, 240, 0.88);  /* Container background */
    border: 2px solid #f0d5b0;  /* Border color */
}

.vn-dialogue {
    background: #fffbf4;  /* Dialogue box background */
    border: 2px solid #f0d5b0;
}

.puzzle-btn {
    background: #d9a066;  /* Primary button color */
}

.badge-btn {
    background: #f0d5b0;  /* Secondary button color */
}
```

---

## 📖 Story Summary

You play as **Detective Tyler**, investigating the disappearance of Sierra "Vanny" Santero on a remote tropical island. As you interrogate five eccentric couples, you uncover a black‑market smuggling operation, a faked disappearance, and a romantic conspiracy that ties it all together.

**The Twist:** Agent "B" (your partner) has been undercover the whole time, and Sierra is alive – she faked her own abduction to expose her parents' illegal Heartwood trade.

**The Finale:** A pixel‑art tree bearing 7 fruits, each hiding a gift that celebrates your anniversary.

---

## 🛠️ Built With

- **HTML5** – Structure
- **CSS3** – Styling & animations
- **Vanilla JavaScript** – Game logic & interactivity
- **Spotify Embeds** – Music integration
- **GitHub Pages** – Hosting

---

## 📄 License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).
