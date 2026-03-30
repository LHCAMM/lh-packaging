# LH Packaging Website

A professional, production-ready website for LH Packaging—a packaging supply company serving small businesses, startups, and ecommerce brands.

## Features

- **Modern Design**: Clean, professional aesthetic with navy and steel color palette
- **Fully Responsive**: Mobile-first design that works on all devices
- **SEO Optimized**: Proper meta tags and keyword-friendly content
- **Fast Performance**: Optimized for speed with Vite
- **Easy to Edit**: Centralized data files for pricing and contact information

## Pages/Sections

1. **Hero**: Strong headline with CTAs and trust indicators
2. **About**: Company story and mission
3. **Products**: Product categories with descriptions
4. **Pricing**: Editable price list with expandable categories
5. **Why Choose Us**: Business benefits and differentiators
6. **How Ordering Works**: 3-step process explanation
7. **Contact**: Contact info and inquiry form

## Tech Stack

- **Framework**: React + Vite
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Build Output**: Static export for easy deployment

## Getting Started

### 1. Install Dependencies

```bash
npm install
```

### 2. Run Development Server

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) to view the site.

### 3. Build for Production

```bash
npm run build
```

This creates a static export in the `dist` folder.

## Deployment

### Deploy to Vercel

1. Push your code to GitHub:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/lh-packaging.git
git push -u origin main
```

2. Connect to Vercel:
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Framework Preset: Vite
   - Deploy

### Deploy to Netlify

1. Build the project: `npm run build`
2. Drag and drop the `dist` folder to Netlify

### Deploy to Other Static Hosts

The `dist` folder contains the static site. Upload these files to any static hosting service.

## Customization

### Edit Contact Information

Update `src/data/pricing.ts`:

```typescript
export const CONTACT_INFO = {
  phone: '567-202-3240',
  email: 'lhpackaging@gmail.com',
  companyName: 'LH Packaging',
}
```

### Edit Pricing

Update `src/data/pricing.ts`:

The `pricingData` array contains all product categories and items. Each item has:
- `id`: Unique identifier
- `category`: Category ID
- `name`: Product name
- `size`: Size dimensions
- `quantity`: Pack size
- `price`: Price in USD
- `notes`: Optional description

### Edit Colors

Update `tailwind.config.js`:

The color palette is defined in the `theme.extend.colors` section.

### Edit Content

All section content is in the `src/components` folder:
- `Hero.tsx` - Homepage hero section
- `About.tsx` - About section
- `Products.tsx` - Product categories
- `Pricing.tsx` - Pricing display
- `WhyChooseUs.tsx` - Benefits section
- `HowOrderingWorks.tsx` - Process explanation
- `Contact.tsx` - Contact section and form

## Project Structure

```
lh-packaging/
├── public/                # Static assets
│   └── favicon.svg
├── src/
│   ├── components/        # React components
│   │   ├── Navigation.tsx
│   │   ├── Hero.tsx
│   │   ├── About.tsx
│   │   ├── Products.tsx
│   │   ├── Pricing.tsx
│   │   ├── WhyChooseUs.tsx
│   │   ├── HowOrderingWorks.tsx
│   │   ├── Contact.tsx
│   │   ├── Footer.tsx
│   │   └── Logo.tsx
│   ├── data/              # Editable data files
│   │   └── pricing.ts
│   ├── App.tsx
│   ├── index.css
│   ├── main.tsx
│   └── vite-env.d.ts
├── index.html
├── tailwind.config.js
├── postcss.config.js
├── vite.config.ts
├── tsconfig.json
├── package.json
└── README.md
```

## Business Information

- **Company**: LH Packaging
- **Phone**: 567-202-3240
- **Email**: lhpackaging@gmail.com
- **Business Type**: Packaging supply company (B2B)

## License

This project is proprietary to LH Packaging.
