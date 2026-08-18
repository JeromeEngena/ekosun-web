# Ekosun Logistics Company-SMC Ltd Website

A complete, responsive website for a logistics company built with HTML and CSS.

## 📁 File Structure

``` html
car-hire-website/
│
├── index.html          # Homepage
├── about.html          # About/Company profile page
├── services.html       # Services and vehicle fleet page
├── contact.html        # Contact page with form and map
├── styles.css          # All CSS styles
└── README.md          # This file
```

## 🚀 Quick Start

1. **Download all files** and place them in the same folder
2. **Open `index.html`** in your web browser
3. The website is ready to use!

## 🎨 Customization Guide

### 1. Changing Company Name and Information

**In ALL HTML files (index.html, about.html, services.html, contact.html):**

```html
<!-- Find and replace these: -->
<h1>Ekosun Logistics Company-SMC Ltd</h1>              <!-- Replace with your company name -->
<p class="tagline">Logistics Services</p>  <!-- Replace with your tagline -->

<!-- In the footer, update: -->
<p>📞 +256 700 123 456</p>       <!-- Your phone number -->
<p>📧 info@ekosun.com</p>     <!-- Your email -->
<p>📍 123 Main Street, Kampala</p>  <!-- Your address -->
```

### 2. Changing Colors

**In `styles.css`**, modify these main color variables:

```css
/* Primary Blue: #3498db */
/* Dark Blue/Gray: #2c3e50 */
/* Red/Accent: #e74c3c */
/* Light Gray: #ecf0f1 */
```

**To change the entire color scheme:**

- Search for `#3498db` and replace with your primary color
- Search for `#e74c3c` and replace with your accent color
- Search for `#2c3e50` and replace with your dark color

### 3. Updating Vehicle Fleet

**In `services.html`**, find the vehicle cards section and modify:

```html
<div class="vehicle-card">
    <div class="vehicle-category">Economy</div>  <!-- Category name -->
    <h3>Compact & Sedan</h3>                      <!-- Vehicle type -->
    <p class="vehicle-description">Perfect for city driving</p>  <!-- Description -->
    <div class="vehicle-features">
        <span>🚗 5 Seats</span>    <!-- Capacity -->
        <span>🎒 2 Bags</span>     <!-- Luggage -->
        <span>⚙️ Manual/Auto</span> <!-- Transmission -->
    </div>
    <p class="price">From $30/day</p>  <!-- Price -->
    <p class="vehicle-examples"><em>Examples: Toyota Corolla</em></p>  <!-- Models -->
</div>
```

### 4. Changing Service Prices

**In `services.html`**, update pricing in the service cards:

```html
<ul>
    <li>Starting from $30/day</li>  <!-- Change price here -->
    <li>Unlimited mileage options</li>
    <li>Same-day availability</li>
</ul>
```

### 5. Setting Up the Contact Form

The contact form currently shows an alert. To make it functional:

### Option A: Using a Form Service (Easiest)

