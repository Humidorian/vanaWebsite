# Vana Aishwarya Green Enterprises — Website

Corporate website for **Vana Aishwarya Green Enterprises** — a **tribal-owned, women-led ST (Scheduled Tribe) solar EPC company** of the Koya community from the Eastern Ghats (registered at Mothugudem on the banks of the river Sileru). Built with the same design as `dev/` (Aeterna Energy) but populated with this company's data. Plain HTML + CSS + vanilla JS, single file.

**Core message:** the copy deliberately leads with the tribal-owned (ST, Koya) and women-led (promoted by Ms Veena Soyam) identity, and pushes its business ramifications — easier/priority-sector loans, concessional funding, and ESG value for corporate partners.

## Files
- `index.html` — the entire site (styles & script inline). Everything editable lives
  in the `SITE` object at the top of the `<script>` block (`SITE DATA` banner).
- `assets/` — the 5 solar photographs (hero, team, residential, commercial, utility).
- `vana.png` — the official company logo (used as the brand image in the nav and
  footer via `.brand-logo`; horizontal lockup with emblem + wordmark).
- `dev/` — the original Aeterna reference design this site was derived from.

## Content source
The data comes from the uploaded profile `Vana-Aishwarya-Profile.docx` (source text:
`scratch/vana.txt`). Company, mentors, CEO (Ravikumar N), Energy-as-a-Service
model, and supplier names all come from that document.

## PLACEHOLDERS TO REPLACE (not in the source doc)
- **Contact** — `SITE.contact.email`, `.phone`, `.phoneHref` are dummy values
  (`contact@vanaaishwarya.in`, `+91 00000 00000`). Set the real ones.
- **Stats** (`SITE.stats`) — the four counter figures are indicative placeholders;
  update with real numbers (MW installed, projects, etc.).
- **Domain** — `SITE.meta.url` and the footer link use `vanaaishwarya.in`.
- Two mentors (Dr Herve Laberthe, S Ravi) have no LinkedIn URL in the source, so
  their LinkedIn links are omitted (the script hides the link when `linkedin` is empty).

## Editing
Change a value in `SITE` and it updates everywhere it appears (brand, contact,
mentors, FAQ, calculator, stats). The visual identity is deliberately distinct from the
`dev/` template: **Fraunces** serif display headings (earthy/organic, not the
template's geometric sans) + green pill-shaped primary buttons, on a palette derived
from the logo (`vana.png`): deep forest green (`--navy`/`--navy-2`), leaf
green (`--green`), gold/sun accent (`--amber`), teal (`--teal`), and red
(`--red`, used for small leadership chips echoing the logo's red wordmark). Tweak these
in the `:root` variables in the `<style>`
block. The enquiry form opens a pre-filled `mailto:` — swap for Netlify Forms /
Formspree to actually capture submissions.
