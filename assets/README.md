# Assets Folder

This folder contains static assets for your personal website.

## Required Files

### Resume
- ✅ **File**: `Rithwik Swarnkar Resume.pdf` (Already added)
- **Description**: Your latest resume/CV in PDF format
- **Used in**: All pages (download button)

### Logo
- ✅ **File**: `logo.png` (Already added - DeepNeuro.dev logo)
- **Description**: Company logo
- **Used in**: Homepage hero section

## Images Needed

### University Logos (For About Page)
Please add these university logos to display in the Education section:

1. **Stanford Logo**
   - ✅ **Filename**: `Stanford Logo_block-s-right.avif` (Already added)
   - **Used in**: About page - Stanford education card
   - **Note**: The logo is displayed at 80px height

2. **UC Davis Logo**
   - ✅ **Filename**: `UCD_Logo_wordmarks_5.png` (Already added)
   - **Used in**: About page - UC Davis education card
   - **Note**: The logo is displayed at 80px height

### Project Images (For Projects Page)
Add screenshots or representative images from your Medium articles or project demos:

1. **Emotion Analyzer API**
   - **Filename**: `emotion-analyzer.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Screenshot of the web interface or architecture diagram

2. **Brain MRI Classifier**
   - **Filename**: `brain-mri.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Sample MRI scan with prediction overlay or confusion matrix

3. **Enzyme Classification**
   - **Filename**: `enzyme-classification.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Protein structure visualization or ROC curve

4. **Fake News Detection**
   - **Filename**: `fake-news.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Word cloud, feature importance, or results visualization

5. **Student Performance Analysis**
   - **Filename**: `student-performance.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Cluster visualization or PCA plot from your Medium article

6. **Diabetes Risk Predictor**
   - **Filename**: `diabetes-predictor.png`
   - **Recommended size**: 800x400px or similar 2:1 ratio
   - **Suggestion**: Feature importance chart or prediction interface

## Image Guidelines

- **Format**: PNG or JPG (PNG preferred for logos with transparency)
- **Size**: Keep individual images under 500KB for fast loading
- **Aspect Ratio**: 
  - University logos: Square or horizontal, will be displayed at 80px height
  - Project images: 2:1 ratio (800x400px recommended)
- **Quality**: High resolution but optimized for web

## Fallback Behavior

If images are not provided:
- University logos will be hidden automatically (onerror handler)
- Project images will fall back to gradient backgrounds
- The website will still look professional without images

## How to Add Images

1. Save images with the exact filenames listed above
2. Place them in this `assets` folder
3. No code changes needed - images will appear automatically
4. Test locally to ensure proper display

## Additional Assets (Optional)

You can add:
- Profile photo (`profile.jpg` or `profile.png`)
- Favicon (`favicon.ico`)
- Any other images referenced in your pages

Reference them in HTML using: `assets/filename.ext`
