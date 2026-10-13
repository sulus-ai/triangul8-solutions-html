# Solutions hub (index)

**CRM page path:** `/content-solutions`  
**CRM page id (reference only):** `211`  
**Original zip file:** see master README

## Before you paste anything
In the CRM page editor for `/content-solutions`:
1. Use **one** section that holds all Custom HTML blocks.
2. Set that section to:
   - **Padding top:** None
   - **Padding bottom:** None
   - **Container / width:** Full (not App container)
3. Hide the site’s global header/footer for this page if your theme has that toggle (these HTML blocks include their own nav + footer).
4. Delete old Custom HTML blocks on this page first (or clear their contents) so you are not stacking duplicates.

## Paste order (one Custom HTML block per file)
1. `00-crm-shell-fix.html`
2. `00b-solx-hub-css.html`
3. `01-css-base.html`
4. `02a-css-brand-part1.html`
5. `02b-css-brand-part2.html`
6. `03a-css-nav-mobile-part1.html`
7. `03b-css-nav-mobile-part2.html`
8. `03c-css-nav-mobile-part3.html`
9. `04-nav.html`
10. `05-body.html`
11. `06-form-scripts.html`
12. `07-footer.html`

## Rules
- Paste **one file = one block**, in the order above.
- Do **not** combine files into one giant paste.
- Every CSS file is a complete `<style>...</style>` — never cut mid-tag.
- After all blocks are pasted: save, publish, deploy, then hard-refresh the live URL.
