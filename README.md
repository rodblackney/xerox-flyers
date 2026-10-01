# Xerox Flyers

A punk show flyer maker in the browser. Cut-out ransom-note headline letters, info pasted on torn paper strips, a photo run through a fake photocopier, and a starburst for the price.

**Live:** https://rodblackney.github.io/xerox-flyers/ (once GitHub Pages is on)

## What it does

- **Three looks:** Xerox (black and white, hand-lettered), Riot (hot pink stencil letters, typewriter strips) and Magazine (mixed full-colour scraps).
- **Edit the words:** headline, lineup, date, venue and price.
- **Photocopy a photo:** upload any image and it gets thresholded with a coarse dot screen, toner specks and streaks. Grit and contrast are adjustable.
- **Paste it up by hand:** drag any letter, strip, sticker or the price star. Click a piece to rotate or resize it. Duplicate, delete, or bring it to the front.
- **Stickers:** one-click extras like ALL AGES or NO COPS, or type your own.
- **Scatter headline:** throws the headline letters across the poster so you can place them yourself.
- **Save PNG:** exports the poster at about 2550 × 3300 px (US letter at 300 dpi).
- **Autosave:** your layout and text are kept in your browser between visits. Photos aren't saved.

### Keyboard

With a piece selected: arrow keys move, `[` `]` rotate, `-` `=` resize, Ctrl/⌘+D duplicate, Delete remove, Esc deselect. Hold Shift for bigger steps.

## Running it

No build step. Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server
```

Fonts come from Google Fonts and PNG export uses [html-to-image](https://github.com/bubkoo/html-to-image) from jsDelivr, so you need a connection the first time.

## Files

- `index.html`: the flyer maker
- `letters.html`: the cut-out letter generator on its own

Every letter is drawn in code (random typeface, paper stock, print texture and torn edge), so there are no image assets. Inspired by Arlan's [ransom note](https://www.arlan.me/vault/ransom-note) experiment.
