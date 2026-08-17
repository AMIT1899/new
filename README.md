# NORTHROW — Static Menswear E-commerce Store

GitHub Pages-ready menswear storefront built with HTML, CSS and Vanilla JavaScript only. No backend, database, framework or build step is required.

## Main files
- `index.html` — homepage
- `shop.html` — searchable/filterable catalog
- `product.html` — product detail, size pricing, pincode, add-to-cart and Buy Now
- `cart.html` — LocalStorage cart, coupons and totals
- `checkout.html` — validated COD checkout
- `wishlist.html`, `orders.html`, `account.html`, `order-success.html`
- `js/core.js` — store config, 36-product catalog, pricing, LocalStorage, header/search/wishlist logic
- `css/bundle.css` — storefront styles
- `assets/images/brand/product-fallback.svg` — local placeholder image

## Edit store details
Edit `STORE_CONFIG` at the top of `js/core.js`.

## Edit coupons
Edit `COUPONS` at the top of `js/core.js`.

## Edit products
Edit the product rows near the top of `js/core.js`. Product objects, sizes, stock and prices are generated from those rows. Replace `images` paths when you upload real photography.

## Deployment
The existing `.github/workflows/static.yml` workflow is preserved. Pushes to `main` can continue deploying this repository through GitHub Pages.

## Limitations
This static build cannot provide real card/UPI settlement, secure authentication, cross-device orders, server-side inventory, courier tracking or transactional SMS/email. COD creates a browser-local order record only until a backend is connected.