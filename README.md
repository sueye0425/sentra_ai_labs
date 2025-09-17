# Sentra AI Labs

Sue Ye's AI consulting company website - showcasing AI-powered products and professional services.

## 🚀 Quick Start

This is a static website built with HTML, CSS (Tailwind), and JavaScript. The site features:

- **Products**: TripAIbuddy - AI-powered travel companion
- **Case Studies**: Technical blog posts and project logs
- **About**: Sue's professional background and expertise

## 📁 Project Structure

```
sentra_ai_labs/
├── public/
│   ├── index.html          # Main landing page
│   ├── meet-sue.html       # About/bio page
│   ├── assets/
│   │   └── profile_photo.JPG
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
- **Styling**: Uses Tailwind CSS via CDN
- **Assets**: Stored in `public/assets/`

## 📞 Contact

For questions about this website, contact Sue Ye via the booking link on the site.