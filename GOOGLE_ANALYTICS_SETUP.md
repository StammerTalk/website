# Google Analytics Setup Instructions

## Overview
This website now includes Google Analytics 4 (GA4) tracking to monitor visitor statistics and page performance.

## Setup Steps

### 1. Create a Google Analytics Account
1. Go to [Google Analytics](https://analytics.google.com/)
2. Sign in with your Google account
3. Click "Start measuring" to create a new account
4. Follow the setup wizard to create a property for your website

### 2. Get Your Measurement ID
1. In your Google Analytics account, go to Admin (gear icon)
2. Select your property
3. Click on "Data Streams" under the Property column
4. Click on your web stream
5. Copy the "Measurement ID" (it starts with "G-")

### 3. Update Your Website Configuration
1. Open `_config.yml` in your website root
2. Find the line: `google_analytics: "G-XXXXXXXXXX"`
3. Replace "G-XXXXXXXXXX" with your actual Measurement ID
4. Save the file

### 4. Deploy Your Changes
1. Commit and push your changes to GitHub
2. Your GitHub Pages site will automatically rebuild with Google Analytics

## Features Included

### Basic Tracking
- Page views for all pages
- Visitor sessions and user behavior
- Geographic data about visitors
- Device and browser information

### Enhanced Tracking
- Individual page performance metrics
- Outbound link clicks tracking
- File download tracking (PDF, DOC, XLS, ZIP, media files)
- Custom page categorization
- Enhanced ecommerce events

### Page-Level Analytics
Each page is tracked with:
- Page title and URL
- Page category (from post/page categories)
- Page type (layout used)
- Custom dimensions for detailed analysis

## Viewing Your Analytics

### Google Analytics Dashboard
1. Go to [Google Analytics](https://analytics.google.com/)
2. Select your property
3. Navigate to Reports > Engagement > Pages and screens to see individual page performance

### Key Reports to Monitor
- **Audience Overview**: General visitor statistics
- **Behavior > Site Content > All Pages**: Individual page performance
- **Behavior > Site Content > Landing Pages**: Entry points to your site
- **Acquisition > All Traffic > Source/Medium**: How visitors find your site
- **Real-time**: Live visitor activity

### Custom Reports
You can create custom reports to track:
- Most popular blog posts
- Page categories performance
- Download activity
- Outbound link clicks

## Privacy Considerations
- IP anonymization is enabled by default
- Cookie flags are set for compliance
- All tracking respects user privacy settings

## Troubleshooting

### Analytics Not Showing Data
- Allow 24-48 hours for data to appear
- Check that your Measurement ID is correct
- Verify the site is receiving traffic
- Check browser console for any JavaScript errors

### Testing the Setup
1. Visit your website
2. Check the browser's developer tools > Network tab
3. Look for requests to `googletagmanager.com`
4. Use Google Analytics Real-time reports to see live activity

## Support
For issues with Google Analytics setup, refer to the [Google Analytics Help Center](https://support.google.com/analytics/).
