# Eleventy Template for QuantCDN

A simple Eleventy static site template ready for deployment to QuantCDN.

[![Deploy to QuantCDN](https://www.quantcdn.io/img/quant-deploy-btn-sml.svg)](https://dashboard.quantcdn.io/projects/add/jamstack?template=eleventy)

## Features

- Eleventy 3.x (latest)
- Nunjucks and Markdown templates
- Zero client-side JavaScript
- Minimal configuration
- Fast build times

## Local Development

```bash
# Install dependencies
npm install

# Start development server with hot reload
npm start

# Build for production
npm run build
```

The development server runs at `http://localhost:8080`.

## Project Structure

```
ssg-eleventy/
├── src/
│   ├── _includes/
│   │   └── layout.njk      # Base layout template
│   ├── index.njk           # Homepage
│   └── about.md            # About page
├── eleventy.config.js      # Eleventy configuration
├── package.json
└── README.md
```

## Deployment

This template includes a GitHub Actions workflow that automatically builds and deploys your site to QuantCDN when you push to the main branch.

### Required Secrets

Add these secrets to your GitHub repository:

- `QUANT_CUSTOMER` - Your QuantCDN customer ID
- `QUANT_PROJECT` - Your QuantCDN project name
- `QUANT_TOKEN` - Your QuantCDN API token

## Learn More

- [Eleventy Documentation](https://www.11ty.dev/docs/)
- [QuantCDN Documentation](https://docs.quantcdn.io/)
