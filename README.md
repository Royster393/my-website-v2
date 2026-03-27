# Joel Roy — Personal Website

## File Structure

```
joelroy-site/
├── index.html              ← Main page (only HTML file needed)
├── README.md
│
├── css/
│   ├── reset.css           ← Meyer-style reset
│   ├── variables.css       ← All design tokens (colours, spacing, fonts)
│   ├── base.css            ← Body, blobs, shared utilities
│   ├── nav.css             ← Sticky navbar
│   ├── hero.css            ← Hero / landing section
│   ├── portfolio.css       ← Project cards grid
│   ├── skills.css          ← Technical skills section
│   ├── blog.css            ← Blog post list
│   ├── about.css           ← About / bio section
│   ├── contact.css         ← Contact form & social links
│   ├── footer.css          ← Footer
│   └── responsive.css      ← Mobile & tablet breakpoints
│
├── js/
│   ├── blobs.js            ← Mouse parallax on background blobs
│   ├── nav.js              ← Hamburger menu + active link highlight
│   ├── animations.js       ← Scroll-triggered reveal animations
│   ├── contact.js          ← Form validation & submission
│   └── main.js             ← App init, smooth scroll, copyright year
│
└── assets/
    ├── images/
    │   └── (add joel.jpg here for the about section photo)
    └── fonts/
        └── (add any local fonts here if needed)
```

## How to Deploy

### Option 1 — Upload directly to joelroy393.com
1. Upload the entire `joelroy-site/` folder contents to your hosting root
   (so `index.html` lives at the root, not inside a subfolder)
2. Done — visit joelroy393.com

### Option 2 — GitHub Pages (free)
1. Push this folder to a GitHub repo named `yourusername.github.io`
2. Go to Settings → Pages → Deploy from main branch
3. Your site will be live at `yourusername.github.io`

## Customisation Checklist

- [ ] Replace "your photo here ✦" blob in About section:
      In `index.html`, uncomment the `<img>` tag and add `assets/images/joel.jpg`
- [ ] Update blog post titles/dates/excerpts with real posts
- [ ] Hook up the contact form (see `js/contact.js` for Formspree instructions)
- [ ] Update project cards with real descriptions and links
- [ ] Update stat numbers in the Hero section if they change

## Contact Form Setup (Formspree — free tier)
1. Go to https://formspree.io and create a free account
2. Create a new form, copy the endpoint URL
3. Open `js/contact.js`, paste your URL into `FORMSPREE_URL`
4. Uncomment the fetch block under "Option A"

## Colours (edit in css/variables.css)
| Variable           | Value     | Used for            |
|--------------------|-----------|---------------------|
| --color-accent     | #a78bfa   | Purple — primary    |
| --color-accent-2   | #f472b6   | Pink — secondary    |
| --color-accent-3   | #34d399   | Green — security    |
| --color-bg         | #0d0b14   | Page background     |
