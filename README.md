# Nash Napuli - Portfolio Website

A modern, high-performance portfolio showcasing engineering projects, experience, and technical expertise. Built with vanilla JavaScript and Tailwind CSS for maximum performance and customizability.

## Features

✨ **Modern Design**
- Dark theme with custom Tailwind color system
- Smooth animations and scroll effects
- Glassmorphism effects and hover interactions
- Fully responsive mobile-first design

🎯 **Key Sections**
- Hero section with portrait
- Dynamic project grid with modal details
- Experience/timeline section
- About section with skills
- Blog/articles preview
- Contact form with email integration
- Social media links

⚡ **Performance**
- Lightweight (no heavy frameworks)
- Fast load times
- SEO optimized with meta tags
- Intersection Observer for scroll animations

📱 **Responsive**
- Mobile-first design
- Tablet and desktop optimized
- Touch-friendly navigation

---

## File Structure

```
NashPortfolio/
├── index.html          # Main HTML file with all sections
├── projects.js         # Project data (easily customizable)
├── portrait.png        # Hero section image
├── project1.png        # Project images
├── project2.png
├── project3.png
├── DEPLOYMENT_GUIDE.md # How to deploy online
└── README.md          # This file
```

---

## Quick Start

### 1. Customize Your Content

**Update Personal Info:**
Edit `index.html`:
```html
<a class="font-headline-md...">NASH NAPULI</a> <!-- Change name -->
<span class="material-symbols-outlined">mail</span>
<span class="text-on-surface-variant font-code-label text-sm">nash.napuli@example.com</span> <!-- Change email -->
```

**Update Projects:**
Edit `projects.js` - Add/edit project objects:
```javascript
{
  id: "project-id",
  title: "Your Project Title",
  year: "2024",
  tags: ["Tech1", "Tech2"],
  shortDesc: "Brief description",
  longDesc: "Detailed description",
  image: "./project1.png",
  demoLink: "https://demo.com",
  githubLink: "https://github.com/yourrepo"
}
```

**Update About Section:**
Edit the About section in `index.html`:
```html
<p class="text-body-lg text-on-surface-variant leading-relaxed">
  Your bio here...
</p>
```

**Update Skills:**
Edit the skills boxes in the About section:
```html
<h4 class="font-code-label text-secondary...">Languages</h4>
<ul class="text-on-surface-variant space-y-xs text-sm">
  <li>Your Language</li>
  <!-- Add more -->
</ul>
```

### 2. Add/Replace Images

1. Replace `portrait.png` with your photo
2. Replace `project1.png`, `project2.png`, `project3.png` with your project screenshots
3. Keep image sizes roughly:
   - Portrait: 420x500px
   - Projects: 800x600px

### 3. Update Social Links

In the footer (`index.html`), update these links:
```html
<a href="https://github.com/YOUR_USERNAME">GitHub</a>
<a href="https://linkedin.com/in/YOUR_PROFILE">LinkedIn</a>
<a href="mailto:your@email.com">Email</a>
<a href="https://x.com/YOUR_HANDLE">Twitter</a>
```

### 4. Setup Email Form

See `DEPLOYMENT_GUIDE.md` for Formspree setup instructions.

---

## Customization Guide

### Color Scheme

Colors are defined in `<script id="tailwind-config">` in `index.html`:

```javascript
"colors": {
  "secondary": "#4edea3",  // Primary accent color
  "primary": "#bec6e0",    // Primary color
  "surface": "#031427",    // Background
  "on-surface": "#d3e4fe", // Text
  // ... more colors
}
```

**To change theme:**
1. Keep the structure but change hex values
2. Use a color picker tool
3. Test for contrast (accessibility)

### Fonts

Edit in `<script id="tailwind-config">`:
```javascript
"fontFamily": {
  "display-xl": ["Your Font Name"],
  "headline-lg": ["Your Font Name"],
  // ...
}
```

Currently uses: Hanken Grotesk & JetBrains Mono

### Animations

Animations are defined in `<style>` tag:
- `fade-in-up` - Fade and slide up
- `pulse-glow` - Glowing pulse effect

Add new animations:
```css
@keyframes yourAnimation {
  0% { /* start */ }
  100% { /* end */ }
}
```

### Typography Sizes

Change in Tailwind config:
```javascript
"fontSize": {
  "display-xl": ["72px", { "lineHeight": "1.1", ... }],
  // ...
}
```

---

## Adding New Sections

To add a new section (e.g., "Services"):

1. **Add HTML** before `</main>`:
```html
<section class="max-w-[1280px] mx-auto px-gutter py-2xl" id="services">
  <h2 class="font-headline-lg text-headline-lg text-on-surface">Your Section</h2>
  <!-- Content here -->
</section>
```

2. **Add nav link** in the navbar:
```html
<a href="#services">SERVICES</a>
```

3. **Add to footer navigation**

---

## Development Tips

### Local Testing
1. Open `index.html` in your browser
2. Changes auto-reflect (just refresh)
3. No build step needed!

### Browser DevTools
- Use Chrome DevTools for responsive testing
- Check console for any errors
- Test on mobile devices

### Performance
- Keep images optimized
- Avoid heavy JavaScript libraries
- Monitor Core Web Vitals

---

## Deployment

See `DEPLOYMENT_GUIDE.md` for complete deployment instructions.

**Quick Deploy to Netlify:**
```bash
# 1. Create GitHub repo
git init
git add .
git commit -m "Initial commit"
git push -u origin main

# 2. Connect to Netlify
# - Go to netlify.com
# - Drag & drop folder OR connect GitHub repo
# - Done!
```

---

## SEO Optimization

Already included:
- ✅ Meta descriptions
- ✅ Open Graph tags
- ✅ Semantic HTML
- ✅ Mobile responsive
- ✅ Fast load times

To improve further:
1. Add Google Analytics
2. Submit sitemap to Google Search Console
3. Get backlinks from dev.to, Twitter
4. Write blog posts

---

## Browser Support

Works on:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## Troubleshooting

**Form not sending emails?**
- Check Formspree setup in DEPLOYMENT_GUIDE.md
- Ensure form ID is correct in HTML

**Images not loading?**
- Check file paths are correct
- Ensure image files are in same directory

**Animations not working?**
- Check browser console for errors
- Ensure CSS is loaded
- Try clearing browser cache

**Mobile layout broken?**
- Test in DevTools responsive mode
- Check Tailwind responsive classes (md:, lg:)
- Adjust spacing/padding if needed

---

## Performance Metrics

Target metrics:
- Lighthouse score: 90+
- First Contentful Paint: <2s
- Largest Contentful Paint: <2.5s
- Cumulative Layout Shift: <0.1

---

## Accessibility

The portfolio includes:
- ✅ Semantic HTML
- ✅ ARIA labels
- ✅ Keyboard navigation
- ✅ Color contrast compliance
- ✅ Alt text for images

---

## License

Feel free to use and customize! Credit appreciated but not required.

---

## Support Resources

- **Tailwind CSS**: https://tailwindcss.com/docs
- **MDN Web Docs**: https://developer.mozilla.org
- **Web Dev Best Practices**: https://web.dev
- **Formspree**: https://formspree.io/docs

---

## Next Steps

1. ✏️ Customize content with your information
2. 🖼️ Replace images with your own
3. 🎨 Adjust colors to match your brand
4. 🚀 Deploy to web (see DEPLOYMENT_GUIDE.md)
5. 📊 Add analytics and monitoring
6. 📝 Keep blog/articles updated

---

**Built with ❤️ for ambitious engineers.**

Portfolio Version: 2.0
Last Updated: 2026-06-11
