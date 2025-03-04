# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. It's designed for beginners and provides step-by-step instructions for common modifications.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Policy Pages](#adding-policy-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your brand name and navigation menu. To update:

1. **Brand Name**
```html
<div class="text-2xl font-semibold tracking-tight">
    <span class="text-gray-900">Brand</span>  <!-- Replace "Brand" with your company name -->
</div>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <!-- Update text between <a> tags -->
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight text-gray-900 mb-8">
    Lorem ipsum dolor  <!-- Replace with your main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Lorem ipsum dolor  <!-- Replace with your subheading -->
</p>
```

### Understanding Tailwind Classes
Common classes used in this template:
- `text-[size]`: Controls text size (e.g., `text-xl`, `text-2xl`)
- `mb-[size]`: Adds bottom margin (e.g., `mb-8`, `mb-12`)
- `py-[size]`: Adds vertical padding (e.g., `py-4`, `py-24`)
- `bg-[color]`: Sets background color (e.g., `bg-white`, `bg-indigo-600`)

## Managing Links

### Navigation Menu Links
The page uses anchor links to scroll to sections:
```html
<a href="#features">Features</a>  <!-- Links to features section -->
<a href="#benefits">Benefits</a>  <!-- Links to benefits section -->
<a href="#contact">Contact</a>    <!-- Links to contact section -->
```

To update these:
1. Find the section ID you want to link to
2. Update the `href` attribute with `#` followed by the section ID
3. Update the link text between the `<a>` tags

### Footer Links
Current placeholder links in the footer:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">About</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Careers</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Contact</a></li>
</ul>
```

To update these:
1. Replace `#` with your actual URL
2. Example: `<a href="about.html">` or `<a href="https://yoursite.com/about">`

## Adding Policy Pages

### Adding Footer Policy Links
Add these links to your footer section:
```html
<div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
    <p>&copy; 2024 Company Name. All rights reserved.</p>
    <!-- Add policy links below copyright -->
    <div class="mt-4">
        <a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300 mr-4">Privacy Policy</a>
        <a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a>
    </div>
</div>
```

### Styling Policy Links
The added links use these Tailwind classes:
- `text-gray-400`: Light gray text color
- `hover:text-white`: White text on hover
- `transition-colors`: Smooth color transition
- `duration-300`: Transition timing
- `mr-4`: Right margin spacing

## Troubleshooting

### Common Issues

1. **Links Not Working**
   - Check that IDs match exactly (case-sensitive)
   - Ensure URLs are correctly spelled
   - Verify file paths for internal pages

2. **Responsive Design Issues**
   - Look for classes starting with `md:` or `lg:`
   - These control appearance at different screen sizes
   - Don't remove these classes unless you're sure

3. **Styling Problems**
   - Keep the `class` attribute intact
   - Add new classes at the end of existing ones
   - Maintain spacing between class names

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate your HTML at [W3C Validator](https://validator.w3.org/)
- Test responsiveness using browser developer tools

Remember to:
- Back up your files before making changes
- Test all links after updating
- View changes on different screen sizes
- Keep consistent styling across all pages