# Site Form Config

A simple configuration package for site form IDs. This package provides predefined constants for various site settings and form IDs to be used in your application.

## Installation

### From npm (recommended):

```bash
npm install @tanqory/site-utils
```

### From GitHub Packages:

```bash
npm install @tanqory/site-utils --registry https://npm.pkg.github.com
```

## Usage

### JavaScript:

```javascript
const { SiteFormConfig } = require("@tanqory/site-utils");

// Example usage
console.log(SiteFormConfig.SITES_SETTING_FORM_ID_CREATE_SITE);
// Output: "SITES_SETTING_FORM_ID_CREATE_SITE"
```

### TypeScript:

```typescript
import { SiteFormConfig } from "@tanqory/site-utils";

// Example usage with type checking
console.log(SiteFormConfig.SITES_SETTING_FORM_ID_CREATE_SITE);
// Output: "SITES_SETTING_FORM_ID_CREATE_SITE"
```

## Available Constants

### Settings Form IDs

- `SITES_SETTING_FORM_ID_CREATE_SITE`
- `SITES_SETTING_FORM_ID_GENERALE`
- `SITES_SETTING_FORM_ID_SETUP_GUIDE`
- `SITES_SETTING_FORM_ID_PLAN`
- `SITES_SETTING_FORM_ID_BILLING`
- `SITES_SETTING_FORM_ID_USERS_PERMISSIONS`
- `SITES_SETTING_FORM_ID_PAYMENTS`
- `SITES_SETTING_FORM_ID_CHECKOUT`
- `SITES_SETTING_FORM_ID_CUSTOMER_ACCOUNTS`
- `SITES_SETTING_FORM_ID_SHIPPING`
- `SITES_SETTING_FORM_ID_TAXES`
- `SITES_SETTING_FORM_ID_LOCATIONS`
- `SITES_SETTING_FORM_ID_MARKETS`
- `SITES_SETTING_FORM_ID_APPS_SALES_CHANNELS`
- `SITES_SETTING_FORM_ID_DOMAINS`
- `SITES_SETTING_FORM_ID_CUSTOMER_EVENTS`
- `SITES_SETTING_FORM_ID_NOTIFICATIONS`
- `SITES_SETTING_FORM_ID_NOTIFICATIONS_STAFF`
- `SITES_SETTING_FORM_ID_NOTIFICATIONS_WEBHOOK`
- `SITES_SETTING_FORM_ID_NOTIFICATIONS_CUSTOMER`
- `SITES_SETTING_FORM_ID_CUSTOM_DATA`
- `SITES_SETTING_FORM_ID_LANGUAGES_DATA`
- `SITES_SETTING_FORM_ID_PRIVACY_DATA`
- `SITES_SETTING_FORM_ID_POLICY_DATA`

### Content and Store Form IDs

- `SITES_FORM_ID_CONTENT_FILE`
- `SITES_FORM_ID_CONTENT_META_OBJECTS`
- `SITES_FORM_ID_CUSTOMER`
- `SITES_FORM_ID_CUSTOMER_SEGMENTS`
- `SITES_FORM_ID_DEMO_PREVIEW`
- `SITES_FORM_ID_DISCOUNTS`
- `SITES_FORM_ID_ONLINE_STORE_MENU`
- `SITES_FORM_ID_ONLINE_STORE_PAGE`
- `SITES_FORM_ID_ONLINE_STORE_POST`
- `SITES_FORM_ID_ONLINE_STORE_PREFERENCES`
- `SITES_FORM_ID_ORDER`
- `SITES_FORM_ID_ORDER_CHECKOUTS`
- `SITES_FORM_ID_ORDER_DRAFT`
- `SITES_FORM_ID_PRODUCT`
- `SITES_FORM_ID_PRODUCT_COLLECTIONS`
- `SITES_FORM_ID_PRODUCT_GIFT`
- `SITES_FORM_ID_PRODUCT_INVENTORY`
- `SITES_FORM_ID_PRODUCT_PURCHASE`
- `SITES_FORM_ID_PRODUCT_TRANSFERS`

## Project Structure

```
src/
├── index.ts                 # Package entry point
└── utils/
    └── site.form.config.ts  # Form ID constants and types
dist/
├── index.js
├── index.d.ts
└── utils/
    ├── site.form.config.js
    └── site.form.config.d.ts
```

## TypeScript Support

This package includes TypeScript declarations and provides full type safety. The type definitions are automatically included when you install the package.

## Development

To build the package:

```bash
npm run build
```

To publish the package:

```bash
npm publish
```

## License

This project is licensed under the MIT License.
