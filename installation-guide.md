# Installation Guide for Faculty Tracker PWA

Follow these steps to install the Faculty Application Tracker as a Progressive Web App (PWA) on your home screen:

## Option 1: Using GitHub Pages (Easiest)

1. Create a GitHub account if you don't already have one
2. Create a new repository on GitHub
3. Upload all the files provided in this project to your repository
4. Enable GitHub Pages in your repository settings:
   - Go to Settings > Pages
   - Select "main" branch as the source
   - Click Save
5. Your app will be available at: https://[your-username].github.io/[repository-name]/
6. Visit this URL on your mobile device
7. Install to home screen (instructions below)

## Option 2: Local Development and Deployment

### Prerequisites
- Node.js and npm installed on your computer

### Setup Instructions

1. Create a new folder for your project
2. Save all the provided files to their respective locations:
   - `FacultyTracker.jsx` in `src/` folder
   - `index.js` in `src/` folder
   - `index.html` in `public/` folder
   - `manifest.json` in `public/` folder
   - `webpack.config.js` in the root folder
   - `package.json` in the root folder
   - `service-worker.js` in `public/` folder

3. Create app icons:
   - Create two PNG images with MIT's cardinal red background:
     - icon-192x192.png (192×192 pixels)
     - icon-512x512.png (512×512 pixels)
   - Place them in the `public/` folder

4. Open your terminal/command prompt and navigate to your project folder
5. Run the following commands:
   ```
   npm install
   npm run build
   ```

6. The built app will be in the `build/` folder
7. You can deploy this to any static website hosting service like:
   - GitHub Pages
   - Netlify
   - Vercel
   - Firebase Hosting

## Installing to Home Screen

### On Android:
1. Open Chrome and navigate to your app's URL
2. Tap the three dots menu in the top right
3. Select "Add to Home screen"
4. Follow the prompts to add the app

### On iOS:
1. Open Safari and navigate to your app's URL
2. Tap the Share button (square with up arrow)
3. Scroll down and select "Add to Home Screen"
4. Name your app and tap "Add"

Now you'll have an icon on your home screen that opens the Faculty Tracker app in full-screen mode without the browser interface!

## Important Files

- **FacultyTracker.jsx**: The main React component
- **index.js**: Entry point for the React application
- **index.html**: HTML template
- **manifest.json**: Defines how the app appears when installed
- **service-worker.js**: Enables offline functionality
- **webpack.config.js**: Builds the application
- **package.json**: Defines dependencies and scripts

## Features

- Track faculty members you're interested in working with
- MIT color scheme with cardinal red and gray
- Filter and sort functionality
- Works offline once installed
- Saves your data locally
- Mobile-friendly design