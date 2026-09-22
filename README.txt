Give me one Dollar - static 2-page site

FILES
  index.html   home page (Give $1 popup, socials)
  about.html   "About me" page with your photo and animations
  style.css    shared styles for both pages
  favicon.svg  browser tab icon

HOW TO UPLOAD
  Upload ALL four files to the root of your hosting (public_html / www / htdocs),
  or to GitHub Pages / Netlify / Cloudflare Pages / Vercel.
  Keep them in the same folder, otherwise styles and links will break.

WHAT'S NEW IN THIS VERSION
  - The "Wall of Fame" donors page and every link/button pointing to it were removed.
  - The avatar on the About page is now your uploaded photo: cropped to a circle,
    with a bold border and a spinning dashed ring around it, matching the site style.
    The photo is embedded directly inside about.html (as base64), so it's still a
    single self-contained file - no separate image file to keep track of.
  - Animations added throughout:
      - Home page: headline, text, stat chips and buttons fade/slide in on load.
      - About page: same on-load animation for the top section; your photo drops in
        and gently floats; the dashed ring around it slowly spins; further down,
        the story text, each skills card, the "Good to know" table and the bottom
        call-to-action fade up into view as you scroll to them.
  - All animations respect the "reduce motion" accessibility setting and turn off
    automatically for people who have that enabled on their device.

TO CHANGE CONTACTS OR WALLETS
  Open the file in a text editor and search for:
    TYwmZqW86RVbfEYAY68sTiVEzSx6WGzdqt   (USDT TRC20 address, index.html)
    boosty.to/igorkim/...                (Boosty support link, index.html)
    BUSD_BOSS                            (Telegram, both pages)
    igor-kim-79a013275                   (LinkedIn, both pages)

TO CHANGE THE PHOTO
  Easiest way: ask to have it replaced with a new uploaded photo.
  Manually: replace the base64 string inside the <img class="avatar" src="data:image/jpeg;base64,...">
  tag in about.html with a new one (any base64-image converter tool can generate it).

Fonts (Bricolage Grotesque, Caveat) load from Google Fonts, so the site needs internet to look exactly right.
