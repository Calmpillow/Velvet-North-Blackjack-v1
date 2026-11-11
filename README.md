# Velvet North Blackjack — character creator edition

A mobile-first private multiplayer blackjack table with casino-inspired felt, animated cards/chips, and a built-in character creator.

## What's included
- Blackjack table and existing host-authoritative PeerJS multiplayer flow (up to 12 seats).
- Character creator with masculine and feminine style catalogs.
- 100 selectable options in each of six categories for each presentation: hair, shirts, hats, glasses, chains, and necklaces (1,200 catalog entries total).
- Eight skin tones, original unbranded colors/styles, live SVG character preview, random-look button, and local saved appearance.
- Player appearance is sent to the host when joining and displayed beside each player's name at the table.
- Animated Velvet North loading screen on initial launch and while opening/joining a room.
- Responsive layout for desktop and mobile.

## Files
- `index.html` — app structure, creator UI, loading screen, and PeerJS loader
- `style.css` — table, responsive styling, character creator, and loading animations
- `game.js` — blackjack logic, multiplayer state, generated cosmetic catalogs, avatar rendering, and local appearance saving

## Publish
Upload all four files (`index.html`, `style.css`, `game.js`, and `README.md`) to the root of a GitHub Pages repository, then enable Pages from the repository's main branch and root folder.

## Play with friends
1. Open the published game, enter a display name, and select **Customize** to style your character.
2. Save the look, enter a room code, then create or join the table.
3. Share the published link and room code with friends.
4. Everyone places a bet; the host selects **Deal cards**.
5. Players use Hit, Stand, or Double on their own devices.

## Notes
- Cosmetic artwork is generated locally with original SVG/CSS shapes and palettes; no third-party branded assets or logos are included.
- Appearance is saved in the browser's local storage and shared with the host at join time. Each player customizes on their own device before joining.
- PeerJS's public signaling service is used to establish direct browser-to-browser connections. The host must keep the game tab open and online.
- Each player starts with 250,000 virtual chips. Balances last for the current hosted table only. Virtual chips only; no real-money wagering.
- Room codes are not authentication. This is a casual friends-only prototype, not a hardened production gambling platform.

## Validation
The JavaScript source passes `node --check`, and the ZIP archive is integrity-checked before delivery. A live multi-device browser session is still required to verify real PeerJS connections and cross-device behavior.
