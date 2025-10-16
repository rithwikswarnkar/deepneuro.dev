# Website Setup Guide

## Overview
This is your professional AI/ML portfolio website built with HTML, CSS, and JavaScript. It's designed to showcase your projects, skills, and experience to potential employers and collaborators.

## 🎯 What's Included

### Pages
1. **Home (index.html)** - Hero section with stats, featured projects, and skills overview
2. **About (about.html)** - Professional summary, education, expertise, and personal interests
3. **Projects (projects.html)** - Detailed project showcases with tech stacks and metrics
4. **Experience (experience.html)** - Timeline of work experience and achievements
5. **Skills (skills.html)** - Technical skills with visual proficiency indicators
6. **Contact (contact.html)** - Multiple contact methods and FAQs
7. **Blog (blog.html)** - Links to your writing on Medium and LinkedIn

### Features
- ✨ Modern, professional design with smooth animations
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎨 Dark theme with gradient accents
- 🚀 Fast loading and optimized performance
- ♿ Accessibility-friendly
- 📊 Visual skill bars and progress indicators
- 🔗 Integrated social media links
- 📄 Resume download functionality

## 🚀 Quick Start

### 1. Add Your Resume
```bash
# Place your resume PDF in the assets folder
cp /path/to/your/resume.pdf assets/resume.pdf
```

### 2. Update Content
Edit the HTML files to customize:
- Your name and contact information
- Project descriptions and GitHub links
- Work experience details
- Skills and proficiency levels
- Education information

### 3. Customize Colors (Optional)
Edit `style.css` to change the color scheme:
```css
:root {
  --primary-color: #667eea;    /* Main brand color */
  --secondary-color: #764ba2;  /* Secondary brand color */
  --accent-color: #f093fb;     /* Accent color */
}
```

### 4. Test Locally
Open `index.html` in your browser to preview:
```bash
# Option 1: Direct opening
open index.html

# Option 2: Using Python server
python3 -m http.server 8000
# Then visit: http://localhost:8000

# Option 3: Using Node.js
npx http-server
```

## 🌐 Deployment Options

### GitHub Pages (Recommended - Free)
1. Create a GitHub repository
2. Push your files to the repository
3. Go to Settings > Pages
4. Select the main branch as source
5. Your site will be live at: `https://yourusername.github.io/repo-name`

### Custom Domain with GitHub Pages
1. Add a `CNAME` file with your domain (already included: deepneuro.dev)
2. Configure DNS settings with your domain provider:
   ```
   Type: A Record
   Name: @
   Value: 185.199.108.153
   Value: 185.199.109.153
   Value: 185.199.110.153
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: yourusername.github.io
   ```

### Netlify (Easy deployment)
1. Sign up at netlify.com
2. Drag and drop your folder
3. Get instant deployment with HTTPS

### Vercel
1. Sign up at vercel.com
2. Import from GitHub
3. Auto-deployment on every push

## 📝 Customization Guide

### Updating Projects
In `projects.html`, find the project cards and update:
```html
<div class="project-card">
  <h3>Your Project Name</h3>
  <p>Your project description...</p>
  <div class="card-tech">
    <span>Technology 1</span>
    <span>Technology 2</span>
  </div>
  <a href="https://github.com/yourrepo">GitHub Link</a>
</div>
```

### Updating Skills
In `skills.html`, adjust skill bars:
```html
<div class="skill-bar-container">
  <div class="skill-header">
    <span class="skill-name">Skill Name</span>
    <span class="skill-level">Proficiency Level</span>
  </div>
  <div class="skill-bar">
    <div class="skill-progress" style="width: 90%;"></div>
  </div>
</div>
```

### Updating Experience
In `experience.html`, modify timeline items:
```html
<div class="timeline-item">
  <div class="timeline-content">
    <div class="timeline-date">2024 - Present</div>
    <h3 class="timeline-title">Job Title</h3>
    <div class="timeline-subtitle">Company | Location</div>
    <div class="timeline-description">
      <p>Description...</p>
      <ul>
        <li>Achievement 1</li>
        <li>Achievement 2</li>
      </ul>
    </div>
  </div>
</div>
```

### Updating Contact Information
Replace placeholder contact info in:
- `index.html` (Hero section social links)
- `contact.html` (All contact cards)
- `footer` (In all HTML files)

## 🎨 Design Philosophy

This website is designed to be:
- **Professional:** Clean, modern design that appeals to recruiters
- **Informative:** Detailed project descriptions with metrics and tech stacks
- **Engaging:** Smooth animations and interactive elements
- **Accessible:** Semantic HTML and keyboard navigation support
- **Fast:** Optimized CSS and minimal dependencies

## 📊 SEO Optimization

Each page includes:
- Meta descriptions
- Semantic HTML5 tags
- Descriptive titles
- Alt text for images (when you add them)

To improve SEO:
1. Add more detailed meta descriptions
2. Include structured data (JSON-LD)
3. Optimize images (compress and add alt text)
4. Create a sitemap.xml
5. Submit to Google Search Console

## 🔧 Advanced Customization

### Adding Google Analytics
Add this to the `<head>` of each HTML file:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

### Adding Project Images
1. Create an `assets/images/` directory
2. Add project screenshots
3. Update project cards:
```html
<div class="card-image">
  <img src="assets/images/project-name.png" alt="Project screenshot">
</div>
```

### Adding a Blog Section (Embedded)
Instead of just linking to Medium, you can embed Medium articles:
```html
<script src="https://medium-widget.pixelpoint.io/widget.js"></script>
<div class="medium-widget" data-username="swarnkar.rithwik"></div>
```

## 📱 Browser Support

This website works on:
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🐛 Troubleshooting

### Resume Download Not Working
- Ensure `resume.pdf` exists in the `assets/` folder
- Check file permissions
- Verify the path in HTML: `href="assets/resume.pdf"`

### Animations Not Working
- Check if JavaScript is enabled
- Open browser console for errors
- Ensure CSS animations are supported

### Mobile Menu Not Opening
- Check JavaScript console for errors
- Verify the menu toggle script is present
- Test in different browsers

## 📈 Next Steps

After setup:
1. ✅ Add your resume PDF
2. ✅ Update all personal information
3. ✅ Customize project descriptions
4. ✅ Add actual work experience
5. ✅ Update GitHub repository links
6. ✅ Test on mobile devices
7. ✅ Deploy to GitHub Pages or Netlify
8. ✅ Share your website link on LinkedIn
9. ✅ Add to your email signature
10. ✅ Include in job applications

## 📞 Support

If you need help customizing or have questions:
- Check the code comments in HTML/CSS files
- Refer to MDN Web Docs for HTML/CSS questions
- Open an issue on GitHub

## 🎓 Learning Resources

Want to customize further? Check out:
- [MDN Web Docs](https://developer.mozilla.org/) - HTML, CSS, JavaScript reference
- [CSS Tricks](https://css-tricks.com/) - CSS tutorials and examples
- [Can I Use](https://caniuse.com/) - Browser compatibility checker

---

**Good luck with your job search! 🚀**

Remember to keep your website updated as you complete new projects and gain new skills. A regularly updated portfolio shows continuous learning and professional growth.


