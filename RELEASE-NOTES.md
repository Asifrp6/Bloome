# Bloome 0.3.4

- Header can be transparent and sit over the homepage hero. Sticky header fills in with the page background after scroll.
- New header design places the menu on the left, the logo in the center, and search, account, and cart on the right.

# Bloome 0.3.3

- The header has four designs: classic, centered logo, stacked menu, and minimal.
- Mega menu opens a wide panel for menu items that have child links. Turning it off uses a short dropdown.

# Bloome 0.3.2

- Homepage hero, concern finder, and ingredient lab use the stand-in photographs as the layout, with quieter type and working tabs.

# Bloome 0.3.1

- Section headings use the full content width, so words such as “ingredients” and “concern” stay intact.

# Bloome 0.3.0

- Homepage now opens with a concern finder, then categories, then an ingredient lab, so shoppers can start from how their skin feels.
- Concern finder swaps a large image, explanation, and collection link from a numbered rail. Arrow keys and the theme editor move the selection together.
- Ingredient lab uses a selectable mosaic and a detail panel. Each ingredient can link to its own collection.

# Bloome 0.2.9

- Product and bundle variant lists now include up to 250 variants, and option selectors include up to 250 values.
- Customers can choose a one-time purchase or a selling plan on the product form. The cart still shows the selected plan.
- Impossible option combinations clear the selected variant and mark the product unavailable.
- Swatch clicks keep the compare price before the sale price and follow the currency-code setting.
- Shop by price formats zero-decimal and three-decimal currencies correctly.
- Shared muted text, search pagination, and search filter checkboxes use global styles so they render on every page.
- The header fallback menu links to catalog, collections, and search when no menu is selected.

# Bloome 0.2.8

- Made standard product cards more compact with square images, 12px corners, tighter information spacing and smaller quick-add buttons.
- Improved badge readability and title wrapping. Image shape and corner radius remain editable in Theme settings.
- Verified square image dimensions and rounded corners in the Shopify development preview at 529px; existing quick-add tests pass.

# Bloome 0.2.7

- Content with video now supports thumbnail-driven product previews: left thumbnail selection updates the large right image, whose link opens the corresponding product.
- Added selected-state styling, keyboard selection, editor block-selection handling and an option to retain the original video/image behavior.
- Verified switching in Shopify's development preview and matching product-link navigation in local browser tests.

# Bloome 0.2.6

- Redesigned Shop by price with rounded image cards, category descriptions, prominent price limits and outlined shop buttons.
- Added card colors/radius, mobile columns, and per-card descriptions/button labels. Images can fall back to collection imagery.
- Verified card links, responsive layout and real Shopify filtering: the maximum-price query is applied and displayed products respect the limit.

# Bloome 0.2.5

- Redesigned Look tabs with vertical navigation, a central portrait, adjacent image previews and synchronized descriptive text/shop links.
- Added five default looks, portrait-height and preview controls, entry transitions and reduced-motion support.
- Added vertical keyboard navigation and responsive tab orientation. Verified selection, preview clicks, focus and mobile bounds in the Shopify development preview.

# Bloome 0.2.4

- Added Rounded product edit: rounded product cards, sale/new badges, prices, native swatches and round purchase/quick-view actions.
- Added product/collection selection, desktop/mobile columns and card styling controls.
- Swatches update the image, price and product link; quick view retains the chosen variant.
- Verified interactions locally and actual product-section rendering on Shopify's development preview.

# Bloome 0.2.3

- Added layout, font and color fallbacks when saved global settings are missing or blank, preventing an invalid section grid and one-sided blank gutters.
- Kept fallback CSS at lower specificity so saved merchant settings still take precedence in the native layout's stylesheet order.
- Removed duplicated color-scheme resolution and isolated the native scheme editor in its own settings category.
- Checked balanced alignment across 40 section-library entries at 1920, 1294, 760 and 390px, including a missing-settings fixture. Existing editor-control, slider, predictive search and mock-commerce checks pass.
- Fixed the native Shopify upload failure: logo width had 241 range positions, exceeding the 101-position limit. It now uses 5px increments. Packaging checks every range control for this constraint.
- Following store approval, uploaded to a development theme. Shopify accepted the schema and stored all three schemes. Real collection/search/product/cart rendering, option selection, add-to-cart and cart removal passed. The authenticated admin color-scheme panel still requires a browser login.

# Bloome 0.2.2

- Completed color-scheme values in current settings and the Bloome preset to match the schema definitions.
- Added explicit scheme defaults to all 52 section color-scheme selectors and initialized template selections.
- Corrected section rendering to accept Shopify's selected color-scheme object, with compatibility for stored scheme IDs.
- Verified object-based color rendering locally. Native Shopify editor verification remains pending.

# Bloome 0.2.1

- Replaced the initial home-page banner with a full-width image slideshow, overlaid text and thumbnail navigation.
- Added separate desktop/mobile images and height controls, editable overlay colors/opacity and optional navigation arrows.
- Added keyboard navigation, offscreen slide focus protection, editor block selection and active-slide preservation on resize.
- Removed empty heading spacing and reset main-content/header spacing above the first banner.
- Improved header fit on screens narrower than 360px.
- Local tests verified zero header-to-banner gap at 1440, 760, 390 and 246px, with no horizontal page overflow. Real Shopify editor/store testing remains pending.
