# Homepage handoff: mockup to WordPress

The client approved **Version 2**. That is the only file to build from.

- **Source:** `v2/index.html` (all HTML, CSS and JS in one file)
- **Live preview:** https://veneer-training.vercel.app/v2/
- **Ignore:** `v1/` (rejected direction) and the root `index.html` (comparison page)

## Do not carry these over

| What | Where in `v2/index.html` | Why |
|---|---|---|
| `<meta name="robots" content="noindex, nofollow">` | line 6 | Hides the page from Google. Must not reach the live site |
| The dark "Version 2 · see Version 1 · draft" bar | `<div class="draft">` | Mockup label only |
| `../assets/` paths | throughout | Point these at the WordPress media library instead |

## Assets to upload to the media library

All in the `assets/` folder, already compressed and web-ready.

| File | Used for |
|---|---|
| `hero-desktop.mp4` (3.1 MB) + `hero-desktop.jpg` | Banner video and its still frame, desktop |
| `hero-mobile.mp4` (1.3 MB) + `hero-mobile.jpg` | Banner video and its still frame, phones up to 820px |
| `logo-transparent.png` | Header and footer logo. Use this one, not the logo with the grey box |
| `patel.jpg` | Meet Dr. Tejas Patel |
| `podcast-1.jpg` | Free Resources, Podcast card |
| `free-resources.jpg` | Free Resources, Learning Lab card |
| `ada.webp` | ADA CERP badge in the footer |

The **testimonial videos and their posters are already on the live site**
(`wp-content/uploads/2024/05/` and `2026/08/`). The mockup loads them from there,
so nothing to upload.

## Fonts

- **Inter** (400–900): the whole page
- **Bodoni Moda** (500–700): only the "Your Path" graphic headings

Both load from Google Fonts in the `<head>`. The live site already uses Inter.

## Behaviour that needs the JavaScript

The `<script>` block at the bottom of the file has four parts. Keep all of them.

1. **Mobile menu:** opens and closes the ☰ menu on phones
2. **Hero video:** picks the desktop or mobile video by screen size, and runs the
   play/pause button. Visitors with "reduce motion" or battery saver on get a play
   button instead of a stuck still frame
3. **Course card hover:** the spotlight effect that follows the cursor
4. **Testimonial videos:** starting one pauses the others

## Links still to fill in

Every `href="#"` is a placeholder:

- **Enroll now** (Blueprint, No Prep), **View course** (3 Minute Crown Prep), **Join free**: need the Mighty Networks checkout links (Ami was sending updated ones)
- **Log in, More about Dr. Patel, Read more reviews, View program**: point to the matching live pages

Already live and correct: the **waitlist** buttons (`vvt.kit.com/5d0d976ed6`) and **Listen** (Spotify).

## Worth knowing

- **Blog section is hard-coded** to three posts. On WordPress it should pull the
  latest posts automatically so it doesn't go stale.
- **Sections in order:** Hero → Ready to Start → Your Path → Where Should You Start
  (six cards) → Meet Dr. Patel → Are You Struggling With → What Dentists Are Saying →
  Free Resources → Membership → Blog → Footer.
- **Breakpoints:** 1000px, 900px, 820px and 640px. Tested at 320, 360, 390, 414,
  768, 1024 and 1440px with no sideways scroll.
- The ADA CERP statement in the footer is **required word for word** wherever the
  ADA logo appears.

Questions: VJ.
