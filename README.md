# press & question

An interactive clicking game with Vercel Web Analytics integration for tracking user engagement.

## Features

- Interactive button clicking game
- Real-time statistics tracking
- Share functionality (via social media or friend link)
- Evolution stages with visual effects
- Vercel Web Analytics integration

## Getting Started

### Prerequisites

- A Vercel account (sign up at [vercel.com](https://vercel.com))
- Vercel CLI installed (optional, for local testing)

### Installation

```bash
# Install Vercel CLI (optional)
npm install -g vercel
```

### Deployment to Vercel

1. Push your code to a Git repository (GitHub, GitLab, or Bitbucket)
2. Go to [Vercel Dashboard](https://vercel.com/dashboard)
3. Click "Add New Project" and select your repository
4. Click "Import" to deploy

Once deployed, Vercel Web Analytics will automatically track:
- Visitor counts
- Page views
- Interaction patterns
- Geographic data
- Browser and device information

### Enable Web Analytics

1. Go to your [Vercel Dashboard](https://vercel.com/dashboard)
2. Select your project
3. Click the **Analytics** tab
4. Click **Enable** to start tracking

## Vercel Web Analytics Integration

This project includes Vercel Web Analytics configured for plain HTML sites. The tracking script is included in `index.html`:

```html
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>
```

### What Gets Tracked

- Page views
- Core Web Vitals (LCP, FID, CLS)
- User interactions
- Performance metrics

### View Analytics

After deployment and once users have visited your site:

1. Go to your Vercel Dashboard
2. Select your project
3. Click the **Analytics** tab
4. View real-time data and historical trends

After a few days of visitors, you'll be able to filter and explore the data in detail.

## Local Development

For local testing:

```bash
# Using http-server (if installed)
npm install -g http-server
http-server

# Or use Python
python -m http.server 8000
```

Then visit `http://localhost:8000`

## Files

- `index.html` - Main HTML file with analytics script
- `script.js` - Game logic and interactivity
- `style.css` - Styling and animations
- `vercel.json` - Vercel deployment configuration
- `.vercelignore` - Files to ignore during deployment
- `package.json` - Project metadata

## Privacy & Compliance

Vercel Web Analytics respects privacy standards and user data protection regulations. For more information, see [Vercel Analytics Privacy Policy](https://vercel.com/docs/analytics/privacy-policy).

## Learn More

- [Vercel Web Analytics Documentation](https://vercel.com/docs/analytics)
- [Vercel Deployment Guide](https://vercel.com/docs/deployments/overview)
- [Custom Events with Web Analytics](https://vercel.com/docs/analytics/custom-events)