1. Sign up for [Formspree](https://formspree.io/) (free)
2. Get your form endpoint
3. In `contact.html`, update the form:

```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <!-- Remove the onsubmit handler -->
    <!-- Remove the JavaScript at the bottom -->
</form>
```

### Option B: Using Your Own Backend

1. Create a backend endpoint (PHP, Node.js, Python, etc.)
2. Update the form action attribute
3. Handle the POST request on your server

### 6. Adding Google Maps

**In `contact.html`:**

1. Get a Google Maps API key from [Google Cloud Console](https://console.cloud.google.com/)
2. Find your location coordinates:
   - Go to Google Maps
   - Right-click your location → "What's here?"
   - Copy the coordinates
3. Uncomment the script at the bottom of `contact.html`
4. Replace `YOUR_API_KEY` with your actual API key
5. Update coordinates in the `initMap()` function:

```javascript
const location = { lat: YOUR_LATITUDE, lng: YOUR_LONGITUDE };
```

### 7. Updating Social Media Links

**In ALL HTML files**, find the footer section:

```html
<a href="https://facebook.com/yourpage" target="_blank">Facebook</a>
<a href="https://twitter.com/yourhandle" target="_blank">Twitter</a>
<a href="https://instagram.com/yourhandle" target="_blank">Instagram</a>
<a href="https://linkedin.com/company/yourcompany" target="_blank">LinkedIn</a>
```

### 8. Changing Business Hours

**In `contact.html`**, update the hours:

```html
<p>Monday - Friday: 8:00 AM - 6:00 PM<br>
   Saturday: 9:00 AM - 4:00 PM<br>
   Sunday: Closed</p>
```

### 9. Modifying the About Page

**In `about.html`:**

- Update "Our Story" section with your company history
- Modify "Mission" and "Vision" statements
- Change "Core Values" to match your values
- Update the benefits list

### 10. Adding Your Logo

To add a logo image instead of text:

1. Save your logo as `logo.png` in the same folder
2. In ALL HTML files, replace the logo section:

```html
<!-- Replace this: -->
<div class="logo">
    <h1>Ekosun Logistics Company-SMC Ltd</h1>
    <p class="tagline">Logistics Services</p>
</div>

<!-- With this: -->
<div class="logo">
    <img src="logo.png" alt="Your Company Name" style="height: 50px;">
</div>
```

## 📱 Responsive Design

The website is fully responsive and works on:

- Desktop computers
- Tablets
- Mobile phones

No additional work needed - it automatically adapts!

## 🌐 Publishing Your Website

### Option 1: Free Hosting (Netlify)

1. Go to [Netlify](https://www.netlify.com/)
2. Sign up for free
3. Drag and drop your folder
4. Your site is live!

### Option 2: Traditional Web Hosting

1. Purchase hosting from providers like Bluehost, HostGator, etc.
2. Upload files via FTP
3. Point your domain to the hosting

### Option 3: GitHub Pages (Free)

1. Create a GitHub account
2. Create a new repository
3. Upload your files
4. Enable GitHub Pages in settings

## 🎯 Features Included

✅ Responsive design (mobile-friendly)  
✅ Multiple pages (Home, About, Services, Contact)  
✅ Contact form  
✅ Google Maps integration ready  
✅ Social media links  
✅ Professional styling  
✅ Easy to customize  
✅ SEO-friendly structure  
✅ Fast loading  

## 🔧 Browser Support

Works on all modern browsers:

- Chrome
- Firefox
- Safari
- Edge
- Opera

## 📝 Adding New Pages

To add a new page (e.g., "Gallery"):

1. Copy `about.html` and rename to `gallery.html`
2. Update the title and content
3. Add the link to the navigation in ALL HTML files:

```html
<ul class="nav-links">
    <li><a href="index.html">Home</a></li>
    <li><a href="about.html">About</a></li>
    <li><a href="services.html">Services</a></li>
    <li><a href="gallery.html">Gallery</a></li>  <!-- New page -->
    <li><a href="contact.html">Contact</a></li>
</ul>
```

## 💡 Tips for Success

1. **Use High-Quality Images**: Add actual car photos to make the site more appealing
2. **Update Content Regularly**: Keep prices and vehicle availability current
3. **Test on Mobile**: Always check how it looks on phones
4. **Get Customer Reviews**: Add a testimonials section
5. **Add a Booking System**: Integrate with booking software
6. **SEO**: Add meta descriptions and keywords
7. **Analytics**: Add Google Analytics to track visitors

## 🆘 Troubleshooting

### Problem: Styles not loading

- Make sure `styles.css` is in the same folder as HTML files
- Check the file name is exactly `styles.css` (case-sensitive on some servers)

### Problem: Links not working

- Ensure all HTML files are in the same folder
- Check file names match exactly

### Problem: Contact form not sending

- The form needs backend integration or a service like Formspree
- See "Setting Up the Contact Form" section above

## 📧 Support

For questions about customizing this website:

- Check this README carefully
- Search online for HTML/CSS tutorials
- Use browser developer tools (F12) to inspect elements

## 📄 License

This template is free to use for commercial and personal projects.

---
