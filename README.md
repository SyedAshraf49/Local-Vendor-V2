# Local Connect — Local Vendor V2

A neighborhood marketplace prototype that brings customers and local vendors together to browse and manage everyday essentials. Built as a responsive React and TypeScript app with separate customer and vendor experiences.

**Live demo:** [local-vendor-v2.vercel.app](https://local-vendor-v2.vercel.app)

## Features

### Customer demo
- Browse and search a seeded catalogue of everyday products from sample Chennai neighborhoods.
- Manage a cart, favorites and pre-orders; complete a simulated checkout and view order progress.
- View featured products and recipe suggestions. Recipes currently use local mock data.
- Choose from English, Tamil, Hindi, Telugu and Malayalam UI translations.

### Vendor demo
- View orders for a sample vendor location and inspect order details.
- Add, edit, delete and reset products in the local catalogue.
- Review and manage pre-orders, and view an earnings report.

Sample vendor locations are Royapuram, T. Nagar, Ashok Nagar and Saidapet. Product changes and cart contents are stored in the browser. Authentication, orders and other demo state are not backed by a server.

## Try the demo

Select a role on the sign-in screen and use one of these public demo accounts. All use the password `pass`.

| Role | Username | Sample location |
| --- | --- | --- |
| Customer | `customer` | — |
| Vendor | `vendorR` | Royapuram |
| Vendor | `vendorT` | T. Nagar |
| Vendor | `vendorA` | Ashok Nagar |
| Vendor | `vendorS` | Saidapet |

These credentials are for demonstration only. Do not enter real personal or payment information.

## Run locally

Requirements: Node.js and npm.

```bash
npm ci
npm run dev
```

Vite serves the development app at `http://localhost:3000` by default. Create and preview a production build with:

```bash
npm run build
npm run preview
```

## Skills and technologies

- **Frontend:** React 19, TypeScript, Vite 6
- **UI:** Tailwind CSS (loaded from its CDN), responsive component design, light/dark and seasonal themes
- **Application state:** React Context API and browser `localStorage`
- **Product capabilities:** role-based demo screens, catalogue management, cart and order workflows, localization, mock recipe suggestions
- **Deployment:** Vercel

## Demo limitations

Local Connect is a client-side prototype, not a production commerce service. Sign-in uses hard-coded demo credentials; there is no server-side authentication, shared inventory or order database, or payment processor. Checkout and order progress are simulated. Recipe suggestions return fixed local examples rather than calling Gemini, and recipe content is currently in English.

## Deployment

The app is deployed on [Vercel](https://local-vendor-v2.vercel.app). The repository's `vercel.json` configures the Vite build command (`npm run build`) and output directory (`dist`).
