# Quick Customization Checklist

Use this checklist to quickly customize your portfolio with your own information.

## Personal Information

- [ ] **Name**: Update "NASH NAPULI" → your name
  - Location: navbar, footer
  - Search: `NASH NAPULI` in index.html

- [ ] **Email**: Update email address
  - Current: `nash.napuli@example.com`
  - Footer & contact section

- [ ] **Location**: Update "San Francisco, CA"
  - Contact section

- [ ] **Bio**: Update the About section
  - Replace paragraph text with your bio

## Images

- [ ] Replace `portrait.png` with your photo
  - Recommended size: 420x500px
  - Format: JPG or PNG

- [ ] Replace `project1.png`, `project2.png`, `project3.png`
  - Recommended size: 800x600px
  - These are displayed in project grid

## Projects

Edit `projects.js` and add/update your projects:

```javascript
{
  id: "unique-id",
  title: "Your Project Title",
  year: "2024",
  tags: ["Technology", "Another Tech"],
  shortDesc: "One-line description shown in grid",
  longDesc: "Detailed description shown in modal",
  image: "./project1.png",
  demoLink: "https://live-demo-url.com",
  githubLink: "https://github.com/username/repo"
}
```

**Template for new project:**
```javascript
{
  id: "your-project-id",
  title: "Your Awesome Project",
  year: "2024",
  tags: ["React", "Node.js", "MongoDB"],
  shortDesc: "A brief one-liner about what the project does.",
  longDesc: "A detailed explanation of the project. What problem did it solve? What technologies were used? What was the impact?",
  image: "./project1.png",
  demoLink: "#",  // Replace with live URL
  githubLink: "#"  // Replace with GitHub repo URL
}
```

**Current projects to update:**
- [ ] Quantum Analytics Dashboard
- [ ] Nexus Core Protocol
- [ ] Neural Synthesizer
- [ ] Velocity Engine
- [ ] Ethereal Mesh Network
- [ ] Solstice Web Framework

## Skills & Experience

### About Section
- [ ] Update programming languages list
- [ ] Update tools & technologies list

### Experience Timeline
Edit the 4 timeline items:
- [ ] 2024: Sr. Systems Engineer (or your current role)
- [ ] 2023: Full-Stack Engineer (or relevant experience)
- [ ] 2022: Junior Developer
- [ ] 2021: CS Graduate

Template for timeline entry:
```html
<div class="relative group">
  <div class="absolute -left-4 md:left-1/2 top-4 w-8 h-8 bg-secondary/20 border-2 border-secondary rounded-full..."></div>
  <div class="pl-6 md:pl-0 md:pr-6 md:text-right">
    <h3 class="font-headline-md...">YEAR</h3>
    <p class="text-secondary...">Your Role</p>
    <p class="text-on-surface-variant...">Your description</p>
  </div>
</div>
```

## Blog/Articles

Edit the 3 blog cards in the blog section:

Template:
```html
<article class="group bg-surface-container-low...">
  <div class="mb-4">
    <span class="bg-secondary/10...">CATEGORY</span>
  </div>
  <h3 class="font-headline-md...">Your Article Title</h3>
  <p class="text-body-md...">Brief description of your article</p>
  <span class="font-code-label...">DATE, 2026</span>
</article>
```

Current blog topics to update:
- [ ] Building Fault-Tolerant Microservices
- [ ] WebAssembly for Real-Time Processing
- [ ] Designing for Scale from Day One

## Social Media Links

Update in the footer:

- [ ] **GitHub**: `https://github.com/YOUR_USERNAME`
- [ ] **LinkedIn**: `https://linkedin.com/in/YOUR_PROFILE`
- [ ] **Email**: `mailto:your@email.com`
- [ ] **Twitter/X**: `https://x.com/YOUR_HANDLE`

## Contact Form Setup

- [ ] Sign up at [formspree.io](https://formspree.io)
- [ ] Create new form and copy Form ID
- [ ] Find this line in index.html:
  ```html
  action="https://formspree.io/f/YOUR_FORM_ID"
  ```
- [ ] Replace `YOUR_FORM_ID` with your actual ID
- [ ] Test by submitting test email

## Color Customization (Optional)

Want to change the color scheme?

1. Find `<script id="tailwind-config">` in index.html
2. Locate the "colors" section
3. Update hex codes:
   - `"secondary": "#4edea3"` → your accent color
   - `"surface": "#031427"` → background color
   - `"on-surface": "#d3e4fe"` → text color

Popular color combinations:
```javascript
// Ocean Blue
"secondary": "#0ea5e9"  // Sky blue
"surface": "#0f172a"    // Dark blue
"on-surface": "#e0f2fe" // Light blue text

// Purple
"secondary": "#a78bfa"  // Purple
"surface": "#1e1b4b"    // Dark purple
"on-surface": "#ede9fe" // Light text

// Green
"secondary": "#10b981"  // Emerald
"surface": "#0f2e19"    // Dark green
"on-surface": "#d1fae5" // Light green text
```

## SEO Customization

- [ ] Update page title in `<title>` tag
- [ ] Update meta description in `<meta name="description">`
- [ ] Update Open Graph tags for social sharing

```html
<title>Your Name - Your Title</title>
<meta name="description" content="What you do and what makes you unique">
<meta property="og:title" content="Your Portfolio">
<meta property="og:description" content="Brief description">
```

## Deployment

- [ ] Set up GitHub repository
- [ ] Deploy to Netlify or Vercel (see DEPLOYMENT_GUIDE.md)
- [ ] Set up custom domain (optional)
- [ ] Enable analytics (Google Analytics)
- [ ] Add to portfolio platforms (dev.to, GitHub, etc.)

## Testing

- [ ] Test on mobile (use DevTools or real device)
- [ ] Test form submission
- [ ] Check all links work
- [ ] Test all navigation
- [ ] Verify images load
- [ ] Check animations on different browsers

## Final Checks

Before going live:
- [ ] All personal info updated
- [ ] All images replaced
- [ ] All projects added
- [ ] All social links updated
- [ ] Contact form working
- [ ] Mobile responsive
- [ ] No broken links
- [ ] No console errors
- [ ] Performance is good

---

**Need help?** Check:
- README.md - Full documentation
- DEPLOYMENT_GUIDE.md - How to go live
- index.html - HTML structure
- projects.js - Project data

**Your portfolio is almost ready! 🎉**
