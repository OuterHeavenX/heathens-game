# Heathens

A browser-based 3D life simulation game, packaged as a self-contained static site.

## Play locally

Requires [Node.js](https://nodejs.org/) 20 or newer.

```bash
npm install
npm run dev
```

Open the URL printed by Vite (normally `http://localhost:5173`).

## Production build

```bash
npm install
npm run build
npm run preview
```

The deployable static site is generated in `dist/`.

## Controls

The game is primarily mouse/touch driven. Use the on-screen controls to move, interact with characters and furniture, open the phone, and manage your character.

Progress is saved in your browser's local storage.

## Visitors & Roommates

**While a guest is visiting**, tap them for:

- 😂 Laugh / 💬 Talk / 🃏 Joke / 🤡 Play the fool / 🎤 Sing
- 😘 Cheek kiss / 💋 Make out / 🛏️ Have sex
- 🏠 Invite to move in (needs affinity ~35+)
- 🚪 Send Home

**Once they move in** (persistent, saved across sessions):

- Same social options anytime they're home
- 💼 Send to work — they leave for a while and return with wages that go straight to your money
- 💍 Propose / Marry (needs higher affinity ~60+)
- 💔 Divorce
- 📦 Ask to move out

Roommates stay in your apartment, are saved in localStorage, and reappear when you reload. Work timers and marriage status persist.

## Content note

This game contains mature themes, including fictional crime, drugs, violence, and adult interactions.
