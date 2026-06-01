# Quick Customization Checklist

Use this checklist to quickly customize the portfolio with your information.

## 📋 Step-by-Step Customization

### Step 1: Update Your Name & Contact Info
- [ ] **Find & Replace** in all HTML files:
  - Replace `Your Name` with your actual name
  - Replace `your.email@example.com` with your email
  - Replace `+1234567890` with your phone number
  - Replace `City, State, Country` with your location

**Quick way**: Use VS Code Find & Replace (Ctrl+H)

### Step 2: Add Your Images
- [ ] Create `assets/images/` folder (already done)
- [ ] Add `profile.jpg` (300x300px) - Your profile photo
- [ ] Add `about-photo.jpg` (500x400px) - About page photo
- [ ] Add `project-1.jpg` through `project-6.jpg` (600x400px each)
  
📸 **See IMAGE_GUIDE.md for detailed image specifications**

### Step 3: Update Project Information

Open `projects.html` and update each project card:

**For each project, change:**
```html
<!-- 1. Image -->
<img src="assets/images/project-X.jpg" alt="Your Project Name">

<!-- 2. Title -->
<h3>Your Project Title</h3>

<!-- 3. Category (choose: web, mobile, or design) -->
<p class="project-category">Web Development</p>

<!-- 4. Description -->
<p class="project-description">
    Brief description of what your project does...
</p>

<!-- 5. Technology Tags -->
<div class="tech-tags">
    <span class="tag">Technology1</span>
    <span class="tag">Technology2</span>
    <span class="tag">Technology3</span>
</div>

<!-- 6. Links -->
<a href="YOUR_LIVE_SITE_URL" target="_blank">Live Site</a>
<a href="YOUR_GITHUB_REPO_URL" target="_blank">Code</a>
```

### Step 4: Update About Page

Open `about.html` and update:

**Main About Section:**
- [ ] Update your bio paragraph (starting with "I'm a passionate...")
- [ ] Add your story/journey
- [ ] Update hobbies/interests section
- [ ] Add any other personal details

**Experience Section (Timeline):**
- [ ] Add 3-5 past positions
- [ ] Include dates, company names, and job titles
- [ ] Write brief descriptions of roles

**Education Section:**
- [ ] Add your degree/certification name
- [ ] Add school/organization name
- [ ] Add graduation year
- [ ] Add relevant achievements

### Step 5: Update Homepage Content

Open `index.html` and update:

**Hero Section:**
- [ ] "Hi, I'm Your Name" → Your name
- [ ] "Full Stack Developer | Designer | Problem Solver" → Your roles
- [ ] "I create beautiful, functional web experiences" → Your tagline

**Featured Projects:**
- [ ] Update the 3 featured projects (same as projects.html)
- [ ] Choose which projects to feature

**Skills Section:**
- [ ] Update Frontend skills list
- [ ] Update Backend skills list
- [ ] Update Tools list

### Step 6: Update Contact Page

Open `contact.html` and update:

**Contact Information:**
- [ ] Email (make it clickable with mailto:)
- [ ] Phone (make it clickable with tel:)
- [ ] Location
- [ ] Social media links
  - [ ] GitHub URL
  - [ ] LinkedIn URL
  - [ ] Twitter URL
  - [ ] Instagram URL

**Form Behavior:**
- [ ] Currently validates and shows success message
- [ ] For actual email delivery, see backend setup in README.md

### Step 7: Update Social Media Links

In all HTML files, update footer social links:
```html
<div class="social-links">
    <a href="https://github.com/yourusername" target="_blank">GitHub</a>
    <a href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
    <a href="https://twitter.com/yourhandle" target="_blank">Twitter</a>
    <a href="contact.html">Email</a>
</div>
```

### Step 8: Customize Theme Colors (Optional)

Open `style.css` and modify the color variables:

```css
:root {
    --primary-color: #667eea;      /* Change main brand color */
    --secondary-color: #764ba2;    /* Change secondary color */
    --accent-color: #f093fb;       /* Change accent color */
}
```

### Step 9: Update Meta Information

For SEO, update meta tags in each HTML file:

```html
<!-- In <head> section -->
<meta name="description" content="Your professional portfolio description here">
<title>Your Name - Portfolio | Your Title</title>
```

### Step 10: Test Everything

- [ ] **Test Navigation**
  - Click all menu links
  - Verify active link highlighting
  - Test on mobile view

- [ ] **Test Links**
  - All project links work
  - Social media links open correctly
  - Contact email link works (mailto:)

- [ ] **Test Responsiveness**
  - Open on mobile device
  - Test on tablet
  - Check desktop view
  - Use browser DevTools (F12)

