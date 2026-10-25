# Bloome review — 20 October 2026

Reviewed against [Shopify Theme Store requirements](https://shopify.dev/docs/storefronts/themes/store/requirements). This is a development audit, not Shopify approval. Those requirements include store testing and business obligations beyond an uploadable theme.

Latest review (0.2.3): added global fallback tokens and checked 164 section-child alignments across 40 library sections at four viewport widths. After the user confirmed the store, an actual Shopify upload exposed an invalid logo-width range (241 positions, over Shopify's 101-position limit) that local schema validation missed. Corrected it to 5px increments and added a packaging guard for all ranges. Shopify accepted the schema, and remote config readback confirmed all three complete schemes. The real development storefront loads Work Sans and balanced 30px desktop gutters. Collection/search/product/cart pages render without Liquid or JavaScript errors; product options, native add-to-cart and cart removal pass on the actual catalog. Admin editor UI verification requires an authenticated browser session. No live theme was published.

## Delivered improvements

| Area | Implementation and evidence |
| --- | --- |
| Upload structure | Native theme directories; required layout and Shopify content placeholders. ZIP entries use forward slashes with no parent folder. Packaging verifies every entry against its source SHA-256. |
| Editor customization | Branding, logo/favicon, native color schemes, body/heading font pickers, buttons, cards, layout, social links and motion settings. Most content sections expose spacing, width, typography, images and visibility controls. |
| Flexible content | JSON templates; header/footer section groups; addable sections; Custom Liquid section; product and featured-product details use reorderable blocks including app and Custom Liquid blocks. |
| Product purchase | Native product forms; separate option selectors with a full variant-selector fallback; unavailable combinations disable purchase; variant price, compare price, unit price, SKU and featured media updates; quantity and accelerated checkout. |
| Product media | Shared main/featured gallery renders image, video, external-video and model media. Quick view requests server-rendered product media with an image fallback. |
| Product services | Installment payment terms, gift recipient fields, pickup availability using Shopify variant endpoints, related/complementary recommendation setting. |
| Cart | Item quantities/removal, original/final prices, unit pricing, line/cart discounts, selling plan names, public item properties, notes, taxes-included notice and native accelerated checkout output. |
| Discovery | Nested navigation; collection/search filters and sorting; predictive suggestions with keyboard handling, cancellation and ordinary search fallback; paginated collections/search results. |
| Markets/accounts | Native country/language forms show configured choices; Shopify account component; Follow on Shop output where supported. |
| Content templates | Product, collection, collection list, search, blog/article, page, contact, FAQ, cart, password and gift card. Article comments paginate. Gift card includes QR/Wallet output. |

## Local verification

- Shopify AI Toolkit checked all 107 theme files: valid with warnings, no code errors. Nonblocking warnings concern CSS defined in shared components. Its documentation-cache refresh was denied by the sandbox; it successfully used cached Shopify schemas/resources.
- Actual Liquid source rendered locally with mock Shopify data. Tested 18 homepage sections and 40 section-library entries at 1440px and 390px; no horizontal overflow or JavaScript page errors.
- Browser tests exercised global/section styling, mobile overrides, variant prices/SKU, separate options, sold-out and nonexistent combinations, tab keyboard handling, editor selection/reconnection/reorder, carousel, comparison control, FAQ and dialogs.
- Mock commerce tests exercised quick-add variants, bundle limits, duplicate variant aggregation, stock errors and retry, totals, cart redirect and countdown expiry.
- Predictive-search tests exercised request parameters, results, arrow keys, Escape/focus, failed requests and component reconnection.
- Default color-scheme text/button contrast tested at least 4.5:1. This is not a complete accessibility certification.

Local rendering uses a substitute Liquid engine and mocked data. It cannot certify Shopify editor behavior, real forms, inventory, payments, localization redirects, or account components.

## Required before production or Theme Store submission

| Check | What remains |
| --- | --- |
| Native editor | Upload the reviewed ZIP as an unpublished theme; test saving, adding/reordering sections and product blocks, app blocks and settings on Shopify. |
| Real commerce | Test real variant images/media, stock, gift recipient delivery, pickup locations, recommendations, subscriptions, discounts, taxes, installment messaging and accelerated checkout. |
| Search/Markets/accounts | Enable actual filters, configure markets/languages, test predictive results, account component, Follow on Shop and localization redirects. |
| Performance/accessibility | Run Shopify-required Lighthouse home/product/collection tests with real content on mobile/desktop; meet average performance ≥60 and accessibility ≥90. Complete keyboard/screen-reader and contrast review with configured imagery/colors. |
| Compatibility | Complete Safari/iOS, Firefox, Chrome, Edge and real device checks. Local browser automation used Edge. |
| Merchandising | Replace demonstration illustrations/copy with owned product/campaign imagery and accurate ingredients, usage, claims, prices and policies. Product selections currently need your catalog. |
| Theme Store operations | Provide a realistic demo store, actual theme documentation/support URLs, release notes and support arrangements. Generic Shopify help links in metadata are temporary. Review originality and every submission criterion with Shopify. |

No Shopify store address or authenticated development connection was supplied. These live checks remain pending; this package is not represented as Theme Store approved or fully production verified.
