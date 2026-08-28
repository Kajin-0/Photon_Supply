# Photon Supply Co.

Minimal static storefront prototype for the initial Photon Supply Co. fiber-cleaning line.

## Initial products

- **PSC-FCE-25** — Fiber Cleaning Essentials — 2.5 mm — **$129.95**
  - AFL 8500-05-0009MZ Mini-500 (SC/ST/FC)
  - Chemtronics CP400, 50 individually wrapped wipes

- **PSC-FCE-125** — Fiber Cleaning Essentials — 1.25 mm — **$129.95**
  - AFL 8500-05-0010MZ Mini-500 (LC/MU)
  - Chemtronics CP400, 50 individually wrapped wipes

- **PSC-UFC** — Universal Fiber Cleaning Kit — **$199.95**
  - AFL 8500-05-0009MZ Mini-500 (SC/ST/FC)
  - AFL 8500-05-0010MZ Mini-500 (LC/MU)
  - Chemtronics CP400, 50 individually wrapped wipes

- **PSC-MPO** — MPO/MTP Cleaning Kit — **$134.95**
  - AFL 8500-05-0030MZ One-Click MPO/MTP cleaner
  - Chemtronics CP400, 50 individually wrapped wipes

## Checkout integration

The page is intentionally payment-provider agnostic.

At the bottom of `index.html`, populate the four URLs in:

```js
const CHECKOUT_LINKS = {
  kit25: "",
  kit125: "",
  universal: "",
  mpo: ""
};
```

These can point to FOC-owned Stripe Payment Links, PayPal/Square links, FOC direct checkout URLs, or a future reseller storefront. Once a URL is populated, that product's **Buy now** button automatically activates.

## Product imagery

The prototype uses externally hosted public product imagery so the repository can stay lightweight while the FOC reseller structure is being finalized. Before commercial launch, replace external imagery with manufacturer/distributor assets that Photon Supply Co. has explicit permission to use.

## Deployment

The site is a single static `index.html` file and can be hosted directly with GitHub Pages or any static web host.
