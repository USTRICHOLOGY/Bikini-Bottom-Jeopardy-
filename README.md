# Bikini Bottom Jeopardy

A SpongeBob trivia game in the style of Jeopardy, all in one `index.html`. There's nothing to build.

## How to play
1. Open the site on the laptop or TV. It's the big screen, and it shows a 5-letter game code and a QR code.
2. Players scan the QR code (or open the site and type the code), then tap their name.
3. Pick a tile. Every question has four answer choices (A to D) on each phone. The big screen marks who got it right.
4. Players without a phone answer out loud. After each reveal, tap their name to mark them right or wrong.

The board has 6 categories and 30 questions, plus a hidden Daily Double and Final Jeopardy with wagers.

Phones connect to the big screen directly through PeerJS (a free WebRTC service). It works best with everyone on the same Wi-Fi.

## Picture round ("Picture This")
A 7th category with "Who / Where / What is this?" questions about characters, places and items. Each picture starts zoomed in and pulls back as the clock runs down, and the bigger the dollar value, the further in it starts. Wrong answers are drawn from the same kind of thing (places vs. places).

The column only appears once you've added pictures. There are two ways to add them:
- **On the big screen:** Players & QR → **Picture setup**. Click a card and paste an image, drop a file on it, or upload one. Pictures saved this way stay on that laptop only.
- **In the repo:** add files to `images/` using the file names in `images/README.md`. Every device then picks them up.

## Start transition
Pressing **Start the game** plays a bubble transition on the big screen and every phone. To add your own sound effect: in the lobby, find **Start transition**, tap **Load sound** and pick an audio file (MP3, M4A, WAV or OGG). The sound saves on that laptop, and **Preview** plays it with the animation. If no sound is loaded, the game plays built-in bubble pops. To use a bubble video, tap **Load video** under **Bubble video** and pick a WebM with a transparent background. It plays on the big screen, and phones show built-in CSS bubbles. You can also put files at `sounds/transition.mp3` and `sounds/bubbles.webm` in the repo.
