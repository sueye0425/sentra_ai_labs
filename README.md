# Cocoo - Smart Baby Tracking App

Developed by Sentra AI - A comprehensive mobile app for modern parents to track their baby's daily activities, sleep patterns, feeding schedules, and developmental milestones.

## 🚀 Quick Start

This is a static website built with HTML, CSS (Tailwind), and JavaScript showcasing the Cocoo mobile app. The site features:

- **App Overview**: Complete baby tracking solution with 7-sticker system
- **Features**: Sleep tracking, feeding logs, diaper changes, developmental milestones
- **Screenshots**: Visual previews of the mobile app interface
- **Download**: App store links and waitlist signup (coming soon)
- **About**: Sentra AI as the development company

## 📁 Project Structure

```
sentra_ai_labs/
├── public/
│   ├── index.html          # Cocoo app landing page
│   ├── meet-sue.html       # About/bio page (legacy)
│   ├── assets/
│   │   ├── cocoo-logo.png          # Cocoo app logo
│   │   ├── cocoo-full-logo.png     # Cocoo full logo
│   │   ├── baby_sleep.png          # App screenshot assets
│   │   ├── baby_breastfeed.png     # App screenshot assets
│   │   ├── wakeup_baby.png         # App screenshot assets
│   │   └── profile_photo.JPG       # Sue's photo (legacy)
│   └── 404.html
├── netlify.toml           # Netlify hosting config
├── _redirects             # Netlify redirects
└── README.md
```

## 🌐 Deployment

### Netlify Hosting (Current Setup)

This project is configured for deployment on Netlify with automatic builds and optimized caching.

#### Quick Deploy Options

1. **Via Git Integration** (Recommended):
   - Connect your GitHub repository to [Netlify](https://netlify.com)
   - Netlify will automatically detect the `netlify.toml` configuration
   - Deploy automatically on git push to main branch

2. **Via Netlify CLI**:
   ```bash
   # Install Netlify CLI
   npm install -g netlify-cli
   
   # Login to Netlify
   netlify login
   
   # Deploy to production
   netlify deploy --prod
   ```

3. **Via Drag & Drop**:
   - Go to [Netlify](https://netlify.com)
   - Drag the `public` folder to the deploy area

#### Configuration Files
- `netlify.toml`: Build settings, headers, and redirects
- `_redirects`: Additional redirect rules

### Alternative Deployment Options

#### Vercel
```bash
npm install -g vercel
vercel --prod
```

#### GitHub Pages
1. Enable GitHub Pages in repository settings
2. Set source to `/ (root)` or move `public/` contents to root

## 🛠️ Local Development

To run locally, simply serve the `public` directory:

```bash
# Using Python
cd public
python -m http.server 8000

# Using Node.js
npx serve public

# Using PHP
cd public
php -S localhost:8000
```

Then visit `http://localhost:8000`

## 📝 Making Changes

1. Edit HTML files in the `public/` directory
2. Test changes locally
3. Deploy using your preferred method above

## 🔧 Configuration

- **Netlify**: Configured in `netlify.toml` and `_redirects`
- **Styling**: Uses Tailwind CSS via CDN with Cocoo's warm color palette
- **Assets**: App logos and screenshots stored in `public/assets/`
- **Design**: Cream (#F4EAE1) and pink (#E26887) color scheme matching the mobile app

## 📱 About Cocoo

Cocoo is a comprehensive baby tracking mobile app that helps new parents:

- **Track 7 Essential Activities**: Sleep, wake-up, breastfeeding, formula, pee, poop, and combination diaper changes
- **Expert Sleep Templates**: Age-appropriate schedules for babies 0-24 months based on pediatric guidelines
- **Timeline Visualization**: Beautiful daily timeline showing all activities at a glance
- **Developmental Milestones**: Track progress using AAP/WHO standards
- **Smart Analytics**: Drift analysis and personalized schedule recommendations
- **Intuitive Interface**: Simple sticker-based tracking designed for tired parents

## 🏢 About Sentra AI

Cocoo is developed by Sentra AI, a company specializing in AI-powered solutions that solve real-world problems. For questions about this website or Sentra AI services, contact Sue Ye via the booking link on the site.

## 🔗 Related Repositories

- [cocoo-frontend-flutter](../cocoo-frontend-flutter/): Flutter mobile app source code
- [cocoo-backend](../cocoo-backend/): FastAPI backend with expert sleep templates