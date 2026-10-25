# Bloome beauty theme

A modern skincare and makeup theme with ivory, warm peach, dusty rose and plum. Includes editable campaign hero, featured collection, makeup story, brand philosophy, newsletter, navigation, product, collection and cart layouts.

## Preview

Open preview.html in a browser. This visual preview uses sample illustrations. Cart, search, newsletter submission and checkout require Shopify.

## Install

1. In Shopify admin, open Online Store > Themes and upload **bloome-theme.zip** using the theme import option. All future theme updates overwrite this same ZIP filename.
2. Open Customize on the uploaded theme.
3. In Beauty product edit, select your actual featured collection.
4. Open the first **Slideshow** section and upload a desktop image for each Slide block. Optional mobile images let you use a portrait crop on phones. The decorative Bloome illustrations are placeholders until you select your campaign images.
5. Link the makeup button to your makeup collection. Set header and footer menus, and update the wordmark in both sections.
6. Add your products, variants, policies and store details. Newsletter uses Shopify's native customer form.
7. Preview product choices, cart quantities, checkout, newsletter and mobile navigation in your Shopify store before publishing.

Sample cards are labeled and replaced when you select a populated collection. No sample inventory or reviews have been created.

## Where to customize

In **Content with video**, leave **Enable product image selection** checked for linked product previews. Each Product block selects the product and an optional image override. Clicking its left thumbnail changes the large right image; clicking the large image opens that product. Blocks without a selected product show an unlinked preview. Turn the option off to use the section's original video/image mode.

**Shop by price** uses four image cards with descriptions, price limits and rounded shop buttons. Edit each Budget block to choose its collection/image, maximum price and button label. Images fall back to the collection's featured image. Both the image and button apply the same maximum-price filter. Price amounts use the displayed currency; enable the Price filter in Shopify Search & Discovery for destination collections. The section includes card colors, corner radius and mobile-column controls.

The **Look tabs** section includes the vertical look selector and portrait layout demonstrated in your video. Add/reorder Look blocks, then choose each block's image, heading, description and shop link. Portrait height and adjacent image previews are section settings. Tabs switch the image and copy together; preview images also select the adjacent look. Mobile uses a horizontal tab row. The reference portraits are not included.

For the rounded makeup cards, use **Add section → Rounded product edit** (also included on the home page). Select individual Products or a Collection. Cards use real product images, prices, sale information and native shade/color swatches where available. Products tagged `new` receive a New badge. Single-variant products use add-to-cart; products with options open quick view. Card colors, corner radius, columns, spacing and swatch visibility are editable. Reference photography is not included.

- Open **Theme settings** (the gear icon) for branding/logo, color schemes, fonts, buttons, layout, product cards, social links and motion.
- Click a content section for its content and design controls. Most sections include color scheme, width, alignment, optional typography overrides, spacing and desktop/mobile visibility. Header/footer have their own controls.
- In **Slideshow**, set desktop/mobile height, thumbnails and arrow visibility. Each Slide block controls its image, mobile image, text, button, foreground/background colors and image overlay. The default home-page slideshow starts immediately below the header with zero top padding; desktop thumbnails sit on the right and mobile thumbnails sit along the bottom.
- Use **Add section** to browse the section library or add Custom Liquid. Drag sections to reorder them.
- Switch the editor page selector to **Products > Default product**. Drag the Vendor, Title, Price, SKU, Purchase options and Description blocks; add Information, Custom Liquid or app blocks as needed. Featured product sections use the same editable detail blocks.
- Select actual products/collections in commerce sections. Empty demonstration sections do not create store inventory.
- Configure languages, countries, pickup, payment methods and filters in Shopify admin. Theme controls display the resources and services you enable there.

## Verification

Shopify AI Toolkit validated all 107 theme files with no code errors and nonblocking shared-CSS warnings. Browser checks passed at 1440px and 390px. See [BLOOME-AUDIT.md](BLOOME-AUDIT.md) for evidence and the remaining Shopify tests. A live store has not been connected, so native editor saving, checkout and real form submission remain unverified.

## Expanded section library

The Bloome homepage contains 18 curated sections. All additional sections are available through Add section in the theme editor; they do not need to be placed on one long homepage.

Open preview-sections.html to inspect the sections individually. Assign page.section-library to a Shopify page to explore an additional preassembled layout. FAQ and contact page templates are included. See BLOOME-SECTIONS.md for the Bloome section catalog.

Configure collection tabs, gift collections, featured products, product hotspots, bundle products and shoppable videos with your store resources. Add collection filters in Shopify Search & Discovery. Product finder product types and tags must match the catalog and enabled filters. Add ingredients, usage and shipping copy in the product section information blocks; empty blocks stay hidden. Product recommendations are supplied by Shopify.

The footer group includes a promotion panel (automatic opening off by default) and the quick-add dialog. Enter only existing discount codes in the promotion panel. Configure header navigation using nested Shopify menus, and set its optional promotion image.

Local verification covered the section picker at desktop and mobile widths, tabs and keyboard navigation, before/after slider, slideshow, FAQ, dialog dismissal, nested menu, countdown expiry, and mocked quick-add/bundle commerce requests. Final purchasing and customer-form checks still need the connected store.
