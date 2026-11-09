# NGANYA ELITES — React/Vite production project

This package contains the original NGANYA ELITES React application prepared as a standard Vite project. It is source code, not a prebuilt `dist` deployment; dependencies must be installed and the production build generated before a manual Netlify upload.

## Build

Requires Node.js 18 or newer.

```bash
npm install
npm run build
```

Vite creates the production website in `dist/`.

## Netlify

For a Git-connected Netlify site, set:
- Build command: `npm run build`
- Publish directory: `dist`

For a manual Netlify deploy, upload the contents of `dist/` after running the build. Do not upload this source folder as if it were the built website.

## Important current limitations

The supplied original React app is a frontend prototype. Its data collections are held in React state and are not connected to Supabase in this source. Its existing customer authentication/payment flows are not production-secure. This packaging does not add backend authentication, database persistence, real SMS, or M-Pesa payment verification.
