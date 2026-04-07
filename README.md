# Emoji Burst Input

Typing animation that shoots emoji particles from the text cursor. Each keystroke launches colorful emojis that arc up and fade out.

## Quick Start

```html
<iframe
  src="index.html"
  style="width:500px; height:300px; border:none;">
</iframe>
```

## Demo

Open `index.html` in a browser and start typing to see emojis burst from the cursor.

## Features

- Emojis launch upward with physics-based arcs
- Particles spin and fade as they fall
- Uses crisp Twemoji SVGs (Twitter's emoji set)
- Configurable physics and appearance

## Configuration

Edit the `CONFIG` object in `index.html` to customize:

```javascript
const CONFIG = {
  // Physics
  gravity: 0.4,              // Downward acceleration
  initialSpeedMin: 10,       // Min launch speed
  initialSpeedMax: 17,       // Max launch speed

  // Appearance
  sizeMin: 72,               // Min emoji size (px)
  sizeMax: 110,              // Max emoji size (px)

  // Spawning
  particlesPerKey: 1,        // Emojis per keystroke
};
```

## Emoji Set

Default emojis: ✨ 🔥 ⭐ 💫 🎉 💖 🌈 🌟

To change emojis, edit the `images` array in CONFIG with Twemoji URLs:
```javascript
images: [
  'https://cdn.jsdelivr.net/gh/twitter/twemoji@latest/assets/svg/2728.svg',  // ✨
  // Add more...
]
```

Find emoji codes at: https://twemoji.twitter.com/

## Tech

Pure HTML + CSS + JavaScript. Uses Twemoji CDN for crisp SVG emojis.
