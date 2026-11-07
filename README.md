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
A 7th category with "Who / Where / What is this?" questions. Each picture starts zoomed in and pulls back as the clock runs down, and the higher the dollar value, the further in it starts. Pictures load from `images/`, using the file names listed in `images/README.md`.

## Transitions
There's an animated title screen. Pressing Start, starting the game, and opening any question each play the bubble transition, using `sounds/transition.mp3` and `sounds/bubbles.webm` (built-in bubbles if those are missing).

## Art
The UI art in `ui/` (desktop and phone backgrounds, logo sign, blue board tiles, wooden category signs, clue card, framed lobby boards, four painted answer buttons) is original hand-painted-style artwork generated with Higgsfield (GPT Image 2.6), using painted reference stills for texture and color only.

## Question music
Add tracks as `sounds/music1.mp3`, `sounds/music2.mp3` and so on, up to `music12.mp3`. A random track fades in while each question is up and fades out at the reveal.
