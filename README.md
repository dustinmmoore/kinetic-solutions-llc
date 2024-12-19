# Kinetic Solutions LLC Website

Professional single-page website built with modern web technologies.

## Quick Start

```bash
git clone https://github.com/dustin-moore/kinetic-solutions-llc.git
cd kinetic-solutions-llc
npm install
# Use VS Code Live Server to run locally
```

## Development Stack

- **Frontend Framework:** Bootstrap 4 with custom SASS
- **JavaScript:** Vanilla JS with jQuery for DOM manipulation
- **API Integration:** Google Calendar API for scheduling
- **Deployment:** Vercel with automatic builds
- **Version Control:** Git with branch protection

## Project Architecture

```
src/
├── assets/
│   ├── css/
│   │   ├── style.css      # Core styles
│   │   └── custom.css     # Custom components
│   ├── js/
│   │   ├── main.js       # App logic
│   │   └── plugins.js    # Third-party integrations
│   └── images/          # Optimized assets
└── index.html          # Single-page application
```

## Key Features

- **Responsive Design:** Mobile-first approach using Bootstrap grid
- **Performance:** 
  - Lazy loading images
  - Minified assets
  - WebP image format
  - CDN for libraries
- **Calendar Integration:** Dynamic class scheduling
- **SEO Optimization:** Meta tags and semantic HTML
- **Cross-browser Support:** Modern browser compatibility

## Development Workflow

1. **Setup Environment:**
   ```bash
   nvm use 14  # Ensure correct Node version
   npm install # Install dependencies
   ```

2. **Local Development:**
   - Use VS Code with Live Server
   - SASS watch: `npm run sass:watch`
   - Prettier formatting: `npm run format`

3. **API Configuration:**
   ```javascript
   // main.js
   const CALENDAR_CONFIG = {
     apiKey: process.env.GOOGLE_API_KEY,
     calendarId: process.env.CALENDAR_ID
   };
   ```

4. **Deployment:**
   - Push to main triggers auto-deploy
   - Manual deploy: `npm run deploy`
   - Preview URL generated for PRs

## Contributing

1. Create feature branch: `feature/name`
2. Follow style guide and conventions
3. Write meaningful commit messages
4. Submit PR with description
5. Wait for CI checks and review

## Testing

Current Lighthouse Scores:
- Performance: 78
- Accessibility: 82
- Best Practices: 87
- SEO: 90

Areas for Improvement:
- Image optimization needed
- Reduce unused JavaScript
- Implement better caching strategy
- Add missing alt tags
- Fix contrast issues

## Environment Variables

```env
GOOGLE_API_KEY=your_api_key
CALENDAR_ID=your_calendar_id
VERCEL_TOKEN=deployment_token
```

## Maintenance

- Regular dependency updates
- Performance monitoring
- Analytics review
- Content updates via CMS
- SSL certificate renewal

## Support

Contact: training.kinetic.solutions@gmail.com
Issues: GitHub issue tracker
