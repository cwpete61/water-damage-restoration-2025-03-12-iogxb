# Water Damage Landing Page - Maintenance Guide

This guide will help you maintain and customize the Water Damage Restoration landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu:

```html
<div class="text-2xl font-bold text-blue-600">WaterRestore</div>
```

To change the company name:
1. Locate this div in the header section
2. Replace "WaterRestore" with your company name
3. Adjust text size using these Tailwind classes if needed:
   - `text-xl` (smaller)
   - `text-2xl` (current size)
   - `text-3xl` (larger)

### Hero Section
The main headline and subheading are in the first section after the header:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">
    Water Damage Restoration
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-8">
    Emergency Water Removal Service
</p>
```

To modify:
1. Replace the text between the `<h1>` tags for the main headline
2. Update the text between the `<p>` tags for the subheading
3. The responsive text sizes are:
   - Mobile: `text-4xl`
   - Tablet: `md:text-5xl`
   - Desktop: `lg:text-6xl`

### Service Cards
Located in the services section, each card follows this structure:

```html
<div class="bg-white p-8 rounded-2xl shadow-lg hover:shadow-xl transition-shadow duration-300">
    <div class="text-blue-600 mb-4">
        <!-- SVG icon here -->
    </div>
    <h3 class="text-xl font-bold mb-4">Fast Response</h3>
    <p class="text-gray-600">24/7 emergency response team...</p>
</div>
```

To add or modify service cards:
1. Copy the entire `<div>` block
2. Paste it within the `grid grid-cols-1 md:grid-cols-3 gap-8` container
3. Update the heading and description text
4. Maintain the class structure for consistent styling

## Managing Links

### Navigation Menu Links
The navigation menu contains internal page links:

```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. The `href="#section-name"` corresponds to section IDs in the HTML
2. Ensure section IDs match exactly (case-sensitive)
3. For external links, replace `#section-name` with the full URL

### Contact Information
Update contact links in the contact section:

```html
<a href="mailto:water@restoration.com" class="bg-white text-blue-600 px-8 py-4 rounded-full">
    Email Us
</a>
<a href="tel:+1234567890" class="bg-transparent border-2 border-white text-white px-8 py-4 rounded-full">
    Call Now
</a>
```

To modify:
1. Replace `water@restoration.com` with your email address
2. Update the phone number in both the `href="tel:+1234567890"` and display text

## Adding Privacy and Terms Pages

### Footer Legal Links
The footer contains placeholder links for legal pages:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your website directory
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Internal Links**
   - Verify that section IDs match navigation href attributes exactly
   - Check for extra spaces or special characters
   - Ensure IDs are unique across the page

2. **Responsive Design Problems**
   - Check that you're maintaining the responsive class patterns:
     - Mobile (default): `text-base`
     - Tablet: `md:text-lg`
     - Desktop: `lg:text-xl`

3. **Styling Inconsistencies**
   - Keep the existing color scheme using Tailwind classes:
     - Primary Blue: `text-blue-600`
     - Gray Text: `text-gray-600`
     - White Background: `bg-white`

### Need Help?
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Double-check HTML syntax and closing tags
- Ensure all changes maintain mobile responsiveness
- Test all links after making changes

Remember to always backup your files before making significant changes, and test your website across different devices and browsers after updates.