# QR Cards

A lightweight, no-framework card-reveal page. Two sets of cards (A and B) are randomly drawn on load. Tap a card to flip it and reveal the QR code image underneath.

## Features

- 🎴 Random card drawn from each set on every load
- 🔄 **Redraw** button picks fresh cards without a full page reload
- 👆 **Flip All / Unflip All** toggle
- ⌨️ Full keyboard navigation (Tab to focus, Enter/Space to flip)
- 📱 Responsive — works on mobile and desktop
- ♿ ARIA roles and labels for screen readers

## File Structure

```
qr-cards/
├── index.html      # Single-file app — all HTML, CSS, and JS
├── a1.png … a6.png # Card set A images
├── b1.png … b6.png # Card set B images
└── README.md
```

## How to Use

### Locally
Just open `index.html` in any browser — no build step, no dependencies.

### GitHub Pages (recommended)
1. Push this folder to a GitHub repository.
2. Go to **Settings → Pages**.
3. Under *Source*, select **Deploy from a branch** → `main` → `/ (root)`.
4. Save. Your page will be live at `https://<username>.github.io/<repo-name>/`.

## Customising Cards

- **Add images**: Drop new PNGs into the folder and add their filenames to the `SETS` object inside `index.html`.
- **Add more sets**: Extend the `SETS` object with a new key (e.g. `C: ["c1.png", ...]`).
- **Change the theme**: Edit the CSS variables at the top of the `<style>` block (`--bg`, `--accent`, etc.).

## License

MIT — do whatever you like with it.
