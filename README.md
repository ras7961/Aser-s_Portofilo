# Gugo Portfolio

A one-page personal portfolio with a hand-drawn ink animation: a developer at his desk, standing on a map of Africa with Ethiopia highlighted, who turns around to say hi.

## Run it

It is a single file with no build step.

1. Save the page as `index.html`.
2. Open it in a browser, or upload it to any static host (GitHub Pages, Netlify, Vercel).

It needs an internet connection to load the Google Fonts (Bricolage Grotesque, Schibsted Grotesk, IBM Plex Mono, Caveat). Everything else is inline.

## Edit your content

All content lives in three lists at the top of the `<script>` section:

- `PROJECTS`: copy a block, paste it at the top, and change the text. Add a `link` to show a "View project" link.
- `SKILLS`: your skills, grouped. These fill the skills cards.
- `CONTACT`: your email, GitHub and LinkedIn. The message form on the page opens an email to the address in `CONTACT.email`.

## Customize the look

- **Colors and fonts:** the tokens at the top of the `<style>` section (`:root`). There is a light and a dark version.
- **Speech bubble text:** search for `Hi, I'm` in the `overlay` function.
- **Animation speed:** the `frame` function near the bottom of the script (frame rate and speed).
- **Always start in light theme:** add `document.documentElement.setAttribute("data-theme", "light");` at the top of the script.

## Built with

HTML, CSS and plain JavaScript. The animation is drawn with the 2D canvas, redrawn 12 times per second for the frame-by-frame look. It respects the `prefers-reduced-motion` setting by showing a still frame.
