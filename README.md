# Landing Page Maintenance Guide
A comprehensive guide for maintaining and customizing the Best Websites TX landing page.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
```html
<!-- Original header text -->
<div class="text-2xl font-bold text-blue-600">
    Best Websites TX
</div>
```
To update the company name:
1. Locate the header section at the top of the HTML file
2. Change "Best Websites TX" to your desired text
3. Adjust text size using Tailwind classes:
   - `text-xl` (smaller)
   - `text-2xl` (current size)
   - `text-3xl` (larger)

### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Best Websites In Texas
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Custom Websites For Your Business
</p>
```
To modify hero content:
1. Update the h1 text for your main headline
2. Modify the paragraph text for your subheading
3. Key classes explained:
   - `md:text-5xl`: Changes text size on medium screens
   - `lg:text-6xl`: Changes text size on large screens
   - `mb-8`: Adds margin bottom spacing (8 units)

### Features and Benefits Cards
Each card follows this structure:
```html
<div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300">
    <div class="text-blue-600 mb-4">
        <i class="fas fa-laptop-code text-4xl"></i>
    </div>
    <h3 class="text-xl font-bold mb-4">Easy to Use</h3>
    <p class="text-gray-600">Your description here</p>
</div>
```
To customize cards:
1. Locate the specific card in either Features or Benefits section
2. Update the icon class (e.g., `fa-laptop-code` to `fa-users`)
3. Modify the heading text
4. Update the description paragraph
5. Important classes:
   - `rounded-xl`: Rounds corners
   - `shadow-lg`: Adds shadow effect
   - `p-8`: Adds padding (8 units)

## Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Contact</a>
</div>
```
To update navigation links:
1. Identify the section ID you want to link to
2. Update the `href` attribute to match the section ID
3. Example: `<a href="#new-section">New Section</a>`

### Call-to-Action Links
```html
<a href="https://sigmaseo.io" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">
    Get Started Today
</a>
```
To update CTA links:
1. Replace `https://sigmaseo.io` with your desired URL
2. Update the button text as needed
3. Test the link to ensure it opens correctly

## Linking Privacy and Terms Pages

### Footer Legal Links
Current structure:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```
To add privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match exactly with href attributes
   - Check for typos in IDs and hrefs
   - Section IDs should not contain spaces

2. **Responsive Design Issues**
   - Check media query classes (md:, lg:)
   - Verify container class is present
   - Test on different screen sizes

3. **Icon Not Displaying**
   - Confirm Font Awesome CDN is loaded
   - Check icon class names against Font Awesome documentation
   - Ensure proper icon style prefix (fas, far, fab)

4. **Styling Problems**
   - Verify Tailwind CDN is loaded
   - Check for conflicting classes
   - Ensure classes are spelled correctly

Remember to:
- Always make backups before making changes
- Test all links after updating
- View changes on multiple devices
- Validate HTML using W3C Validator

For additional help, consult the [Tailwind CSS documentation](https://tailwindcss.com/docs) or [Font Awesome documentation](https://fontawesome.com/docs).