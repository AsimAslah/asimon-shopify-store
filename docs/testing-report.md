# ASIMON storefront testing report

## Automated validation

- Command: `shopify theme check`
- Scope: Liquid, JSON templates, schema references, and theme structure
- Current baseline findings: Horizon reports two `UnknownFilter` errors for Shopify's `applicable_disclosures` filter, one header settings-count warning, and existing divider documentation warnings. These are upstream theme compatibility findings and are not introduced by the ASIMON storefront configuration.

## Verified storefront paths

- Homepage hero renders ASIMON desktop and mobile media references.
- Hero copy and call-to-action are merchant editable.
- Hero call-to-action targets the New Arrivals collection.
- Homepage product grid targets the New Arrivals collection.
- Product cards render image, title, current price, compare-at price, and product links.
- Product template includes media gallery, variants, quantity selector, add-to-cart controls, description, and recommendations.
- Cart template uses Shopify's native cart implementation and New Arrivals recommendations.
- Header includes search, account, localization, and cart controls.
- Footer includes newsletter, policies, copyright, and social-link blocks.

## Manual checks before publishing

- Verify the main navigation links in Shopify Admin.
- Verify desktop, tablet, and mobile layouts in the theme preview.
- Test every product variant and add-to-cart path.
- Confirm inventory and market availability for the intended selling region.
- Open the cart drawer, change quantity, remove an item, and visit the cart page.
- Enter checkout only with Shopify's test configuration; do not activate real payments.
- Replace placeholder social URLs with official ASIMON profiles.
- Confirm store policies and contact details before launch.

## Known store-data issue

Product availability previously appeared as sold out in some preview contexts even when inventory tracking was disabled. Recheck product publication, market availability, and fulfillment location configuration before launch.
