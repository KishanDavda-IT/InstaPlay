# ◼ INSTAPLAY ◻

> Take a photo of any instrument. Play it instantly.  
> Black & White. Pixel Perfect. Full Range.

![Theme](https://img.shields.io/badge/theme-monochrome-000000?style=flat-square&logo=&logoColor=white&labelColor=ffffff)
![Audio](https://img.shields.io/badge/audio-Tone.js-000000?style=flat-square&logo=webaudio&logoColor=white&labelColor=ffffff)
![AI](https://img.shields.io/badge/vision-TensorFlow.js-000000?style=flat-square&logo=tensorflow&logoColor=white&labelColor=ffffff)
![License](https://img.shields.io/badge/license-MIT-000000?style=flat-square&logo=&logoColor=white&labelColor=ffffff)

**InstaPlay** is a zero-install, single-file web app that uses on-device AI to identify musical instruments from photos and turns them into playable synthesizers using the Web Audio API. No downloads, no accounts, no backend — just open and play.

---

## 📸 How It Works

1. **Upload or snap a photo** of any instrument
2. **AI recognizes** the instrument using TensorFlow.js MobileNet (runs entirely in your browser)
3. **Play instantly** with a custom interface designed for that specific instrument
4. Not detected correctly? **Manually override** with one tap

---

## 🎹 Supported Instruments

| Family | Instruments | Interface |
|--------|-------------|-----------|
| **Keys** | Piano, Keyboard, Organ, Accordion, Harpsichord | 3-octave scrollable keybed |
| **Guitar** | Acoustic, Electric, Banjo, Mandolin, Ukulele | 6-string × 4-fret fretboard |
| **Strings** | Violin, Cello, Viola, Harp | 4-string fingerboard grid |
| **Wind** | Flute, Sax, Trumpet, Trombone, Clarinet, Oboe | 12-valve brass pipe |
| **Drums** | Full Kit, Snare, Xylophone | 8-piece top-down kit |
| **Synth** | Universal fallback | 24-pad chromatic grid |

---

## 🚀 Live Demo

**[Play InstaPlay Now](https://KishanDavda-IT.github.io/instaplay)** ← *Replace with your deployed URL*

Or just download `index.html` and open it. That's it.

---

## 🎮 Controls

### Touch / Mouse
- **Tap** any key, string, drum, or pad to play
- **Multi-touch** supported for chords on piano and synth

### Keyboard (Desktop)
| Instrument | Keys |
|------------|------|
| Piano | `Z` through `/`, `Q` through `=` |
| Guitar | `Z-N`, `A-H`, `Q-Y`, `1-6` |
| Drums | `A`, `S`, `D`, `F`, `G`, `H`, `J`, `K` |
| Violin | `Z-N`, `A-H`, `Q-R` |
| Wind | `Z-N`, `A-H` |
| Synth | `Z` through `/`, `Q` through `T` |

- **Volume**: `-40dB` to `0dB`
- **Reverb**: `0%` to `100%`

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| **AI Vision** | TensorFlow.js + MobileNet v2 |
| **Audio Engine** | Tone.js (Web Audio API) |
| **UI** | Vanilla HTML/CSS, no frameworks |
| **Styling** | CSS Custom Properties, pixel-art aesthetic |
| **Deployment** | Single static file |

---

## 📦 Deployment

This is a **single HTML file**. No build step. No dependencies to install.

### Option 1: GitHub Pages (Recommended)
1. Fork or upload `index.html` to a GitHub repository
2. Go to **Settings → Pages → Deploy from branch → main**
3. Done. Your URL is `https://<user>.github.io/<repo>`

### Option 2: Netlify Drop
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag the folder containing `index.html` onto the page
3. Get an instant live URL

### Option 3: Run Locally
```bash
# Simply open the file
open index.html

# Or serve with any static server
npx serve .
python3 -m http.server 8000
