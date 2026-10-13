# Triangul8 /content-solutions — CRM paste HTML

## Download
Use the zip: `triangul8-solutions-ready.zip`

## Important (CRM asset reality)
This Triangul8 CRM site does **not** have separate uploadable `brand.css` / `brand.js` site files.
The original zip referenced `../assets/css/brand.css` and `../assets/js/brand.js` — those only existed in the local zip folder.

What CRM *does* already provide on every published page:
- Fonts (`/_fonts/*`)
- Analytics (GTM / gtag)
- Pins widget
- Media library images under `/api/media/file/...`

Global header/footer slots are **hidden** (`display:none`), so each page must include its own nav + footer HTML (already in these files).

## Paste steps
1. CRM → Triangul8 Main Site → Pages
2. Open the matching path
3. Delete all Custom HTML blocks
4. Add one Custom HTML block
5. Paste the full `.html` file contents
6. Save → Publish
7. Deploy once after all 8

## File → path map
| File | CRM path |
|------|----------|
| content-solutions.html | /content-solutions |
| persona-engine.html | /content-solutions/persona-engine |
| seo-aeo-geo.html | /content-solutions/seo-aeo-geo |
| website-content.html | /content-solutions/website-content |
| social-media.html | /content-solutions/social-media |
| paid-media.html | /content-solutions/paid-media |
| email-marketing.html | /content-solutions/email-marketing |
| marketing-automation.html | /content-solutions/marketing-automation |

## CRM media referenced
- `/api/media/file/triangul8-logo-light-bg-98f5acd8999db8d2.webp?prefix=media`
- `/api/media/file/triangul8-logo-dark-bg-8243db5dde19e5fe.webp?prefix=media`

## If one block rejects a large paste
Split into 7 blocks from the agent folder `/tmp/solutions-crm/pages/<id>/blocks/` in this exact order:
css1 → css2 → css3 → nav → body → form → footer
Never cut mid-tag.
