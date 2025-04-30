# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Whether you're new to web development or need a quick reference, follow these instructions to make updates while preserving the design integrity.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your site name and navigation menu. To update:

1. Change the site name:
```html
<!-- Find this line in the header -->
<a href="#" class="text-2xl font-bold text-purple-500">landing</a>
```
Replace "landing" with your site name while keeping the classes intact.

### Hero Section
The main welcome section includes a title, subtitle, and call-to-action button:

```html
<h1 class="text-4xl md:text-6xl font-bold mb-6 bg-gradient-to-r from-purple-400 to-pink-500 bg-clip-text text-transparent">landing</h1>
<p class="text-xl md:text-2xl mb-12 text-gray-300 max-w-3xl mx-auto">gogogo</p>
```

To modify:
1. Replace "landing" with your title
2. Replace "gogogo" with your subtitle
3. Keep the classes to maintain the gradient effect and responsive sizing

### Features and Benefits
Located in separate sections, each with cards:

```html
<div class="p-8 bg-gray-700 rounded-2xl">
    <h3 class="text-2xl font-semibold mb-4">Fast</h3>
    <p class="text-gray-300">Lightning-quick performance for seamless operation.</p>
</div>
```

To update:
1. Locate the section you want to modify (id="features" or id="benefits")
2. Change the h3 text for titles
3. Update the p text for descriptions
4. Maintain the existing classes for consistent styling

### Understanding Tailwind Classes
Common classes used in this template:
- `text-[size]`: Controls text size (e.g., text-xl, text-2xl)
- `bg-[color]`: Sets background color (e.g., bg-gray-900)
- `p-[size]`: Sets padding (e.g., p-8)
- `mb-[size]`: Sets bottom margin (e.g., mb-4)
- `rounded-[size]`: Controls border radius (e.g., rounded-2xl)

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex items-center space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#video">Watch</a>
    <a href="#faq">FAQ</a>
    <a href="https://awstrikeroz.github.io/lorem-ipsum-dolor-2025-04-30-4xocv/">Get Started</a>
</div>
```

To update:
1. Internal links (starting with #) connect to section IDs
2. Replace the "Get Started" URL with your actual URL
3. Maintain the class structure for consistent styling

### Call-to-Action Buttons
Located in hero and bottom sections:
```html
<a href="https://awstrikeroz.github.io/lorem-ipsum-dolor-2025-04-30-4xocv/" class="inline-block px-8 py-4 bg-purple-600 hover:bg-purple-700 rounded-full">
```

Update all instances of this placeholder URL to your actual destination.

## Adding Privacy and Terms Pages

### Footer Legal Links
Current placeholder links:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create privacy.html and terms.html files in your project directory
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match the href attributes
   - Check for typos in IDs and hrefs
   - IDs should be unique across the page

2. **Responsive Design Issues**
   - Don't remove `md:` prefixed classes - they control tablet/desktop layouts
   - Keep the viewport meta tag in the head section
   - Test on different screen sizes using browser dev tools

3. **Style Problems**
   - Don't remove Tailwind CSS link from head section
   - Maintain class order when copying/pasting
   - Check for missing closing tags

### Need Help?
- Verify changes in a browser's dev tools (F12)
- Test all links after updating
- Ensure all files are in the correct directory
- Keep backups before making major changes

Remember to test all changes across different devices and browsers to ensure consistency in appearance and functionality.