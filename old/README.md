# Momentum Website

Website for Momentum - Team Performance Through Voice, Movement & Connection.

## Project Structure

```
momentum-website/
├── index.html          # Main page
├── css/
│   └── styles.css      # All styles
├── js/
│   └── main.js         # Animations & interactions
├── assets/
│   └── images/         # Photos (add when ready)
├── LAUNCH-CHECKLIST.md # Business launch checklist
└── README.md           # This file
```

## Local Development

Simply open `index.html` in a browser:

```bash
open index.html
```

Or use a local server for best results:

```bash
# Python 3
python -m http.server 8000

# Then visit http://localhost:8000
```

## Deployment to Netlify

### Option 1: Drag & Drop
1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the entire `momentum-website` folder onto the page
3. Done! You'll get a URL like `random-name.netlify.app`

### Option 2: Git Integration (Recommended)
1. Push this folder to a GitHub repository
2. Connect the repo to Netlify
3. Every push will auto-deploy

```bash
# Initialize git
cd momentum-website
git init
git add .
git commit -m "Initial commit"

# Create repo on GitHub, then:
git remote add origin https://github.com/YOUR-USERNAME/momentum-website.git
git push -u origin main
```

## Contact Form

The contact form uses Netlify Forms. Once deployed to Netlify:
- Form submissions appear in your Netlify dashboard
- Set up email notifications in Site Settings > Forms > Form notifications

## Making Changes with Claude Code

This site is designed for easy editing with Claude Code:

1. **CSS changes**: Edit `css/styles.css`
   - Colors are in `:root` CSS variables at the top
   - Each section has clearly labelled styles

2. **Content changes**: Edit `index.html`
   - Sections are clearly commented
   - Team bios, programs, etc. are easy to find

3. **Adding photos**:
   - Place images in `assets/images/`
   - Update the `.team__photo` backgrounds in CSS or add `<img>` tags

## Custom Domain

1. In Netlify: Site Settings > Domain Management > Add custom domain
2. Add DNS records as instructed
3. SSL is automatic

## File Sizes

Keep images optimized:
- Photos: Use WebP format, ~100-200KB each
- Consider lazy loading for below-fold images

## Browser Support

Tested on:
- Chrome (latest)
- Safari (latest)
- Firefox (latest)
- Mobile Safari / Chrome
