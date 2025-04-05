# GitPage Landing Page Maintenance Guide

This guide will help you maintain and customize the GitPage landing page. It's designed for beginners with no prior coding experience.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text**: Find this line and replace "GitPage" with your brand name:
```html
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    GitPage
</a>
```

2. **Navigation Links**: Locate the navigation div and modify menu items:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
    <!-- Add or modify menu items here -->
</div>
```

### Hero Section
Update the main headline and subheading:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">
    Build Your Website Effortlessly with Expert GitPage Support
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Your Partner in Creating and Enhancing Websites
</p>
```

### Tailwind CSS Classes Explained
- `text-4xl`: Sets font size (increases with md: and lg: prefixes)
- `mb-8`: Adds margin bottom (8 units)
- `bg-gray-900`: Sets background color
- `hover:scale-105`: Enlarges element on hover
- `transition-colors`: Enables smooth color transitions

## Managing Links

### Current Link Structure
The page contains these link types:
1. Navigation menu links (internal)
2. Call-to-action buttons (external)
3. Footer links (mixed)

### Updating Internal Links
To modify section links:
1. Locate the section ID:
```html
<section id="features" class="py-24 bg-gray-900">
```

2. Update corresponding navigation link:
```html
<a href="#features" class="text-gray-300 hover:text-white">Features</a>
```

### Updating External Links
Replace the GitPage URL with your website:
```html
<!-- Before -->
<a href="https://gitpage.aibizbots4u.com" class="inline-block px-8 py-4...">

<!-- After -->
<a href="https://your-website.com" class="inline-block px-8 py-4...">
```

### Email Links
Update the mailto link with your email:
```html
<a href="mailto:your-email@domain.com" class="text-gray-400 hover:text-white">
```

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your project:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Locate these lines in the footer:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

Replace the `#` with proper paths:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Links**
- Check that all `href` attributes point to valid URLs
- Verify that section IDs match their corresponding links
- Ensure file names match exactly (case-sensitive)

2. **Styling Problems**
- Make sure Tailwind CSS is properly loaded
- Check for typos in class names
- Verify responsive classes (md:, lg:) are correctly formatted

3. **Layout Issues**
- Confirm container classes are present
- Check for proper closing tags
- Verify responsive design classes are correctly implemented

### Need Help?
If you encounter issues:
1. Check the browser console for errors
2. Verify all files are in the correct directory
3. Ensure all external resources (fonts, CSS) are loading
4. Double-check all opening and closing HTML tags

Remember to test all changes across different devices and screen sizes to ensure proper responsive behavior.

---

For additional support or questions, please contact the development team at the email provided in the footer section.