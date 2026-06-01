# Image Guidelines & Placement Guide

This guide explains what images you need and where to place them.

## 📸 Required Images

### 1. Profile Photo
- **File**: `assets/images/profile.jpg`
- **Size**: 300x300 pixels
- **Format**: JPG, PNG, or WebP
- **Purpose**: Displayed on homepage hero section
- **Recommendation**: Professional headshot or portrait
- **Aspect Ratio**: 1:1 (Square)

### 2. About Page Photo
- **File**: `assets/images/about-photo.jpg`
- **Size**: 500x400 pixels (or similar ratio)
- **Format**: JPG, PNG, or WebP
- **Purpose**: About page main image
- **Recommendation**: Professional photo or candid portrait
- **Aspect Ratio**: 5:4 or 16:10

### 3. Project Thumbnail Images
- **Files**: 
  - `assets/images/project-1.jpg`
  - `assets/images/project-2.jpg`
  - `assets/images/project-3.jpg`
  - `assets/images/project-4.jpg`
  - `assets/images/project-5.jpg`
  - `assets/images/project-6.jpg`
- **Size**: Minimum 300px width, 200px height
- **Format**: JPG, PNG, or WebP
- **Purpose**: Project showcases on homepage and projects page
- **Recommendation**: Screenshot of project, mockup, or preview image
- **Aspect Ratio**: 3:2 or 16:10

## 📂 File Structure

```
assets/
└── images/
    ├── profile.jpg           (300x300px)
    ├── about-photo.jpg       (500x400px)
    ├── project-1.jpg         (300x200px min)
    ├── project-2.jpg
    ├── project-3.jpg
    ├── project-4.jpg
    ├── project-5.jpg
    └── project-6.jpg
```

## 🎨 Image Optimization Tips

### Best Practices
1. **Format Selection**
   - Use JPG for photographs
   - Use PNG for graphics/logos with transparency
   - Use WebP for best compression (convert JPG/PNG)

2. **Compression**
   - Target: 100-150 KB per image maximum
   - Use tools like:
     - TinyPNG (https://tinypng.com/)
     - ImageOptim (Mac)
     - FileOptimizer (Windows)

3. **Dimensions**
   - Don't upload oversized images
   - Follow the recommended sizes above
   - Use 2x resolution for Retina displays

4. **Quality**
   - Maintain good quality while compressing
   - Test on different screen sizes
   - Ensure images look sharp on mobile

## 🖼️ Example Project Image Setup

### Project Card Image (Recommended Setup)
```
Width: 600px
Height: 400px
Format: JPG or WebP
Max File Size: 150KB
Aspect Ratio: 3:2
```

### How Images Display

**On Desktop (≥1200px)**
- Projects grid: 3 columns
- Each image: ~340px wide × ~226px tall

**On Tablet (768px - 1199px)**
- Projects grid: 2 columns
- Each image: ~100% of column width

**On Mobile (≤767px)**
- Projects grid: 1-2 columns
- Each image: Full width or half width

## 🔧 Creating Images

### Tools to Create Project Thumbnails
- **Figma** (Free): https://www.figma.com/
- **Canva** (Free): https://www.canva.com/
- **Adobe Express** (Free): https://www.adobe.com/express/
- **Screenshot Tools**: Built-in on Windows/Mac
- **Browser DevTools**: Screenshot webpage features

### Tips for Project Images
1. **Show Your Work**: Display actual project results
2. **Consistency**: Use similar layouts and sizes
3. **Branding**: Include your logo or color scheme
4. **Mockups**: Use device mockups for apps
5. **Before/After**: Show problem and solution

## 📐 Image Sizing for Different Uses

### Profile Photo
```
Original: 600x600px (2x for Retina)
Optimized: 300x300px, 50-80KB
```

### Hero Section About Photo
```
Original: 1000x800px (2x for Retina)
Optimized: 500x400px, 60-100KB
```

### Project Thumbnails
```
Original: 1200x800px (2x for Retina)
Optimized: 600x400px, 80-120KB each
```

## 🎬 Batch Image Processing

### Using ImageMagick (Command Line)
```bash
# Resize all JPG files
convert *.jpg -resize 600x400 optimized_%d.jpg

# Convert PNG to WebP
convert image.png -quality 80 image.webp
```

### Using Python Script
```python
from PIL import Image
import os

# Resize all images in a folder
for filename in os.listdir('raw_images/'):
    if filename.endswith('.jpg'):
        img = Image.open(f'raw_images/{filename}')
        img.thumbnail((600, 400))
        img.save(f'assets/images/{filename}', quality=85)
```

## 🌐 Hosting Images

### Options
1. **Local** (Current Setup)
   - Store in `assets/images/`
   - Works offline
   - No additional setup needed

2. **CDN** (Recommended for Production)
   - Cloudinary (https://cloudinary.com/)
   - Imgix (https://www.imgix.com/)
   - AWS CloudFront
   - Faster loading globally

3. **Cloud Storage**
   - Google Cloud Storage
   - AWS S3
   - Azure Blob Storage

## 🔍 Checking Image URLs

In your HTML files, verify image paths:

```html
<!-- Correct paths (relative) -->
<img src="assets/images/profile.jpg" alt="Profile">

<!-- If in different location -->
<!-- From about.html to ../assets/images/ -->
<img src="../assets/images/profile.jpg" alt="Profile">
```

### Troubleshooting Missing Images
1. **Check file names** (case-sensitive on Mac/Linux)
2. **Verify paths** relative to HTML file location
3. **Check file extensions** (.jpg vs .JPG)
4. **Open browser console** (F12) for error messages
5. **Use browser DevTools** → Network tab to see failed requests

## 📱 Responsive Images

To improve mobile performance, consider adding multiple image sizes:

```html
<picture>
  <source srcset="assets/images/project-1-large.jpg" media="(min-width: 1200px)">
  <source srcset="assets/images/project-1-medium.jpg" media="(min-width: 768px)">
  <img src="assets/images/project-1-small.jpg" alt="Project 1">
</picture>
```

## 🚀 Quick Start with Placeholder Images

For testing the portfolio before adding real images:

1. Use free image services:
   - Unsplash (https://unsplash.com/)
   - Pexels (https://www.pexels.com/)
   - Pixabay (https://pixabay.com/)
   - Placeholder (https://via.placeholder.com/600x400)

2. Download sample images:
   ```html
   <!-- Quick placeholder from placeholder service -->
   <img src="https://via.placeholder.com/600x400?text=Your+Project" alt="Project">
   ```

3. Replace with real images later

## ✅ Image Checklist

Before deploying your portfolio:
- [ ] All 6-8 project images added
- [ ] Profile photo is professional
- [ ] All images optimized (< 150KB each)
- [ ] Image dimensions match recommendations
- [ ] File names are lowercase without spaces
- [ ] All image paths verified working
- [ ] Images look good on mobile devices
- [ ] No broken image links
- [ ] Alt text is descriptive

## 📊 Performance Metrics

Good website performance targets:
- **Page Load Time**: < 3 seconds
- **Image Load Time**: < 1 second
- **Total Image Size**: < 500KB per page
- **Lighthouse Score**: > 80/100

Check performance:
- Chrome DevTools → Lighthouse
- PageSpeed Insights (https://pagespeed.web.dev/)
- WebPageTest (https://www.webpagetest.org/)

---

**Ready to add your images? Follow the directory structure and size recommendations above!** 🎉
