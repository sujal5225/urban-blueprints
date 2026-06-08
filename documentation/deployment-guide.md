# Deployment Guide: Urban Blueprints

## Prerequisites
- Node.js 18+ installed
- npm or yarn

## Build Process
To generate the static export for deployment:

```bash
cd urban-blueprints
npm install
npm run build
```

This will generate an `out` directory containing the fully optimized static HTML, CSS, and JS files.

## Deployment to Vercel
1. Connect your GitHub repository to Vercel.
2. Set the Framework Preset to **Next.js**.
3. The Build Command should be automatically detected as `npm run build`.
4. The Output Directory should be set to `out` (or left default if Next.js handles it).
5. Click **Deploy**.

## Deployment to Any Static Host (Netlify, AWS S3, Cloudflare Pages)
Simply upload the contents of the `out` directory to your static hosting provider.

## Domain Configuration
- Ensure your DNS records point to your hosting provider.
- Set the primary domain to `urban-blueprintscom.com`.
- Configure SSL/TLS certificates (usually handled automatically by Vercel/Netlify/Cloudflare).
