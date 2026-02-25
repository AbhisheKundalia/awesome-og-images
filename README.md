# Awesome OG Images [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, libraries, and resources for generating Open Graph images

Open Graph images are the preview images shown when you share a link on social media. This list covers everything from APIs and libraries to templates and best practices.

## Contents

- [Services & APIs](#services--apis)
- [Libraries](#libraries)
- [Frameworks with Built-in Support](#frameworks-with-built-in-support)
- [Templates](#templates)
- [Best Practices](#best-practices)
- [Articles](#articles)

## Services & APIs

### Free / Freemium

- **[OG:IMAGE](https://ogimage.art)** - Simple API that generates beautiful OG images. One URL = one image. 8 templates, $9/mo Pro tier. `GET /api/og?title=Hello`
- **[SnapOG](https://snapog.shiplab.xyz)** - One-time payment OG image API. 11 themes, free tier (50 req/hour), $49 one-time for unlimited lifetime access. `GET /og?title=Title&theme=dark`
- **[Vercel OG](https://vercel.com/docs/concepts/functions/edge-functions/og-image-generation)** - Generate dynamic OG images at the edge using React components. Free for Vercel users.
- **[Cloudinary](https://cloudinary.com/documentation/social_media_image_generation)** - Image transformation API with OG image support. Free tier available.

### Paid

- **[Bannerbear](https://www.bannerbear.com/)** - Auto-generate images and videos. From $49/mo.
- **[Placid](https://placid.app/)** - Design templates and generate images via API. From $19/mo.
- **[RoboHash](https://robohash.org/)** - Generate unique robot avatars. Free, useful for placeholder OG images.

## Libraries

### JavaScript/TypeScript

- **[@vercel/og](https://www.npmjs.com/package/@vercel/og)** - Vercel's official OG image generation library using Satori.
- **[satori](https://github.com/vercel/satori)** - Convert HTML/CSS to SVG. Powers Vercel OG.
- **[puppeteer](https://github.com/puppeteer/puppeteer)** - Headless Chrome for screenshot-based OG generation.
- **[playwright](https://github.com/microsoft/playwright)** - Cross-browser automation, alternative to Puppeteer.
- **[node-canvas](https://github.com/Automattic/node-canvas)** - Cairo-backed Canvas implementation for Node.js.
- **[sharp](https://github.com/lovell/sharp)** - High-performance image processing, useful for post-processing OG images.

### Python

- **[Pillow](https://pillow.readthedocs.io/)** - Python Imaging Library fork. Standard for image generation.
- **[imgkit](https://github.com/jarrekk/imgkit)** - HTML to image using wkhtmltoimage.
- **[playwright-python](https://github.com/microsoft/playwright-python)** - Python version of Playwright.

### Go

- **[gg](https://github.com/fogleman/gg)** - 2D rendering library for Go.
- **[go-chart](https://github.com/wcharczuk/go-chart)** - Chart library that can output images.

### Ruby

- **[ruby-vips](https://github.com/libvips/ruby-vips)** - Ruby bindings for libvips image processing.
- **[mini_magick](https://github.com/minimagick/minimagick)** - Ruby wrapper for ImageMagick.

## Frameworks with Built-in Support

- **[Next.js](https://nextjs.org/docs/app/api-reference/file-conventions/metadata/opengraph-image)** - Built-in OG image generation with `opengraph-image.tsx`.
- **[Astro](https://docs.astro.build/en/guides/images/#generating-og-images)** - Static site generator with OG image recipes.
- **[SvelteKit](https://kit.svelte.dev/)** - Use with satori or puppeteer.
- **[Remix](https://remix.run/)** - Use resource routes for OG generation.

## Templates

- **[OG Image Playground](https://og-playground.vercel.app/)** - Vercel's interactive playground for designing OG images.
- **[Figma OG Image Templates](https://www.figma.com/community/search?model_type=hub_files&q=og%20image)** - Community templates on Figma.
- **[Canva Social Media Templates](https://www.canva.com/templates/?query=social-media-preview)** - Drag-and-drop templates.

## Best Practices

### Image Specifications

| Platform | Recommended Size | Aspect Ratio |
|----------|-----------------|--------------|
| Twitter/X | 1200×628 | 1.91:1 |
| Facebook | 1200×630 | 1.91:1 |
| LinkedIn | 1200×627 | 1.91:1 |
| Discord | 1200×630 | 1.91:1 |
| Slack | 1200×630 | 1.91:1 |

### Essential Meta Tags

```html
<meta property="og:image" content="https://example.com/og.png" />
<meta property="og:image:width" content="1200" />
<meta property="og:image:height" content="630" />
<meta property="og:image:alt" content="Description of image" />
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:image" content="https://example.com/og.png" />
```

### Tips

1. **Always use 1200×630** - It's the universal safe size.
2. **Keep text large** - Text should be readable at thumbnail size.
3. **Use contrast** - Ensure text stands out from background.
4. **Include branding** - Add logo or consistent visual identity.
5. **Test everywhere** - Use validators to check appearance.

## Articles

- [The Open Graph Protocol](https://ogp.me/) - Official specification.
- [Twitter Cards Documentation](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards) - Twitter-specific requirements.
- [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) - Debug and preview OG tags.
- [LinkedIn Post Inspector](https://www.linkedin.com/post-inspector/) - Test LinkedIn previews.
- [How to Build an OG Image Generator](https://vercel.com/blog/introducing-vercel-og-image-generation-fast-dynamic-social-card-images) - Vercel's guide.

## Validators & Testing Tools

- **[OpenGraph.xyz](https://www.opengraph.xyz/)** - Preview OG images across platforms.
- **[Meta Tags Tester](https://metatags.io/)** - Test and generate meta tags.
- **[Twitter Card Validator](https://cards-dev.twitter.com/validator)** - Test Twitter card appearance.
- **[Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/)** - Debug Facebook sharing.

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
