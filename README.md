# Polish Master

A small hands-free drill for Polish numbers: hear one language, say the other, and let the app check your answer by voice.

**Live app:** https://newbroman.github.io/PolishNumbershandsfree/

## Features

- Two directions: PL to EN (hear Polish, say the number in English) and EN to PL (hear the number in English, say it in Polish).
- Random numbers within a Min/Max range set by sliders (up to 999).
- Hands-free mode: the app speaks the prompt, listens, says "Correct" / "Dobrze" or the right answer, then moves on automatically.
- Shows what the microphone heard, so misrecognitions are easy to spot.
- Polish and English interface (toggle in the header) and a dark mode.

## Using it

Open the live app in a browser and press Start Training. Spoken prompts use the browser's speech synthesis, so a Polish voice should be available for pl-PL. Voice answers use speech recognition, which needs Chrome or Edge and microphone permission; without it the app still speaks prompts and can be stepped through with the Next Phrase button. There is no service worker or manifest, so it needs a connection to load.

## Project structure

- `index.html` - the whole app (markup, styles, JavaScript, including the number-to-Polish word generator and UI translations).
- `icon.png` - page icon and Apple touch icon.

## Development

No build step. From the repository folder run:

```
python3 -m http.server
```

then open http://localhost:8000.

Built by Martin Hollingham.
