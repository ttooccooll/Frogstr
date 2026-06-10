# FROGSTR

A nostr-powered Frogger arcade game. Dodge real-time bitcoin and nostr notes (the cars), ride GM/GN notes (the logs) across the river. All game content is pulled live from the nostr network.

## How It Works

- **Cars (dangerous):** Real nostr notes containing bitcoin/nostr keywords (bitcoin, btc, sats, nostr, zap, lightning, relay, damus, primal, etc.)
- **Logs (safe to ride):** Real nostr notes containing GM/GN greetings
- **14 relays** connected simultaneously for maximum note throughput
- **NIP-07 login** lets players share their score as a nostr note when their game ends

## Setup

This is a single `index.html` file. No build step required. Just serve it or open it in a browser.

### Lightning Address (Donate Button)

The donate button uses a QR code with your lightning address. Open `index.html` and find this line:

```javascript
const LIGHTNING_ADDRESS = "jasonbohio@blink.sv";
```

Replace with your lightning address.

## Controls

- **Desktop:** Arrow keys or WASD
- **Mobile:** Swipe to move, tap to hop forward

## Features

- 80s arcade aesthetic with CRT scanlines, pixel art, and retro fonts
- Real-time nostr notes as game objects (14 relays)
- NIP-07 nostr login (nos2x, Alby, etc.)
- Share your score on nostr when game ends
- Lightning donate button for zapping the dev (QR code)
- Stacker.news link for micro-blogging
- Fully client-side, no backend needed

## Scoring

- +100 points for each safe home reached
- +500 bonus for filling all 5 homes

## Tech

- Pure HTML/CSS/JS with QRCode.js for donate QR
- Connects to nostr relays via WebSocket
- Uses NIP-07 for signing (browser extension required for login/sharing)
- Press Start 2P font from Google Fonts for arcade feel

## License

MIT