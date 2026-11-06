# Bikini Bottom Jeopardy

A SpongeBob trivia game in the style of Jeopardy, all in one `index.html`. There's nothing to build.

## How to play
1. Open the site on the laptop or TV. It's the big screen, and it shows a 5-letter game code and a QR code.
2. Players scan the QR code (or open the site and type the code), then tap their name.
3. Pick a tile. Every question has four answer choices (A to D) on each phone. The big screen marks who got it right.
4. Players without a phone answer out loud. After each reveal, tap their name to mark them right or wrong.

The board has 6 categories and 30 questions, plus a hidden Daily Double and Final Jeopardy with wagers.

Phones connect to the big screen directly through PeerJS (a free WebRTC service). It works best with everyone on the same Wi-Fi.
