# South County Threadz Website

## Project Overview

**Business:** South County Threadz  
**Tagline:** NEW • OLD • GOLD  
**Description:** Curated new and pre-loved brand-name clothing and fashion finds  
**Location:** Southern Rhode Island  
**Primary Users:** Public shoppers  
**Primary Goal:** Establish a professional branded web presence and direct visitors to South County Threadz's selling platforms and social media.

## Project Scope

This project is a **simple static website** consisting of a one-page responsive landing page with no backend infrastructure.

### Architecture

- ❌ No authentication
- ❌ No database
- ❌ No backend
- ❌ No persistent customer data
- ❌ No payment processing
- ✅ External shopping/social platform links
- ✅ Basic SEO optimization
- ✅ WCAG AA accessibility compliance
- ✅ Mobile responsiveness

## External Destinations

### Shopping Platforms
- **eBay:** https://www.ebay.com/usr/southcountythreadz
- **Poshmark:** https://poshmark.com/closet/threadzri
- **Depop:** https://www.depop.com/southcountythreadz/
- **Whatnot:** https://www.whatnot.com/user/southcountythreadz

### Social Media
- **Facebook:** https://www.facebook.com/SouthCountyThreadz
- **Instagram:** https://www.instagram.com/southcountythreadz/

## Project Structure

```
south-county-threadz/
├── src/
│   ├── index.html
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── main.js
│   └── assets/
│       ├── images/
│       └── fonts/
├── README.md
├── CLAUDE.md
├── .gitignore
└── package.json
```

## Current TBD Items

- [ ] **Logo:** Final South County Threadz logo (placeholder to be used during development)
- [ ] **Domain:** Production domain name (TBD)
- [ ] **Hosting:** Client's Netlify account setup
- [ ] **Editorial Photography:** See Photo Direction below

## Photo Direction

The About section features an editorial photo treatment instead of product cards. The client should provide:

**Required Photos:**
- 1 primary image (main photo, aspect ratio 4:3)
- 2 supporting images (for a collage treatment or row display)

**Photo Guidelines:**
- Should communicate the personality and business aesthetic of South County Threadz
- Can include lifestyle shots, styled product collections, or behind-the-scenes imagery
- Should be high-quality and consistent in style/lighting
- Professional or semi-professional photography recommended
- Client owns the rights to all photos used
- Files: JPG or PNG format, optimized for web (72 DPI, <500KB per image recommended)

**Placeholder:** Currently styled as placeholder divs to demonstrate layout. Replace placeholder divs with `<img>` tags and proper alt text when photos are provided.

## Brand Direction

The South County Threadz website uses a **vintage/elevated thrift boutique aesthetic** with the following color palette:

### Primary Colors

| Color | Hex Value | Usage |
|-------|-----------|-------|
| **Soft Cream** | `#f5f1e8` | Primary website background—majority of page |
| **Deep Navy** | `#1a2a3a` | Primary typography, headings, navigation, structural elements |
| **Antique Gold** | `#c9a961` | Accent only: thin rules, small borders, hover details, tiny decorative accents |
| **Black/White** | Supporting neutrals | Used only when necessary for contrast |

### Design Principles

- Warm, inviting cream background throughout the page
- Navy blue for all primary text and headings
- Gold used very sparingly and restrained (accent only, not dominant)
- Clean, sophisticated aesthetic reflecting a curated vintage boutique
- Coordinates with the developing South County Threadz logo (deep navy lettering with antique-gold detailing on soft cream background)

### Color Variables in CSS

All colors are centralized as CSS variables for easy updates when the final brand board is approved:
- `--color-primary-light`: Soft cream background
- `--color-primary-dark`: Deep navy text
- `--color-accent`: Antique gold accents
- `--color-accent-light`: Lighter gold for hover/secondary uses

## Official Platform Brand Assets

The "Shop South County Threadz" section links to official selling platforms using compact button-style tiles. The design intentionally uses restrained platform branding to keep focus on South County Threadz.

### Brand Asset Sourcing Guidelines

**IMPORTANT:** All platform brand assets must come from official sources only. Do not use:
- Recreated/unofficial logos
- Random Google Image results
- Guessed or assumed brand materials
- Unauthorized reproductions

**Before using any platform asset:**
1. Confirm it comes from an official company resource
2. Review their published brand/logo usage guidelines
3. Use the appropriate official variant for light backgrounds
4. Preserve required proportions and clear space
5. Do not recolor or distort unless explicitly permitted

**If an official asset cannot be confidently obtained,** use clean text-based styling and document the limitation.

### Official Resources by Platform

**REQUIRED:** Download official logo assets and place them in `src/assets/images/platform-logos/`

| Platform | Official Download Location | Current Status | Action Required |
|----------|---------------------------|-----------------|-----------------|
| **eBay** | eBay press/brand resources (https://www.ebay.com) | Logo needed | Access eBay's official brand resources or Seller Central for the official eBay logo (SVG or PNG, 500px+ width, transparent background preferred). |
| **Poshmark** | Poshmark press kit (https://poshmark.com/press) | Logo needed | Visit Poshmark's official press page to download their logo asset. Poshmark typically provides logos in multiple formats. |
| **Depop** | Depop official website or support resources (https://www.depop.com) | Logo needed | Contact Depop or access their official brand guidelines to obtain their logo asset. |
| **Whatnot** | Whatnot creator resources (https://whatnot.com/creators) or brand page | Logo needed | Download Whatnot's official logo from their creator resources or official brand materials. |

### Current Implementation

Shop buttons currently display:
- Small colored icon badge with initials/abbreviations (temporary placeholder)
- Platform name (text: "eBay", "Poshmark", "Depop", "Whatnot")
- Arrow indicator (→)

**Next Step:** Replace temporary icon badges with official platform logos:
1. Download official logo from each platform's official resources (see table above)
2. Save to `src/assets/images/platform-logos/` with naming: `ebay-logo.svg`, `poshmark-logo.svg`, `depop-logo.svg`, `whatnot-logo.svg`
3. Update HTML to use `<img>` tags instead of text badges
4. Create `BRAND-ASSETS-SOURCES.md` documenting:
   - Download date for each logo
   - Official source URL
   - Any brand usage restrictions/permissions
   - Logo file specifications (format, dimensions, colors)

### Logo Specifications

For consistency across buttons, downloaded logos should ideally be:
- Format: SVG preferred (scalable), PNG acceptable (minimum 256px width)
- Background: Transparent
- Size: 32-48px display height in buttons
- Colors: Use official brand colors as published (do not recolor unless brand guidelines explicitly allow)
- Aspect ratio: Preserve original proportions

## Ownership & Deployment

- **Developer:** Sweet Creatives / Michelle
- **Client Ownership:** Client will own production domain and hosting
- **Production Hosting:** Expected to be client's Netlify account
- **Approval Required:** Client approval required before production launch

## Development Guidelines

See [CLAUDE.md](CLAUDE.md) for AI development rules and constraints.

## Content & Copy Strategy

**Sweet Creatives** will draft the website copy using the approved business information. The client will review and approve the content during the normal review process.

## Getting Started

This is a lightweight static website with no build processes required for development. Open `src/index.html` in a browser to view.

**Note:** The visual website design and content build will occur in a subsequent phase after this initialization is complete.
