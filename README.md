# Current Lekka website

The one-page product site for **Current Lekka** (కరెంట్ లెక్క), an Android app that reads a photo of a Telangana electricity bill slip and explains it aloud in Telugu, Hindi or English, on the phone.

It is the website for the app's entry to the Telangana Innovation Startup Challenge (TISC 2026), Challenge #13, and is published with GitHub Pages at <https://current-lekka.pages.dev/>.

## Files

| Path | What it is |
|---|---|
| `index.html` | The page |
| `styles.css` | All styles |
| `404.html` | Not-found page. Its styles are inline and its links start with `/current-lekka/`, because GitHub Pages serves it at any path depth |
| `assets/mark.svg`, `assets/wordmark.svg` | The Concept 2 "Bill slip" logo, copied unchanged from the app project |
| `assets/favicon.svg`, `favicon-32.png`, `apple-touch-icon.png` | Icons made from the mark |
| `assets/og-image.png` | 1200×630 share image made from the wordmark |
| `assets/shot-*.webp` | App screenshots from the Android test phone, showing sample data only |

There is no build step and no JavaScript. Fonts (Roboto Flex, Noto Sans Telugu) load from Google Fonts.

## Editing

- Edit `index.html` and `styles.css` directly, then open `index.html` in a browser to check.
- Keep every link to a page asset relative (`assets/...`, `styles.css`) so the site works under `/current-lekka/`. The only absolute URLs are the Open Graph `og:url` and `og:image` (link-preview crawlers need them), the download link, and the links in `404.html`.
- Colours are defined once at the top of `styles.css`: indigo `#3A2FD0` and saffron `#FFB21A`. Saffron is an accent only; it is too light for text on white.
- Screenshots must show sample data only. Never add a photo or screenshot of a real bill or a real person's account. Resize new screenshots to at most 900 px tall, and keep the whole site under 3 MB.
- Telugu text needs a `lang="te"` attribute so it gets the Telugu font and is read correctly by screen readers.
- `_review/` holds local review screenshots and is listed in `.gitignore`. Don't publish it.

## Claims

The page states only what has been measured or built. Before adding a claim (accuracy, features, availability), check that it holds for the released build.

## Disclaimer

Not affiliated with TGSPDCL, TGNPDCL or the Government of Telangana. Screenshots use sample data.
