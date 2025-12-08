# Pre-Launch Checklist for Tabba Marketing Site

## ✅ Completed

### Favicons & Icons
- ✅ Favicon.ico (16x16, 32x32, 48x48)
- ✅ Favicon.png for modern browsers
- ✅ Apple touch icon (180x180)
- ✅ All favicon links added to index.html, privacy.html, and terms.html

### Open Graph & Social Sharing
- ✅ Open Graph meta tags (title, description, image, url, type)
- ✅ Twitter Card meta tags
- ✅ OG image dimensions specified (1200x630)
- ✅ Added to all pages (index, privacy, terms)

### SEO & Meta Tags
- ✅ Canonical URLs for all pages
- ✅ Theme color meta tag
- ✅ Language tag (lang="en")
- ✅ Meta description for all pages
- ✅ Robots meta tags
- ✅ Google site verification placeholder

### Analytics
- ✅ Umami analytics integrated
- ✅ Waitlist signup event tracking

## 🔲 To Do Before Launch

### Images Required
- [x] **Create `assets/og-image.png`** (1200x630px)
  - Should be a high-quality preview image for social sharing
  - Include Tabba branding/logo
  - Recommended: Screenshot of the extension or hero graphic

### Technical Setup
- [x] **Create `robots.txt`** in root directory
  ```
  User-agent: *
  Allow: /
  Sitemap: https://tabba.so/sitemap.xml
  ```

- [x] **Create `sitemap.xml`** in root directory
  - Include: index.html, privacy.html, terms.html
  - Set proper priorities and change frequencies

- [x] **Set up 404 page** (`404.html`)
  - Match site design
  - Include navigation back to home

- [x] **Verify Google Site Verification**
  - Domain verified in Google Search Console
  - Placeholder meta tag removed (verification complete via Search Console)

### Performance
- [ ] **Optimize images**
  - Compress hero.png and video thumbnails
  - Consider WebP format with fallbacks
  - Lazy load images below the fold

- [ ] **Optimize videos**
  - Ensure MP4 files are compressed
  - Consider adding poster images for videos

- [ ] **Minify CSS** (optional, for production)
  - Current CSS files are readable for development

### Security & Headers
- ✅ **Set up security headers** (via meta tags - GitHub Pages limitation)
  - ✅ Content-Security-Policy (added to all pages)
  - ✅ X-Frame-Options: DENY (added to all pages)
  - ✅ X-Content-Type-Options: nosniff (added to all pages)
  - ✅ Referrer-Policy: strict-origin-when-cross-origin (added to all pages)
  - Note: GitHub Pages doesn't support custom HTTP headers, so meta tags are used

- ✅ **Enable HTTPS** (automatic with GitHub Pages, but verify)
  - ✅ HTTPS is automatically enabled for all GitHub Pages sites
  - [x] **Action Required**: Go to GitHub repo → Settings → Pages → Verify "Enforce HTTPS" checkbox is enabled
  - [x] **Action Required**: Test that https://tabba.so loads correctly (should redirect HTTP to HTTPS automatically)

### Accessibility
- [ ] **Test with screen readers**
- [ ] **Verify keyboard navigation**
- [ ] **Check color contrast ratios**
- [ ] **Add ARIA labels where needed** (most already present)

### Testing
- [ ] **Test on multiple browsers**
  - Chrome, Firefox, Safari, Edge
  - Mobile browsers (iOS Safari, Chrome Mobile)

- [ ] **Test form submissions**
  - Verify Formspree integration works
  - Test error handling
  - Verify Umami tracking fires

- [ ] **Test responsive design**
  - Mobile (320px+)
  - Tablet (768px+)
  - Desktop (1024px+)

- [ ] **Test social sharing**
  - Use Facebook Debugger: https://developers.facebook.com/tools/debug/
  - Use Twitter Card Validator: https://cards-dev.twitter.com/validator
  - Use LinkedIn Post Inspector: https://www.linkedin.com/post-inspector/

### Content Review
- [ ] **Proofread all copy**
- [ ] **Verify all links work**
- [ ] **Check email addresses** (hey@tabba.so)
- [ ] **Verify privacy.html and terms.html content is complete**

### Domain & DNS
- [x] **Set up custom domain** (tabba.so)
  - Configure DNS records
  - Update CNAME file (already exists)
  - Verify domain points to GitHub Pages

- [x] **Set up email** (if needed for hey@tabba.so)
  - Configure email forwarding or mailbox

### Legal
- [x] **Finalize Privacy Policy content**
- [x] **Finalize Terms of Service content**
- [ ] **Add any required disclaimers**

### Optional Enhancements
- [x] **Add structured data (JSON-LD)** for rich snippets
  - ✅ WebSite schema (basic site information)
  - ✅ SoftwareApplication schema (Chrome extension with features, pricing, OS support)
  - Note: Organization schema skipped to keep it minimal (can add later if needed)

- [ ] **Add RSS feed** (if planning blog/content)

- [x] **Set up email list** (Formspree integration already done)

## Quick Launch Checklist

Before going live, ensure:
1. ✅ All favicons are in place
2. ✅ OG image is created and uploaded
3. ✅ robots.txt and sitemap.xml are created
4. ✅ All forms tested and working
5. ✅ Analytics tracking verified
6. ✅ Domain configured and SSL active
7. ✅ All pages load correctly
8. ✅ Mobile responsive design verified
9. ✅ Social sharing previews look good

## Post-Launch

- Monitor Umami analytics for traffic
- Track waitlist signups
- Monitor Formspree for form submissions
- Set up Google Search Console
- Submit sitemap to search engines
- Monitor for 404 errors

