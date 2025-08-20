# @tanqory/site-utils

[![npm version](https://badge.fury.io/js/@tanqory%2Fsite-utils.svg)](https://badge.fury.io/js/@tanqory%2Fsite-utils)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.7+-blue.svg)](https://www.typescriptlang.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A comprehensive TypeScript utility package that provides predefined constants for site form IDs and configurations. This package is designed to centralize form ID management for Tanqory applications, ensuring consistency across different modules and components while improving developer experience.

## ✨ Features

- ✅ **Full TypeScript Support**: Complete type safety with IntelliSense support
- 🔧 **Centralized Configuration**: Single source of truth for all form IDs
- 📦 **Zero Dependencies**: Lightweight package with minimal bundle size
- 🚀 **Easy Integration**: Simple import and usage in any JavaScript/TypeScript project
- 🔄 **Consistent Naming**: Standardized naming conventions across all form IDs
- 🎯 **Tree Shakable**: Import only what you need
- 🛡️ **Production Ready**: Battle-tested in production environments

## 📦 Installation

### Using npm (Recommended)

```bash
npm install @tanqory/site-utils
```

### Using yarn

```bash
yarn add @tanqory/site-utils
```

### Using pnpm

```bash
pnpm add @tanqory/site-utils
```

### From GitHub Packages

```bash
npm install @tanqory/site-utils --registry https://npm.pkg.github.com
```

## 🚀 Quick Start

### JavaScript (CommonJS)

```javascript
const { SiteFormConfig } = require("@tanqory/site-utils");

// Access form IDs
console.log(SiteFormConfig.SITES_SETTING_FORM_ID_CREATE_SITE);
// Output: "SITES_SETTING_FORM_ID_CREATE_SITE"

// Use in form validation
if (formId === SiteFormConfig.SITES_SETTING_FORM_ID_GENERAL) {
  // Handle general settings form
}
```

### TypeScript (ES Modules)

```typescript
import { SiteFormConfig } from "@tanqory/site-utils";

// Type-safe access to form IDs
const createSiteFormId: string =
  SiteFormConfig.SITES_SETTING_FORM_ID_CREATE_SITE;

// Use with type checking
function handleFormSubmission(formId: string) {
  switch (formId) {
    case SiteFormConfig.SITES_SETTING_FORM_ID_GENERAL:
      // Handle general settings
      break;
    case SiteFormConfig.SITES_SETTING_FORM_ID_BILLING:
      // Handle billing settings
      break;
    default:
    // Handle unknown form
  }
}
```

### React Example

```tsx
import React from "react";
import { SiteFormConfig } from "@tanqory/site-utils";

const SettingsPage: React.FC = () => {
  const handleFormChange = (formId: string) => {
    if (formId === SiteFormConfig.SITES_SETTING_FORM_ID_GENERAL) {
      // Update general settings UI
    }
  };

  return (
    <div>
      <form id={SiteFormConfig.SITES_SETTING_FORM_ID_GENERAL}>
        {/* Form content */}
      </form>
    </div>
  );
};
```

## 📋 Available Constants

### 🔧 Settings Form IDs

Form IDs for various site settings and configuration pages:

| Constant                                       | Description               |
| ---------------------------------------------- | ------------------------- |
| `SITES_SETTING_FORM_ID_CREATE_SITE`            | Site creation form        |
| `SITES_SETTING_FORM_ID_GENERAL`                | General site settings     |
| `SITES_SETTING_FORM_ID_SETUP_GUIDE`            | Setup guide form          |
| `SITES_SETTING_FORM_ID_PLAN`                   | Plan management           |
| `SITES_SETTING_FORM_ID_BILLING`                | Billing settings          |
| `SITES_SETTING_FORM_ID_SUBSCRIPTION`           | Subscription management   |
| `SITES_SETTING_FORM_ID_USERS_PERMISSIONS`      | User permissions          |
| `SITES_SETTING_FORM_ID_PAYMENTS`               | Payment settings          |
| `SITES_SETTING_FORM_ID_CHECKOUT`               | Checkout configuration    |
| `SITES_SETTING_FORM_ID_CUSTOMER_ACCOUNTS`      | Customer account settings |
| `SITES_SETTING_FORM_ID_SHIPPING`               | Shipping settings         |
| `SITES_SETTING_FORM_ID_TAXES`                  | Tax configuration         |
| `SITES_SETTING_FORM_ID_LOCATIONS`              | Location management       |
| `SITES_SETTING_FORM_ID_MARKETS`                | Market settings           |
| `SITES_SETTING_FORM_ID_APPS_SALES_CHANNELS`    | Apps and sales channels   |
| `SITES_SETTING_FORM_ID_DOMAINS`                | Domain management         |
| `SITES_SETTING_FORM_ID_CUSTOMER_EVENTS`        | Customer events           |
| `SITES_SETTING_FORM_ID_NOTIFICATIONS`          | General notifications     |
| `SITES_SETTING_FORM_ID_NOTIFICATIONS_STAFF`    | Staff notifications       |
| `SITES_SETTING_FORM_ID_NOTIFICATIONS_WEBHOOK`  | Webhook notifications     |
| `SITES_SETTING_FORM_ID_NOTIFICATIONS_CUSTOMER` | Customer notifications    |
| `SITES_SETTING_FORM_ID_CUSTOM_DATA`            | Custom data management    |
| `SITES_SETTING_FORM_ID_LANGUAGES_DATA`         | Language settings         |
| `SITES_SETTING_FORM_ID_PRIVACY_DATA`           | Privacy settings          |
| `SITES_SETTING_FORM_ID_POLICY_DATA`            | Policy management         |
| `SITES_SETTING_FORM_ID_LOCATION_DETAILS`       | Location details          |
| `SITES_SETTING_FORM_ID_SHIPPING_PROFILES`      | Shipping profiles         |
| `SITES_SETTING_FORM_ID_SHIPPING_ZONES`         | Shipping zones            |
| `SITES_SETTING_FORM_ID_MARKETS_RULES`          | Market rules              |
| `SITES_SETTING_FORM_ID_SHIPPING_LOCATIONS`     | Shipping locations        |
| `SITES_SETTING_FORM_ID_TAXES_REGIONAL`         | Regional tax settings     |

### 🛒 Content and Store Form IDs

Form IDs for content management and store operations:

| Constant                                  | Description             |
| ----------------------------------------- | ----------------------- |
| `SITES_FORM_ID_CONTENT_FILE`              | File content management |
| `SITES_FORM_ID_CONTENT_META_OBJECTS`      | Meta objects            |
| `SITES_FORM_ID_CUSTOMER`                  | Customer management     |
| `SITES_FORM_ID_CUSTOMER_SEGMENTS`         | Customer segmentation   |
| `SITES_FORM_ID_DEMO_PREVIEW`              | Demo preview            |
| `SITES_FORM_ID_DISCOUNTS`                 | Discount management     |
| `SITES_FORM_ID_ONLINE_STORE_MENU`         | Online store menu       |
| `SITES_FORM_ID_ONLINE_STORE_PAGE`         | Store pages             |
| `SITES_FORM_ID_ONLINE_STORE_POST`         | Store posts             |
| `SITES_FORM_ID_ONLINE_STORE_PREFERENCES`  | Store preferences       |
| `SITES_FORM_ID_ORDER`                     | Order management        |
| `SITES_FORM_ID_ORDER_CHECKOUTS`           | Order checkouts         |
| `SITES_FORM_ID_ORDER_DRAFT`               | Draft orders            |
| `SITES_FORM_ID_PRODUCT`                   | Product management      |
| `SITES_FORM_ID_PRODUCT_COLLECTIONS`       | Product collections     |
| `SITES_FORM_ID_PRODUCT_GIFT`              | Gift products           |
| `SITES_FORM_ID_PRODUCT_INVENTORY`         | Inventory management    |
| `SITES_FORM_ID_PRODUCT_PURCHASE`          | Product purchases       |
| `SITES_FORM_ID_PRODUCT_TRANSFERS`         | Product transfers       |
| `SITES_FORM_ID_PRODUCT_VARIANTS`          | Product variants        |
| `SITES_FORM_ID_ONLINE_STORE_BLOG`         | Blog management         |
| `SITES_FORM_ID_PRODUCT_PURCHASE_SUPPLIER` | Supplier purchases      |
| `SITES_FORM_ID_ANALYTICS_REPORTS`         | Analytics and reports   |
| `SITES_FORM_ID_TIMELINE`                  | Timeline management     |
| `SITES_FORM_ID_PRODUCT_INVENTORY_HISTORY` | Inventory history       |

## 📁 Project Structure

```
@tanqory/site-utils/
├── 📄 package.json          # Package configuration
├── 📄 tsconfig.json         # TypeScript configuration
├── 📄 README.md            # Documentation
├── 📄 LICENSE              # MIT license
├── 📂 src/                 # Source code
│   ├── 📄 index.ts          # Main entry point
│   └── 📂 utils/
│       └── 📄 site.form.config.ts  # Form ID constants
└── 📂 dist/                # Compiled output
    ├── 📄 index.js          # Compiled entry point
    ├── 📄 index.d.ts        # Type definitions
    └── 📂 utils/
        ├── 📄 site.form.config.js   # Compiled constants
        └── 📄 site.form.config.d.ts # Type definitions
```

## 🔧 TypeScript Support

This package is built with TypeScript and provides:

- ✅ **Full Type Safety**: All constants are strongly typed
- ✅ **IntelliSense Support**: Auto-completion in modern IDEs
- ✅ **Zero Runtime Overhead**: Constants are inlined during compilation
- ✅ **Tree Shaking**: Import only what you need
- ✅ **Compatible with all TypeScript versions**: 4.0+

### Type Definitions

```typescript
// All form IDs are exported as string constants
export declare const SiteFormConfig: {
  readonly SITES_SETTING_FORM_ID_CREATE_SITE: string;
  readonly SITES_SETTING_FORM_ID_GENERAL: string;
  // ... and many more
};
```

## 🛠️ Development

### Prerequisites

- **Node.js**: 16.0.0 or higher
- **TypeScript**: 5.7.0 or higher
- **Package Manager**: npm, yarn, or pnpm

### Setup Development Environment

```bash
# Clone the repository
git clone https://github.com/tanqory/site-utils.git
cd site-utils

# Install dependencies
npm install

# Build the package
npm run build

# Run linting
npm run lint
```

### Available Scripts

| Script                   | Description                      |
| ------------------------ | -------------------------------- |
| `npm run build`          | Compile TypeScript to JavaScript |
| `npm run lint`           | Run ESLint for code quality      |
| `npm run lint:fix`       | Run ESLint with auto-fix         |
| `npm start`              | Run the compiled package         |
| `npm test`               | Run test suite (coming soon)     |
| `npm run prepublishOnly` | Auto-build before publishing     |

### Building the Package

```bash
# Clean build
npm run build

# The compiled files will be in the dist/ directory
```

### Code Quality

This project uses ESLint for maintaining code quality:

```bash
# Check for linting issues
npm run lint

# Auto-fix linting issues
npm run lint:fix
```

## 📦 Publishing

### Publishing to npm Registry

```bash
npm run publish:npm
```

### Publishing to GitHub Packages

```bash
npm run publish:github
```

### Publishing to Both Registries

```bash
npm run publish:all
```

> **Note**: Make sure you have the necessary permissions and authentication setup for both registries before publishing.

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the Repository**

   ```bash
   git clone https://github.com/your-username/site-utils.git
   ```

2. **Create a Feature Branch**

   ```bash
   git checkout -b feature/amazing-feature
   ```

3. **Make Your Changes**

   - Add new form IDs to `src/utils/site.form.config.ts`
   - Update documentation if needed
   - Follow the existing naming conventions

4. **Test Your Changes**

   ```bash
   npm run build
   npm run lint
   ```

5. **Commit Your Changes**

   ```bash
   git commit -m 'Add some amazing feature'
   ```

6. **Push to Your Branch**

   ```bash
   git push origin feature/amazing-feature
   ```

7. **Open a Pull Request**
   - Describe your changes clearly
   - Include any relevant context or screenshots

### Coding Standards

- Follow TypeScript best practices
- Use consistent naming conventions (SCREAMING_SNAKE_CASE for constants)
- Add JSDoc comments for new constants
- Ensure all code passes ESLint rules

## 📊 Version History

| Version     | Date       | Changes                                                               |
| ----------- | ---------- | --------------------------------------------------------------------- |
| **v0.0.33** | 2025-08-20 | Current version - Enhanced form ID support and improved documentation |
| **v0.0.29** | -          | Added shipping, location, and analytics form IDs                      |
| **v0.0.1**  | -          | Initial release with basic form ID constants                          |

## 🆘 Support

- 📧 **Email**: [support@tanqory.com](mailto:support@tanqory.com)
- 🐛 **Issues**: [GitHub Issues](https://github.com/tanqory/site-utils/issues)
- 📚 **Documentation**: [GitHub Repository](https://github.com/tanqory/site-utils)

## 👨‍💻 Author

**TANQ PTE. LTD.**

- Website: [https://tanqory.com](https://tanqory.com)
- GitHub: [@tanqory](https://github.com/tanqory)

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Made with ❤️ by [TANQ PTE. LTD.](https://tanqory.com)**

[![npm](https://img.shields.io/npm/v/@tanqory/site-utils)](https://www.npmjs.com/package/@tanqory/site-utils)
[![GitHub stars](https://img.shields.io/github/stars/tanqory/site-utils)](https://github.com/tanqory/site-utils/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/tanqory/site-utils)](https://github.com/tanqory/site-utils/issues)

</div>
