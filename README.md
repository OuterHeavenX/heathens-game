# Heathens

Browser-based 3D life sim.

## Command Deck (📱 Phone button)

- **Phone tab** — open the full phone apps (Messages, Friends, Real Estate, Map…) and start City Job Board shifts.
- **Life & Relationships tab** — manage your household (text, gift, apologize, send to work, marry/divorce), invite dating-app matches over, run relationship actions, buy toys and see achievements.
- Tap a **need bar** (Hunger, Energy, Hygiene, Fun, Comfort, The Voices) to send your Heathen to do something about it.
- Spouses and roommates live in your home, wander around it and are saved with your game.

## Economy

- **Jobs** pay more per second the harder they are (easy ≈ $2/s, hard ≈ $3.4/s once you count recovery). Desk freelancing is a small side gig ($14–25).
- **Bills** come every 2 minutes: rent (studio $80, warehouse $110, 2-bedroom $160), utilities that grow with your furniture, and groceries for everyone at home (plus baby costs). Roommates chip in. Missing 3 bills makes an unmarried roommate move out.
- **Roommates** rest for 2 minutes after a shift before they can work again.

## Life & Relationships

- **Dating app** — Match new people
- **Text partner** — Flirty/normal/mean effects on affinity & jealousy
- **Post social** — Earn money; suspicious posts raise heat (especially evil)
- **Accomplice job** — Loyal roommate helps with crime for big cash + heat
- **Bribe heat** — Pay to reduce police heat
- **Cook together / Workout** — Boost needs & affinity
- **Arcade bet** — Wager $30
- **Toys** — Buy mirror / restraints / camera (bonuses to sex; camera fits evil recording flavor)
- **Overview** — See roommates, affinity, marriage, pregnancy, jealousy, heat, reputation, achievements

## Already included
Roommates (persistent), personality jobs, shared bills, jealousy, pregnancy→baby, routines, arguments (apologize/gift), sex positions, strip, threesome, record (evil), street work (via Life panel or future menu), marriage.

All saved locally.

Mature content: crime, drugs, violence, explicit.

## Development

```bash
npm install
npm run dev      # local dev server
npm run build    # production build (what GitHub Pages deploys)
```

All static files (textures, music, avatars, the dusk window) live in `public/assets` so they are copied into the build.
