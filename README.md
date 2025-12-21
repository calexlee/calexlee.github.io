# C. Alex Lee - Personal Website

A sleek, modern personal portfolio website with responsive design.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern Aesthetic**: Dark theme with subtle gradient orbs and noise texture
- **Smooth Animations**: Fade-in effects and hover interactions
- **Single Page**: All content in one smooth-scrolling page
- **No Dependencies**: Pure HTML, CSS, and vanilla JavaScript

## Files

```
personal-website/
├── index.html    # Main website file
├── profile.jpg   # Your profile photo
└── README.md     # This file
```

## Deploying to GitHub Pages

### Option 1: Deploy from Main Branch (Recommended)

1. **Create a new repository on GitHub**
   - Go to [github.com/new](https://github.com/new)
   - Name it `personal-website` (or any name you prefer)
   - Keep it public
   - Don't initialize with README (we already have files)

2. **Push your code to GitHub**
   ```bash
   cd personal-website
   git init
   git add .
   git commit -m "Initial commit: Personal website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/personal-website.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages** (in the left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

4. **Access your site**
   - Your site will be live at: `https://YOUR_USERNAME.github.io/personal-website/`
   - It may take 1-2 minutes for the first deployment

### Option 2: Use Your Username Repository (for calexlee.github.io)

If you want your site at `https://calexlee.github.io/`:

1. Create a repository named exactly `calexlee.github.io`
2. Push these files to the main branch
3. GitHub Pages will automatically deploy it

### Option 3: Custom Domain (www.calexlee.com)

To use your custom domain:

1. **In your GitHub repository settings:**
   - Go to **Settings** → **Pages**
   - Under "Custom domain", enter `www.calexlee.com`
   - Click **Save**
   - Check "Enforce HTTPS" once the DNS is configured

2. **Configure your DNS (at your domain registrar):**
   
   Add these records:

   | Type  | Name | Value |
   |-------|------|-------|
   | CNAME | www  | calexlee.github.io |
   | A     | @    | 185.199.108.153 |
   | A     | @    | 185.199.109.153 |
   | A     | @    | 185.199.110.153 |
   | A     | @    | 185.199.111.153 |

3. **Create a CNAME file** in your repository:
   ```
   www.calexlee.com
   ```

4. DNS changes can take up to 24-48 hours to propagate.

## Customization

### Changing Colors

Edit the CSS variables at the top of `index.html`:

```css
:root {
    --color-bg: #0a0a0b;           /* Main background */
    --color-accent: #3b82f6;        /* Accent color (blue) */
    --color-text: #fafafa;          /* Main text */
    --color-text-muted: #a1a1a6;    /* Secondary text */
}
```

### Updating Content

All content is in `index.html`. Look for these sections:
- **Hero**: Your name, title, and intro
- **Experience**: Work history cards
- **Skills**: Technical skills tags
- **Education**: Degree information
- **Contact**: Email, phone, and social links

### Changing the Photo

Replace `profile.jpg` with your own image. For best results:
- Use a square or 4:5 aspect ratio image
- Minimum 400px width recommended
- JPG or PNG format

## Browser Support

Works in all modern browsers:
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## License

Feel free to use this template for your own personal website.
