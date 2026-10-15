# Room, Lighting & UI QA

- Room reference: warm dusk studio with a blinded city window, glowing wall pools, dark walnut floor and a dark woven rug
- Implementation evidence: production build served locally (`vite preview`), headless Chromium
- Tested viewports: 430 × 932 (phone portrait), 844 × 390 (phone landscape), 1280 × 720 (desktop)

## Lighting and textures

1. Three.js r184 uses physical light units, so the old point lights (intensity ≈ 1) were invisible and the room looked flat. The rig now has a warm key light with a properly sized shadow frustum, a window "sunset" light, three warm/cool point lights and a low ambient.
2. Time of day drives the mood: neutral by day, golden at dusk (≈16:00–20:00), cool and lamp-lit at night. Home-only lights switch off in the park, arcade, market and store, which get a brighter ambient instead.
3. Walls now use a generated plaster texture with floor and ceiling occlusion bands; the rug uses a generated woven texture with borders; the floor is slightly glossier.
4. The window gets blinds, and the city picture now depth-tests correctly (before, it was drawn on top of anything standing in front of the window).
5. A CSS vignette and warm bloom grade the canvas; portrait framing zooms in so the room fills the screen.
6. **Textures/music/avatars were 404ing in production**: the root `assets/` folder was never copied into the Vite build. Everything now lives in `public/assets`.

## Spouse / roommate fixes

- Roommates whose id lives in the arcade list (Riko, Nova, Pixel, Bear) were skipped when a save loaded, so a married arcade friend stayed in the Life panel but had no body in the room. Loading now spawns everyone, and a self-healing spawn catches any other missing body.
- Roommates are seated on a free floor tile, re-seated when you change homes, wander the room and animate.
- "At work" can no longer get stuck, and restarting the game now clears roommates, bills, heat and toys.
- Moving in promotes the visitor to a roommate (no duplicate body). Dating-app matches can be invited over, get a generated look, and can move in and marry.
- The menu now shows "spouse", and Marry, Divorce and Move out report results; Divorce and Move out ask for confirmation.

## UI and action fixes

- Command Deck tabs now work; Phone tab opens the real phone apps, which were previously unreachable. "More" and "Life" in the phone work, and its profile shows the real traits.
- Need bars are buttons (Hunger → eat, Energy → sleep, …). Evil furniture got its missing "use" label; the wicker chair can be used.
- Person menu is a compact two-column sheet that fits on screen; missing Tailwind colours were added; "Go Home" no longer covers the needs panel.
- Actions that failed silently (marry, gift, toys, street work, move in…) now show a toast.

## Final findings

- Browser console errors: none; no failed network requests
- Production build: passed
- Interaction checks passed: HUD buttons, shop, deck tabs/actions, phone app, customizer, inventory, pause/restart, spouse menu, invite → move in → marry → reload → travel
