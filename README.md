# 猫と本を読む — Reading with a Cat

An interactive, vertical Japanese "bead curtain" made of text. Grab a word to pull that strand of beads; let go and it springs back. Whenever you grab a word, a vertical paper card pops up with the word, its furigana, and a cat lounging on the bottom edge — and the word is read aloud.

**Live demo:** https://kanaworksai-hue.github.io/ReadingWithACat/

## Features

- **Text bead curtain** — characters hang as independent vertical strands using Verlet physics. No wind: it rests perfectly still until you touch it.
- **Grab a word, not just a character** — grabbing any bead selects the whole word it belongs to; the strand swings and springs back together.
- **Contextual readings** — [kuromoji.js](https://github.com/takuyaa/kuromoji.js) tokenizes any text so the same kanji is read correctly in different words (e.g. 見当 = けん / 見た = み).
- **Natural speech** — the selected word is spoken with the Web Speech API using its pronunciation, not a robotic per-character readout.
- **Editable** — type any text in the box and the curtain (and its readings) update live.
- **A reading companion** — a cat rests on each card, its tail swaying, occasionally opening its eyes.
- **Mobile friendly** — touch to part the beads and tap a word to hear it.

## Usage

Open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari), or visit the live demo link above. An internet connection is used once to load the kuromoji dictionary; while it loads (or offline) the app falls back to approximate readings.

## Tech

HTML5 Canvas · Verlet integration · kuromoji.js (morphological analysis) · Web Speech API. Everything is in a single self-contained `index.html`.

## Credits

- Default text: excerpt from *I Am a Cat* (吾輩は猫である) by Natsume Sōseki — public domain.
- Logo and project: [@KanaWorks_AI](https://x.com/KanaWorks_AI)
