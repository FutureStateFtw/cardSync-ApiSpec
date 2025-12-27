# CardSync API Specification

OpenAPI specification for the FutureState CardSync system API - a credential management system for physical and digital credentials.

## 📖 Documentation

View the interactive API documentation here: **[https://futurestateftw.github.io/cardSync-ApiSpec/](https://futurestateftw.github.io/cardSync-ApiSpec/)**

## 📁 Repository Contents

- `openapi.yaml` - OpenAPI 3.1.0 specification for the CardSync API
- `index.html` - Redoc-based documentation viewer
- `.github/workflows/deploy-docs.yml` - GitHub Actions workflow for automatic deployment

## 🚀 Features

The CardSync API provides endpoints for:

- **Credential Management** - Create, update, and retrieve person credentials
- **Device Information** - Query devices by card number
- **Mealplan Accounts** - Access mealplan balances and swipe accounts
- **Photo Services** - Retrieve and check person photos
- **Replay Functionality** - Resend credential records to downstream systems

## 🔐 Authentication

All API operations require an API key passed via the `X-API-Key` header.

## 🛠️ Local Development

To view the documentation locally:

1. Clone this repository
2. Start a local web server in the repository directory:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```
3. Open `http://localhost:8000` in your browser

## 📝 Making Changes

The documentation automatically deploys to GitHub Pages when changes are pushed to the `main` branch.

1. Edit `openapi.yaml`
2. Commit and push your changes
3. GitHub Actions will automatically redeploy the documentation

## 🔗 API Base URL

Production: `https://valar.api.futurestate.cloud/cardsync`

## 📄 License

FutureState CardSync API Specification
