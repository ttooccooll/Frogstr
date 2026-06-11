# FROGSTR

A Frogger clone but the cars/logs are real nostr notes. Dodge the bitcoin ones, ride the GM/GN ones.

## What's happening

- **Cars = bad:** Notes about bitcoin, sats, lightning, zap, etc.
- **Logs = good:** Notes saying GM or GN
- 14 relays at once so there's always stuff coming at you
- NIP-07 login (nos2x, Alby, etc.) so you can share your score as a nostr note

## Run it

Just open `index.html` in a browser. No build step, no server needed.

## Controls

- Desktop: Arrow keys or WASD
- Mobile: Swipe or tap

## Donate

There's a donate button with a QR code. Edit the lightning address in `index.html` if you want to change it.

## Score

- +100 every time you make it home
- +500 bonus for filling all 5 spots

## Tech

- Plain HTML/CSS/JS
- QRCode.js for the donate QR
- WebSocket to nostr relays
- NIP-07 for signing
- Press Start 2P font for the vibe