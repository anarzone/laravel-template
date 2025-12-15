# Laravel API Starter Template

[![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)](https://semver.org)
[![PHP](https://img.shields.io/badge/PHP-8.4+-777BB4.svg)](https://www.php.net/)
[![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20.svg)](https://laravel.com)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

A clean Laravel 12 starter template for building modern RESTful APIs with CI/CD workflows.

## What's Included

- Laravel 12
- Laravel Sanctum (optional)
- API Routes configured
- Pest Testing Framework
- Laravel Pint (Code Formatter)
- Laravel Sail (Docker Environment)
- Vite
- GitHub Actions CI/CD workflows

## Quick Start

```bash
# Install dependencies and setup
composer setup

# Start development server
composer dev

# Run tests
composer test

# Format code
vendor/bin/pint
```

## API Structure

- `routes/api.php` - API routes (prefixed with `/api`)
- `routes/web.php` - Web routes
- `GET /` - Returns JSON with app info

## GitHub Workflows

This template includes pre-configured GitHub Actions workflows:

- **CI Pipeline** (`.github/workflows/ci.yml`) - Code quality, tests, and asset building
- **Pull Request Checks** (`.github/workflows/pull-request.yml`) - PR validation and automated comments
- **Deploy to Forge** (`.github/workflows/deploy.yml`) - Automated deployment to Laravel Forge

### Setting Up Workflows

1. **CI Pipeline**: Works out of the box - runs on push/PR to main/develop
2. **Deploy Workflow**: Requires GitHub secrets:
   - `FORGE_API_TOKEN` - Your Laravel Forge API token
   - `FORGE_SERVER_ID` - Your Forge server ID
   - `FORGE_SITE_URL` - Your production domain (as variable)

## Versioning

This project follows [Semantic Versioning](https://semver.org/). Current version: **0.1.0**

## License

[MIT license](https://opensource.org/licenses/MIT)
