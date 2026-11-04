# STEPNOVA project guide

The app is a React 19 / TypeScript storefront built with TanStack Start and deployed through Netlify's Vite adapter.

- `src/routes/index.tsx` contains the storefront, its three-product catalog, category/search/sort interactions, temporary bag and wishlist, product-size dialog, and WhatsApp order links.
- `src/routes/__root.tsx` supplies the document shell and finished site/social metadata.
- `src/styles.css` defines the responsive design with desktop and mobile breakpoints. Mobile product cards scroll horizontally and the bottom navigation stays fixed.
- `public/img/` contains custom product photography served through Netlify Image CDN.
- `netlify.toml` configures the build and local platform proxy.

Keep blue #1e5bd0, yellow, white and green as the principal marketplace colours. Use Manrope for headings and DM Sans for body text. Preserve accessible button labels, keyboard focus outlines, readable product imagery, reduced-motion support and responsive horizontal cards.

Order links go to the specified WhatsApp business number. The site does not collect payments or claim completed transactions. Bag, wishlist and selected sizes are ephemeral UI state; persistence was not requested. If persistent records are added, use Netlify Database and consult the platform database skills. Do not use browser storage as a persistent database.

Build and validation run in the platform pipeline. Do not commit build artifacts or expose credentials. Update root metadata and documentation when the product changes.
