# Livotec Philippines: consumer site

Static site for households and direct buyers. No build step, no backend. Deploy the whole folder to GitHub Pages (keep `.nojekyll`) or Netlify.

## Conversion
No e-commerce. The form at the bottom ("Book a pre-installation survey" or "Ask about buying") opens a pre-filled email to info@iontech.com.ph. Survey requests include the full pre-installation checklist (outlet, water supply, drain, water source, access, sink, existing purifier or filtration) and the customer's agreement to the installation terms.

## Where to edit
All in `index.html`, first `<script>` block ("SITE DATA: edit here"):
- `PRODUCTS`: names, SRPs, specs, badges, filter tags. Source: "Product Details" Google Sheet.
- `SERIES`: series taglines and descriptions.
- `FAQ`: questions and answers.
- `CONTACT`: lead email.

The savings calculator is the original `script.js` in the last `<script>` block; every model is marked `filtersConfirmed: true`. Keep its `LOCAL_PRODUCTS` prices in sync with `PRODUCTS` when an SRP changes.
