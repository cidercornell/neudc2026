# NEUDC 2026 Conference Website

Static website for the **Northeastern Universities Development Consortium (NEUDC) 2026** conference, hosted by Cornell University and CIDER.

## Contents

- **Home** — Event overview, key dates, links to register and submit papers  
- **Program** — Conference program (full program in fall 2026), link to Conference Maker for paper submissions  
- **Logistics** — Venue, travel, hotels, parking  
- **Register** — Fees, travel grants, visa letters, link to CVENT for registration and payment  

## Running locally

Open `index.html` in a browser, or serve the folder with any static server, e.g.:

```bash
# Python 3
python3 -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Before going live

1. **CVENT link**  
   Registration buttons currently point to `#`. When the CVENT event URL is ready (e.g. `https://cvent.me/...`), replace it in:
   - `index.html` — hero “Register via CVENT →” link  
   - `register.html` — “Register and pay via CVENT →” link  

   Search for `href="#"` near “CVENT” to find both spots.

2. **CIDER link**  
   Have the main CIDER site add a link to this site (e.g. “NEUDC 2026” or under Conferences) so the site is (i) linked from the broader CIDER site.

3. **Venue**  
   When the building is confirmed, update the “Conference Venue” section in `logistics.html` and add a map link if available.

## Content source

The copy is derived from the Markdown files in this repo (`home.md`, `program.md`, `logistics.md`, `register.md`). For future edits, update either the HTML directly or the `.md` files and then sync into the HTML.

## Contact

Questions about the conference: [tmt1@cornell.edu](mailto:tmt1@cornell.edu)
