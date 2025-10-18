# Different Localhost Configurations

This project now supports multiple localhost configurations for different environments.

## Available Environments

### 1. Development (Default)
- **Port**: 3000
- **API URL**: http://localhost:8081
- **Command**: `npm run dev`

### 2. Staging
- **Port**: 3001
- **API URL**: http://localhost:8082
- **Command**: `npm run dev:staging`

### 3. Production
- **Port**: 3002
- **API URL**: http://localhost:8083
- **Command**: `npm run dev:production`

### 4. Local
- **Port**: 3000
- **API URL**: http://localhost:8081
- **Command**: `npm run dev:local`

## How to Use

1. **Start the frontend with different environments:**
   ```bash
   # Development (default)
   npm run dev
   
   # Staging
   npm run dev:staging
   
   # Production
   npm run dev:production
   
   # Local
   npm run dev:local
   ```

2. **Build for different environments:**
   ```bash
   # Build for staging
   npm run build:staging
   
   # Build for production
   npm run build:production
   ```

3. **Preview builds:**
   ```bash
   # Preview staging build
   npm run preview:staging
   
   # Preview production build
   npm run preview:production
   ```

## Environment Files

The project uses the following environment files:
- `.env.development` - Development configuration
- `.env.staging` - Staging configuration
- `.env.production` - Production configuration
- `.env.local` - Local configuration

## Backend Setup

Make sure your backend servers are running on the corresponding ports:
- Development: http://localhost:8081
- Staging: http://localhost:8082
- Production: http://localhost:8083

## Configuration

You can modify the environment files to change:
- `VITE_PORT` - Frontend port
- `VITE_API_URL` - Backend API URL
- `VITE_APP_TITLE` - Application title

## Access URLs

After starting the development server, you can access the application at:
- Development: http://localhost:3000
- Staging: http://localhost:3001
- Production: http://localhost:3002
- Local: http://localhost:3000
