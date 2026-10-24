# Shanky's Whip on Shopify with the AccelPay app (sales demo)

**Private sales demo.** This site uses Shanky's Whip's name, marks, product imagery and copy
(from shankyswhip.com) to show their Shopify store with the AccelPay Shopify app installed. It is
not affiliated with or endorsed by Shanky's Whip, it is not a store, and no order is ever placed or
charged. Gopuff, Shopify and ReserveBar marks belong to their owners. Keep the link unlisted;
share it 1:1 only.

Live: https://noshiftsherlock.github.io/shankyswhip-accelpay-demo/

## The pitch it shows

shankyswhip.com runs on Shopify (confirmed 2026-10-24: `window.Shopify` present, `/products.json`
serves the catalog); today the Shopify cart hands alcohol orders to the Bottle Nexus network. The
demo keeps the Shopify store, the native Shopify cart drawer and the Shopify one-page checkout,
with the AccelPay Shopify app taking over payments, taxes and routing to licensed retailers. No
third-party cart; orders and customers stay in Shopify. Express checkout (Shop Pay, Apple Pay,
Google Pay) at the top of checkout, in the cart drawer and on the product page.

| Page | What it shows |
| --- | --- |
| `index.html` | Home, range, Meet Shanky, "How this works", ReserveBar note, AccelPay panel, reordering note |
| `product.html?p=<handle>` | Product pages; the 750 ml is the default |
| `checkout.html` | Shopify one-page checkout: Gopuff delivery in California ZIPs, real in-state retailers for the 750 ml |

Try ZIP 90046 (Los Angeles: Gopuff plus CA retailers), 77006 (Houston, Spec's), 10009 (New York),
33301 (Fort Lauderdale), 60606 (Chicago: no listing yet, routes "connected at launch").

## Real vs illustrative

Real (2026-10-24):
- Products, images, copy and prices: shankyswhip.com `/products.json` (Giant 1.75 L sold out).
- Retailers, cities: active, in-stock listings for the 750 ml (UPC 00810035510111) in the
  ReserveBar / AccelPay retailer catalog. The demo uses a sample of 34 (every non-Texas retailer,
  two Spec's per big Texas metro) out of 217 in stock. Bottle Nexus's own three retailers are
  excluded on purpose.
- Gopuff: 95 California locations carry Shanky's Whip in a live Gopuff check on 2026-10-24; the
  demo uses the delivery ZIPs of the 90 that publish them.
- Shanky's Whip on ReserveBar.com.

Illustrative:
- Shipping ($9.99, free over $70 as today), Gopuff fee ($4.99), 8% tax, payment, confirmation.
- Golden Ostrich, cans, nips and minis have no retailer listing today; they route to "a licensed
  retailer in <state>, connected at launch".

Built from `data.js` and a shared `app.js`. GitHub Pages serves `main`; bump `?v=` on change.
