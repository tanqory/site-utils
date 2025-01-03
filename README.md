# Site Form Config

A simple configuration package for site form IDs. This package provides predefined constants for various site settings and form IDs to be used in your application.

## Installation

Install the package using npm:

```bash
npm install @tanqory/site-utils
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

The package includes the following form ID constants:

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

## License

This project is licensed under the MIT License.
