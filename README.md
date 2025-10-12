# Live Music Event Website

A professional GitHub Pages website for hosting a live music event, featuring a landing page with lineup information and a tickets page with Google Forms and Stripe payment integration.

## 🎵 Features

- **Landing Page** (`index.html`)
  - Eye-catching hero section with event branding
  - Lineup section (ready to be updated with artist information)
  - Event information cards (venue, date, tickets)
  - Responsive design that works on all devices

- **Tickets Page** (`tickets.html`)
  - Google Forms integration for collecting attendee information
  - Stripe payment integration for secure ticket purchases
  - Clear instructions for adding your own forms and payment links
  - Information section about ticket types and security

## 🚀 Quick Start

This website is ready to be deployed on GitHub Pages!

1. The site will be automatically available at: `https://connor-callaghan.github.io`
2. Make sure GitHub Pages is enabled in your repository settings (Settings → Pages → Source: main branch)

## 📝 Customization Guide

### Adding Your Google Form

1. Go to [forms.google.com](https://forms.google.com) and create your form
2. Click the "Send" button in your form
3. Click the embed icon (`<>`)
4. Copy the iframe code
5. Open `tickets.html` and find the Google Forms section (around line 51)
6. Replace the placeholder with your iframe code:

```html
<iframe 
    src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true" 
    width="100%" 
    height="500" 
    frameborder="0" 
    marginheight="0" 
    marginwidth="0">
    Loading…
</iframe>
```

### Adding Your Stripe Payment Link

1. Log in to [Stripe Dashboard](https://dashboard.stripe.com)
2. Go to Products → Add Product
3. Create your product and generate a Payment Link
4. Copy the payment link URL
5. Open `tickets.html` and find the Stripe section (around line 82)
6. Replace the placeholder with your iframe code:

```html
<iframe 
    src="https://buy.stripe.com/test_XXXXXXXX" 
    width="100%" 
    height="400" 
    frameborder="0">
    Loading…
</iframe>
```

Note: Use `test_` prefix for test mode or replace with your actual live payment link.

### Updating the Lineup

To add artists to the lineup, edit `index.html`:

1. Find the lineup section (around line 38)
2. Replace the placeholder artist cards with real information:

```html
<div class="artist-card">
    <div class="artist-name">Artist Name</div>
    <div class="artist-time">8:00 PM - 9:00 PM</div>
</div>
```

3. Remove the `placeholder` class to show the full gradient background

### Customizing Event Details

Edit these sections in `index.html`:

- **Event Title**: Change "Live Music Event" in the navigation and hero
- **Event Date**: Update "Coming Soon" in the hero section
- **Venue**: Update "Location TBA" in the venue info card
- **Date**: Update "Date TBA" in the date info card

## 🎨 Styling

The website uses a purple gradient color scheme (`#667eea` to `#764ba2`). To customize:

1. Open `styles.css`
2. Find the gradient definitions (e.g., `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`)
3. Replace with your preferred colors

## 📱 Responsive Design

The website is fully responsive and optimized for:
- Desktop computers
- Tablets
- Mobile phones

## 🌐 File Structure

```
├── index.html      # Landing page with hero and lineup
├── tickets.html    # Tickets page with forms and payment
├── styles.css      # All styling for the website
└── README.md       # This file
```

## 📸 Screenshots

### Landing Page
![Landing Page](https://github.com/user-attachments/assets/2de4a228-c897-462b-90df-ccf1a70df326)

### Tickets Page
![Tickets Page](https://github.com/user-attachments/assets/85e527da-76b7-40ea-a269-fd6d01fb15ba)

## 🔧 Local Development

To test the website locally:

```bash
# Start a simple HTTP server
python3 -m http.server 8000

# Visit http://localhost:8000 in your browser
```

## 📄 License

This project is open source and available for personal and commercial use.