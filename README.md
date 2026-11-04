# STEPNOVA

A mobile-first premium footwear storefront with Hindi accents, a Freedom Sale promotion, and a curated three-product luxury collection. Customers can search, filter and sort products, inspect sizes, save favourites for their current visit, and order directly through WhatsApp.

STEPNOVA remains the main brand, with a header credit to Mohammad Ayan, a homepage founder message celebrating Agra, and a 2026 footer attribution.

Built with React 19, TanStack Start, TypeScript, CSS, Lucide icons, and Netlify Image CDN. Custom footwear images are stored in `public/img`.

## Local development

Use Node.js 22.13+ and pnpm. Install dependencies with `pnpm install`, then run `netlify dev --port 8889` to include Netlify platform features. The deployment pipeline runs the production build automatically.

The bag and wishlist are temporary interface state and reset on refresh. The initial bag displays the AirVolt Pro and Classic Loom Loafer. Ordering and customer assistance use WhatsApp; no payment is collected by this site.

Buy Now opens a minimal white confirmation screen with a subtle green tick, selected products and sizes, pricing, and a WhatsApp handoff. Continue Shopping returns to the collection. The confirmation is temporary selection state; availability and delivery are confirmed with the team on WhatsApp, and no payment or transaction is completed on the site.
