# 📸 Photo Instructions

This guide explains where and how to add photos to your GitHub Pages site.

## Photo Locations

### 1. **Hero Section Profile Photo** (Recommended)
- **Location**: `/assets/images/profile.jpg`
- **File Path**: Place your photo at `manudwd/assets/images/profile.jpg`
- **Recommended Size**: 400x400px to 800x800px (square, 1:1 aspect ratio)
- **Format**: JPG, PNG, or WebP
- **Current Code Location**: `index.html` line 12

**How to add:**
1. Add your profile photo to the `assets/images/` folder
2. Name it `profile.jpg` (or update the filename in `index.html` if using a different name)
3. The photo will automatically appear in the hero section with a circular frame and floating animation

**If you don't add a photo:**
- The photo container will automatically hide (no error will show)
- The layout will adjust gracefully

### 2. **About Section Photo** (Optional)
- **Location**: `/assets/images/about.jpg`
- **File Path**: Place your photo at `manudwd/assets/images/about.jpg`
- **Recommended Size**: 600x600px to 1000x1000px (square recommended)
- **Format**: JPG, PNG, or WebP
- **Current Code Location**: `index.html` lines 42-44 (currently commented out)

**How to add:**
1. Add your photo to the `assets/images/` folder
2. Name it `about.jpg`
3. In `index.html`, find the About section (around line 42)
4. Uncomment the lines that say:
   ```html
   <!-- <div class="about-image-container">
     <img src="/assets/images/about.jpg" alt="About Manu Dwivedi" class="about-image" onerror="this.style.display='none'; this.parentElement.style.display='none';">
   </div> -->
   ```
5. Remove the `<!--` and `-->` comment markers

## Image Optimization Tips

1. **Compress your images** before uploading:
   - Use tools like [TinyPNG](https://tinypng.com/) or [Squoosh](https://squoosh.app/)
   - Aim for file sizes under 200KB for faster loading

2. **Square images work best**:
   - Both photo containers are circular/square
   - Crop your photos to 1:1 aspect ratio for best results

3. **Professional photos recommended**:
   - Use high-quality, well-lit photos
   - Professional headshots work great for the hero section

## File Structure

```
manudwd/
├── assets/
│   ├── images/
│   │   ├── profile.jpg    ← Your main profile photo (REQUIRED for hero)
│   │   └── about.jpg      ← Optional photo for About section
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
└── index.html
```

## Testing

After adding photos:
1. Commit and push to GitHub
2. Wait for GitHub Pages to rebuild (usually 1-2 minutes)
3. Visit your site and check if photos appear
4. If photos don't show, check:
   - File path is correct
   - Filename matches exactly (case-sensitive)
   - File is committed to the repository

## Need Help?

- Check browser console (F12) for any image loading errors
- Verify the file path in `index.html` matches your actual file location
- Ensure images are in the `assets/images/` folder, not elsewhere

