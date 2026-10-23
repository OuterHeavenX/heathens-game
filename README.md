# Heathens

Browser-based 3D life sim.

## Command Deck (📱 Phone button)

- **Phone tab** — open the full phone apps (Messages, Friends, Real Estate, Map…) and start City Job Board shifts.
- **Life & Relationships tab** — manage your household (text, gift, apologize, send to work, marry/divorce), invite dating-app matches over, run relationship actions, buy toys and see achievements.
- Tap a **need bar** (Hunger, Energy, Hygiene, Fun, Comfort, The Voices) to send your Heathen to do something about it.
- Spouses and roommates live in your home, wander around it and are saved with your game.

## Economy

- **Jobs** pay more per second the harder they are (easy ≈ $2/s, hard ≈ $3.4/s once you count recovery). Desk freelancing is a small side gig ($14–25).
- **Bills** come every 2 minutes of game time: rent (studio $80, warehouse $110, 2-bedroom $160), utilities that grow with your furniture, and groceries for everyone in the household (plus baby costs). Every roommate chips in a share of their wage, whether or not they're at work right now.
- **Unpaid bills** — if you can't cover a bill you pay what you can and the rest becomes debt, which is taken from any cash you earn until it's cleared. Missing 3 bills makes an unmarried roommate move out; with nobody to blame, the eviction stress hits your happiness and comfort instead.
- **Roommates** rest for 2 minutes after a shift before they can work again.
- **Arcade** — each play costs a $5 token and each run pays up to $40.
- **Cooldowns** (posting, accomplice jobs, recording, texting) run on game time and are saved with your game.

## Life & Relationships

- **Dating app** — Match new people
- **Text partner** — Flirty/normal/mean effects on affinity & jealousy
- **Post social** — Earn money; in Evil Mode a suspicious post pays extra but raises heat
- **Accomplice job** — Loyal roommate helps with crime for big cash + heat
- **Bribe heat** — Pay to reduce police heat
- **Cook together / Workout** — Boost needs & affinity
- **Arcade bet** — Wager $30
- **Toys** — Buy mirror / restraints / camera (mirror and restraints boost sex with anyone; the camera makes recordings sell for more)
- **Overview** — See roommates, affinity, marriage, pregnancy, jealousy, heat, reputation, achievements

## Already included
Roommates (persistent), personality jobs, shared bills, jealousy, pregnancy→baby, routines, arguments (apologize/gift), sex positions, strip, threesome, record (evil), street work (via Life panel or future menu), marriage.

All saved locally. Volume and game speed can be changed in the ⏸️ pause menu.

Mature content: crime, drugs, violence, explicit.

## Development

```bash
npm install
npm run dev      # local dev server
npm run build    # production build (what GitHub Pages deploys)
```

All static files (textures, music, avatars, the dusk window) live in `public/assets` so they are copied into the build.
