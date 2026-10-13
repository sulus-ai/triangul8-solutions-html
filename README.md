# Triangul8 content-solutions — CRM paste pack (HTML only)

## Read this first
This pack is **HTML files + instructions only**.

- Paste these yourself in the CRM site editor.
- Do **not** ask agents to edit CRM pages via API.
- Goal: each live page looks like the original zip design.

Download zip: `triangul8_crm_paste_pack.zip`

## Page map (which folder → which CRM page)

| Folder | Paste into CRM page | Live path | Matches original zip |
|--------|---------------------|-----------|----------------------|
| `01-content-solutions/` | Content Solutions (hub) | `/content-solutions` | `index.html` |
| `02-persona-engine/` | Persona Engine | `/content-solutions/persona-engine` | `persona-engine.html` |
| `03-seo-aeo-geo/` | SEO / AEO / GEO | `/content-solutions/seo-aeo-geo` | `aeo-seo.html` |
| `04-website-content/` | Website Content | `/content-solutions/website-content` | `on-page-content.html` |
| `05-social-media/` | Social Media | `/content-solutions/social-media` | `social.html` |
| `06-paid-media/` | Paid Media | `/content-solutions/paid-media` | `paid-media.html` |
| `07-email-marketing/` | Email Marketing | `/content-solutions/email-marketing` | `email.html` |
| `08-marketing-automation/` | Marketing Automation | `/content-solutions/marketing-automation` | `marketing-automation.html` |

## CRM page setup (do this once per page, before pasting HTML)

For **each** page above, in the CRM editor:

1. Open the page.
2. On the main section that will hold the embeds:
   - Padding top = **None**
   - Padding bottom = **None**
   - Container = **Full** (not the default app container)
3. Turn **off / hide** the global site header & footer for that page (the paste includes branded nav + footer).
4. Remove previous Custom HTML blocks for the old rebuild so you start clean.

If you skip step 2, you will get white padding around the whole page and a broken mega menu.

## How to paste (every page)

1. Open the matching folder (example: `01-content-solutions/`).
2. Open that folder’s `README.md` — it lists the exact paste order.
3. For each numbered `.html` file in order:
   - Add **one** Custom HTML / Embed block
   - Paste the **entire** file contents
   - Save
4. Publish the page, deploy the site, hard-refresh the live URL.

### Block roles (typical order)
- `00-crm-shell-fix.html` — kills CRM padding / fixes mega menu overflow (**required first**)
- `00b-solx-hub-css.html` — hub card styles (**only on** `01-content-solutions`)
- `01` / `02a` / `02b` / `03a`… — CSS chunks (complete `<style>` tags)
- `04-nav.html` — sticky nav + mega menu markup
- `05…-body…` — page body (persona-engine is split into 05a–05d)
- `06-form-scripts.html` — CRM form iframe + mobile burger JS
- `07-footer.html` — footer

## Hard rules
1. **Never** paste one giant combined HTML file into a single block (CRM truncates; you will see CSS as text).
2. **Never** cut a file in the middle of a `<style>` tag.
3. Keep files in filename order.
4. Logos/media already use CRM `/api/media/file/...` URLs.

## After paste — quick visual check
- No white frame around the whole page
- Nav mega menus open full-width and opaque
- Body sections match the original zip styling (cards, icons, spacing)
