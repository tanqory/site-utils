# @tanqory/site-utils

A TypeScript utility package that provides predefined constants for site form IDs and configurations. This package is designed to centralize form ID management for Tanqory applications, ensuring consistency across different modules and components.

## Features

- ✅ **TypeScript Support**: Full type safety and IntelliSense support
- 🔧 **Centralized Configuration**: Single source of truth for form IDs
- 📦 **Lightweight**: Zero dependencies, minimal bundle size
- 🚀 **Easy Integration**: Simple import and usage
- 🔄 **Consistent Naming**: Standardized naming conventions across all form IDs

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
- `SITES_SETTING_FORM_ID_GENERAL`
- `SITES_SETTING_FORM_ID_SETUP_GUIDE`
- `SITES_SETTING_FORM_ID_PLAN`
- `SITES_SETTING_FORM_ID_BILLING`
- `SITES_SETTING_FORM_ID_SUBSCRIPTION`
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
- `SITES_SETTING_FORM_ID_LOCATION_DETAILS`
- `SITES_SETTING_FORM_ID_SHIPPING_PROFILES`
- `SITES_SETTING_FORM_ID_SHIPPING_ZONES`
- `SITES_SETTING_FORM_ID_MARKETS_RULES`
- `SITES_SETTING_FORM_ID_SHIPPING_LOCATIONS`
- `SITES_SETTING_FORM_ID_TAXES_REGIONAL`

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
- `SITES_FORM_ID_PRODUCT_VARIANTS`
- `SITES_FORM_ID_ONLINE_STORE_BLOG`
- `SITES_FORM_ID_PRODUCT_PURCHASE_SUPPLIER`
- `SITES_FORM_ID_ANALYTICS_REPORTS`
- `SITES_FORM_ID_TIMELINE`
- `SITES_FORM_ID_PRODUCT_INVENTORY_HISTORY`

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

### Prerequisites

- Node.js 16+
- TypeScript 5.7+
- npm or yarn

### Building the Package

```bash
npm run build
```

### Linting

```bash
npm run lint
```

### Publishing

#### To npm registry:

```bash
npm run publish:npm
```

#### To GitHub Packages:

```bash
npm run publish:github
```

#### To both registries:

```bash
npm run publish:all
```

### Development Scripts

- `npm run build` - Compile TypeScript to JavaScript
- `npm run lint` - Run ESLint
- `npm run lint:fix` - Run ESLint with auto-fix
- `npm start` - Run the compiled package
- `npm test` - Run tests (to be implemented)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Version History

- **v0.0.29** - Current version with enhanced form ID support
- Latest updates include additional shipping, location, and analytics form IDs

## Author

**TANQ PTE. LTD.**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
