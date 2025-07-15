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
├── firebase.json           # Firebase hosting config
└── README.md
```

## 🌐 Deployment Options

### Option 1: Firebase Hosting (Recommended)

Firebase Hosting is already configured for this project.

#### Prerequisites
- [Node.js](https://nodejs.org/) installed
- [Firebase CLI](https://firebase.google.com/docs/cli) installed

#### Setup Steps

1. **Install Firebase CLI** (if not already installed):
   ```bash
   npm install -g firebase-tools
   ```

2. **Login to Firebase**:
   ```bash
   firebase login
   ```

3. **Initialize Firebase project** (if not already done):
   ```bash
   firebase init hosting
   ```
   - Select or create a Firebase project
   - Choose `public` as your public directory (already configured)
   - Configure as single-page app: No
   - Set up automatic builds: No

4. **Deploy to Firebase**:
   ```bash
   firebase deploy
   ```

5. **Your site will be live at**: `https://your-project-id.web.app`

#### Quick Deploy Command
```bash
# Deploy with one command
firebase deploy --only hosting
```

### Option 2: Netlify

1. **Via Git Integration**:
   - Connect your GitHub repository to [Netlify](https://netlify.com)
   - Set build directory to `public`
   - Deploy automatically on git push

2. **Via Drag & Drop**:
   - Go to [Netlify](https://netlify.com)
   - Drag the `public` folder to the deploy area

### Option 3: Vercel

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   ```bash
   vercel --prod
   ```
   - Set output directory to `public`

### Option 4: GitHub Pages

1. **Enable GitHub Pages** in your repository settings
2. **Set source** to `/ (root)` and create an `index.html` in root, or:
3. **Move contents** of `public/` to root directory

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

- **Firebase**: Configured in `firebase.json`
- **Styling**: Uses Tailwind CSS via CDN
- **Assets**: Stored in `public/assets/`

## 📞 Contact

For questions about this website, contact Sue Ye via the booking link on the site.