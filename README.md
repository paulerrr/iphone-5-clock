# iPhone 5 Clock PWA

A digital clock web application optimized as a Progressive Web App (PWA) for iPhone 5 running iOS 10.3.4.

![Clock App Screenshot](https://via.placeholder.com/320x568/000000/FFFFFF/?text=iPhone+5+Clock)

## Features

- **Full-screen clock** with date display
- **Offline support** using AppCache (compatible with iOS 10.3.4)
- **Home screen installation** using iOS-specific meta tags
- **Customizable settings**:
  - 24-hour or 12-hour format
  - Show/hide seconds
  - Night mode
  - Color themes
- **Screen-on functionality** that keeps the display active
- **Battery level indicator** (when available)
- **Responsive design** optimized for iPhone 5 screen (both portrait and landscape)
- **Offline indicator** when network connection is lost
- **Installation guide** for first-time users

## PWA Capabilities

This app implements all PWA features available to iOS 10.3.4:

- ✅ Home screen installation
- ✅ Full-screen mode (no browser UI)
- ✅ Custom splash screen
- ✅ Custom home screen icon
- ✅ Offline functionality via AppCache
- ✅ Persistent settings via localStorage
- ❌ Service Workers (not supported in iOS 10)
- ❌ Web App Manifest (not supported in iOS 10)
- ❌ Push notifications (not supported in iOS 10)

## How to Install (for iPhone 5 Users)

1. Open Safari and visit the deployed website
2. Tap the Share button (box with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Name the app (default: "Clock") and tap "Add"
5. Find and tap the app icon on your home screen to launch in full-screen mode

## Deployment

This project is configured for easy deployment on Vercel:

1. Fork or clone this repository
2. Connect your repository to Vercel
3. Deploy

The included `vercel.json` file handles all necessary configuration.

## Development

To run locally:

1. Clone the repository
2. Open `index.html` in a browser
   
For testing the PWA features, you'll need to:
1. Serve the files using a local web server (e.g., `npx serve`)
2. Access using HTTPS or localhost for some features

## Structure

- `index.html` - Main application
- `clock.appcache` - Offline cache manifest
- `offline.html` - Fallback page for when offline
- `icons/` - App icons for home screen
- `splash/` - Splash screen images
- `vercel.json` - Deployment configuration

## License

[MIT License](LICENSE)

## Acknowledgements

- Designed specifically for iPhone 5 running iOS 10.3.4
- Uses multiple approaches to prevent screen sleep
- Implements AppCache for offline support (deprecated but supported in iOS 10)