- [ ] **Test Contact Form**
  - Fill form completely
  - Try submitting empty fields
  - Try invalid email
  - Verify success message appears

- [ ] **Test Images**
  - All images load correctly
  - No broken image icons
  - Images are properly sized

## 📝 Find & Replace Quick Reference

### Using VS Code (Ctrl+H)

**Replace all instances:**
1. Open Find & Replace (Ctrl+H)
2. Enter search term
3. Enter replacement term
4. Click "Replace All" button

**Common replacements:**
| Find | Replace With |
|------|---------------|
| Your Name | Your Actual Name |
| your.email@example.com | your@email.com |
| +1234567890 | Your Phone Number |
| City, State, Country | Your City |
| https://github.com | https://github.com/yourusername |
| https://linkedin.com | https://linkedin.com/in/yourprofile |

## 🎯 Priority Customization (Most Important)

**Minimum to get started:**
1. ✅ Update your name in all files
2. ✅ Update your email and phone
3. ✅ Add your profile photo
4. ✅ Add 3-6 project details
5. ✅ Update about section
6. ✅ Update social links

**This gives you a working portfolio in ~30 minutes!**

## 🎨 Optional Customizations (Nice to Have)

- [ ] Change color scheme to match your brand
- [ ] Add more projects (up to 6-12)
- [ ] Add more timeline items in experience
- [ ] Add certifications to education
- [ ] Setup contact form backend (see README.md)
- [ ] Add custom domain
- [ ] Setup analytics

## 🚀 Deployment Checklist

Before publishing:
- [ ] All personal info is correct
- [ ] All images are uploaded and showing
- [ ] All links work (internal and external)
- [ ] No placeholder text remains
- [ ] Forms work (or backend configured)
- [ ] Mobile view looks good
- [ ] No console errors (F12)
- [ ] Page loads quickly
- [ ] All typos fixed

## 📱 Testing on Different Devices

### Desktop Testing
- [ ] Chrome (latest)
- [ ] Firefox (latest)
- [ ] Safari (if Mac user)
- [ ] Edge (Windows)

### Mobile Testing
- [ ] iPhone (Safari)
- [ ] Android (Chrome)
- [ ] Use Chrome DevTools (F12 → Toggle Device Toolbar)

### Tablet Testing
- [ ] iPad or similar
- [ ] Test landscape and portrait modes

## 🔍 Quality Checklist

**Content Quality:**
- [ ] No typos or grammatical errors
- [ ] Professional tone throughout
- [ ] Clear descriptions of work
- [ ] Consistent formatting

**Design Quality:**
- [ ] Images are professional and high-quality
- [ ] Layout is clean and organized
- [ ] Color scheme is cohesive
- [ ] Typography is readable

**Functionality:**
- [ ] All links work
- [ ] Forms validate and submit
- [ ] Navigation is intuitive
- [ ] Page loads quickly

**Accessibility:**
- [ ] All images have alt text
- [ ] Buttons are keyboard accessible
- [ ] Color contrast is sufficient
- [ ] Mobile view is usable

## 🎯 Time Estimates

| Task | Time |
|------|------|
| Update names/contact | 10 minutes |
| Add images | 10-15 minutes |
| Update projects | 15-20 minutes |
| Update about & experience | 10-15 minutes |
| Update skills | 5 minutes |
| Test everything | 10 minutes |
| **Total** | **60-75 minutes** |

## 🚨 Common Mistakes to Avoid

- ❌ Leaving placeholder text like "Your Name"
- ❌ Using poor quality images
- ❌ Broken links
- ❌ Not testing on mobile
- ❌ Typos in contact information
- ❌ Images too large (> 200KB each)
- ❌ Inconsistent spacing/alignment
- ❌ Too many projects (stick to 6-8)
- ❌ Outdated information
- ❌ Dead social media links

## 💡 Tips for Best Results

1. **Keep it simple** - Clean design > complex design
2. **Be authentic** - Show real projects and real skills
3. **Keep content updated** - Update regularly with new work
4. **Use high-quality images** - Professional images matter
5. **Test thoroughly** - Check everything before sharing
6. **Ask for feedback** - Get opinions from others
7. **Optimize for mobile** - Most people browse on phones
8. **Make contact easy** - Clear contact info and working forms

## 📞 Need Help?

Refer to these files:
- **README.md** - Detailed documentation and features
- **IMAGE_GUIDE.md** - Image specifications and optimization
- **HTML files** - Comment sections with placeholders
- **style.css** - CSS variables for customization
- **script.js** - JavaScript functionality

---

**You've got this! Your portfolio will be amazing! 🎉**

*Questions? Review the documentation or check the code comments.*
