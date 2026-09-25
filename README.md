# 🎂 Happy Birthday, Satte

A little interactive birthday surprise website made for my sister.

It plays like a tiny four-part game:

1. **Unwrap the present** – tap the gift to open it and start the party.
2. **Blow out the candles** – make a wish, then tap each flame on the cake.
3. **Tap to Flip** – every flip hides something special about her.
4. **Open the letter** – a birthday letter appears with falling confetti.

It works on phones and computers, has small built-in sound effects (with a mute button), and needs no installation. Everything is in one file: `index.html`.

---

## 📁 Files

```
sachita-birthday/
├── index.html   ← the whole website (HTML + CSS + JavaScript)
└── README.md    ← this file
```

---

## ▶️ How to run it
Run a local server
Open a terminal in the project folder and run **one** of these:

```bash
# With Python (already installed on most Mac/Linux computers)
python3 -m http.server 8000
```

```bash
# With Node.js
npx serve .
```

Then open https://sachita-hbd.vercel.app/ (Node) in your browser.

To test it on your phone, connect it to the same Wi-Fi and open `http://YOUR-COMPUTER-IP:8000`.

---

## ✏️ How to personalize it

Open `index.html` in any text editor (Notepad, VS Code, etc.) and find the `CONFIG` section near the bottom:

```js
const CONFIG = {
  name: "Sachita",              // her name
  from: "Your favourite person", // who it's from, e.g. "Your sibling"
  candles: 5,                    // number of candles on the cake
  reasons: [ ... ],              // one message per balloon (add or remove freely)
  letter: [ ... ]                // paragraphs of the final letter
};
```



```bash
git init
git add .
git commit -m "Birthday surprise for Sachita"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/sachita-birthday.git
git push -u origin main
```

Then import the repo on Vercel as in step 3.

---

## 🛠️ Built with

- Plain HTML, CSS, and JavaScript (no frameworks, no build step)
- Google Fonts: Sniglet and Quicksand
- Web Audio API for the sound effects
- Canvas for the confetti

---

Made with 💖 for my sister's birthday.
