# Lexicon — Personal Word Dictionary

A personal vocabulary website with two pages:
- **Gallery** (`index.html`) — browse all words, shuffle/reorganize by theme or source
- **Practice** (`practice.html`) — flashcard and quiz modes to learn your words

## 🗂 File Structure

```
├── words.json        ← SINGLE SOURCE OF TRUTH — add words here
├── index.html        ← Gallery page
├── practice.html     ← Practice page
└── README.md
```

## ➕ Adding New Words

Open `words.json` and add an entry to the `"words"` array:

```json
{
  "word": "Ephemeral",
  "definition": "Lasting for a very short time",
  "source": "Book Title or leave out",
  "tags": ["time", "transience"]
}
```

Only `"word"` is required. All other fields are optional.

**Available tag ideas:** personality, philosophy, emotion, language, law, politics, knowledge, behavior, time, movement, excess, chaos, learning, psychology, literature, formal, latin, ...

## 🚀 Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `lexicon`)
2. Push all files:
   ```bash
   git init
   git add .
   git commit -m "Initial lexicon"
   git remote add origin https://github.com/YOUR_USERNAME/lexicon.git
   git push -u origin main
   ```
3. Go to **Settings → Pages → Source → Deploy from branch → main / root**
4. Your site will be live at `https://YOUR_USERNAME.github.io/lexicon/`

## 🔄 Adding Words Later

```bash
# Edit words.json, then:
git add words.json
git commit -m "Add new words"
git push
```

GitHub Pages will update automatically within ~1 minute.
