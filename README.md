# ASIMON Fashion Studio

ASIMON Fashion Studio is a premium Shopify fashion storefront built on Shopify's Horizon theme. The project demonstrates theme customization, merchant-editable Liquid sections, responsive product merchandising, native cart behavior, and a safe GitHub-based development workflow.

## Storefront highlights

- Editorial hero with separate desktop and mobile imagery
- Merchant-editable headings, copy, buttons, colors, and spacing
- New Arrivals product grid backed by a real Shopify collection
- Fashion product pages with media, variants, quantity controls, availability, and native add-to-cart behavior
- Responsive header with search, account, localization, and cart controls
- Native Shopify cart drawer and cart page
- Newsletter signup, policy links, and social-link support
- Accessible semantic markup and reduced-motion-aware interactions

## Technology

- Shopify Liquid and JSON templates
- HTML, modern CSS, and JavaScript components
- Shopify CLI and Theme Check
- Git and GitHub pull-request workflow
- Shopify Admin collections, products, variants, inventory, and navigation

## Development workflow

1. Create a feature branch from `main`.
2. Preview changes with `shopify theme dev` on a development theme.
3. Run `shopify theme check` and manually test the affected storefront paths.
4. Commit and push the feature branch.
5. Review and merge through a pull request.

The active storefront theme is never replaced automatically by this repository.

## Project documentation

- [ASIMON product catalog](docs/product-catalog.md)
- [Storefront testing report](docs/testing-report.md)
- [Portfolio and freelance copy](docs/portfolio-copy.md)

## Local preview

```powershell
shopify theme dev --store asimon-fashion-studio.myshopify.com --theme-editor-sync --reconciliation-strategy keep-local
```

Do not commit access tokens, passwords, customer data, or other store secrets.
