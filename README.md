# Landing Page Maintenance Guide
## For 101Headshots Corporate Photography Website

This guide provides detailed instructions for maintaining and customizing the 101Headshots landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
```html
<header class="fixed w-full bg-gray-900/95 backdrop-blur-sm z-50 border-b border-gray-800">
    <nav class="container mx-auto px-6 py-4">
        <div class="flex items-center justify-between">
            <a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">101Headshots</a>
```
To modify:
- Company name: Replace "101Headshots" with your business name
- Navigation text: Update "Services", "Benefits", and "Contact" as needed
- Header styling: Adjust background opacity by changing `bg-gray-900/95` (95% opacity)

### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6 bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">Platte City, Missouri Corporate Headshot Photography Services</h1>
```
To modify:
- Main heading: Replace the h1 text
- Responsive text sizes:
  - Mobile: `text-4xl`
  - Tablet: `md:text-5xl`
  - Desktop: `lg:text-6xl`

### Features Cards
```html
<div class="bg-gray-800 rounded-2xl p-8 hover:scale-105 transition-transform duration-300 shadow-xl">
    <h3 class="text-xl font-semibold mb-4 text-purple-400">Executive Image</h3>
    <p class="text-gray-300">Professional portraits that capture leadership presence and authority.</p>
</div>
```
To customize:
- Card background: Change `bg-gray-800`
- Hover effect: Modify `hover:scale-105`
- Text color: Update `text-purple-400` or `text-gray-300`

## Fixing Broken Links

### Current Link Structure
1. Navigation Menu Links:
```html
<a href="#services" class="text-gray-300 hover:text-white transition-colors duration-300">Services</a>
<a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
<a href="#contact" class="text-gray-300 hover:text-white transition-colors duration-300">Contact</a>
```

2. Call-to-Action Link:
```html
<a href="https://www.101headshots.com" class="inline-block px-8 py-4 bg-gradient-to-r from-purple-600 to-pink-600 rounded-full">Book Your Session</a>
```

To update links:
1. Internal links (starting with #): Ensure they match section IDs
2. External links: Replace with full URLs
3. Email links: Update mailto address in contact section

## Linking Privacy and Terms Pages

### Current Footer Links
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add privacy and terms pages:
1. Create new files:
   - `privacy.html`
   - `terms.html`

2. Update footer links:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. Broken Internal Links
```html
<!-- Wrong -->
<a href="services">Services</a>

<!-- Correct -->
<a href="#services">Services</a>
```

2. Missing Responsive Classes
```html
<!-- Wrong -->
<h1 class="text-4xl">Heading</h1>

<!-- Correct -->
<h1 class="text-4xl md:text-5xl lg:text-6xl">Heading</h1>
```

3. Gradient Text Not Showing
```html
<!-- Wrong -->
<h1 class="bg-gradient-to-r from-purple-500 to-pink-500">Text</h1>

<!-- Correct -->
<h1 class="bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">Text</h1>
```

### Testing Changes
1. Test all links after updating
2. View the page at different screen sizes
3. Check hover effects on all interactive elements
4. Verify email links open mail client correctly

Remember to:
- Keep backup copies of the original files
- Test changes in multiple browsers
- Maintain consistent styling across all pages
- Validate HTML using W3C Validator

For additional help, consult the [Tailwind CSS documentation](https://tailwindcss.com/docs) or reach out to your web development team.