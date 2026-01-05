# JInterio Website Setup Instructions

## ✅ Changes Made:

### 1. **Logo Updated**
- Changed from "Jahu Interiors" to "JInterio"
- New logo files provided:
  - `jinterio-logo.svg` (navy version)
  - `jinterio-logo-white.svg` (white version)

### 2. **Dynamic Project Gallery Added**
- Automatically loads images from project folders
- Beautiful lightbox view with keyboard navigation
- Responsive grid layout
- No code changes needed once setup

---

## 📁 Folder Structure Setup:

```
your-website/
├── index.html                    ← Updated website file
├── jinterio-logo.svg            ← New logo (navy)
├── jinterio-logo-white.svg      ← New logo (white)
└── projects/                     ← CREATE THIS FOLDER
    ├── project-1/                ← Your first project
    │   ├── 1.jpg
    │   ├── 2.jpg
    │   └── 3.jpg
    ├── project-2/                ← Your second project
    │   ├── 1.jpg
    │   ├── 2.jpg
    │   └── 3.jpg
    └── modern-kitchen/           ← Another project
        ├── image1.jpg
        ├── image2.jpg
        └── image3.jpg
```

---

## 🚀 Quick Start Guide:

### Step 1: Create the Projects Folder
Create a folder named **`projects`** in the same directory as your `index.html` file.

### Step 2: Create Project Subfolders
Inside the `projects` folder, create subfolders for each project:
- Use descriptive names like: `kitchen-remodel`, `bedroom-interior`, `living-room-design`
- Folder names will appear as titles (e.g., "Kitchen Remodel", "Bedroom Interior")

### Step 3: Add Images
Add images to each project folder:
- **Supported formats:** JPG, JPEG, PNG, WebP, GIF
- **Name them simply:** 
  - `1.jpg`, `2.jpg`, `3.jpg`, `4.jpg`, etc.
  - OR `image1.jpg`, `image2.jpg`, etc.
  - OR `img1.jpg`, `img2.jpg`, etc.

### Step 4: Update the Configuration
Open `index.html` and find this section (around line 1600):

```javascript
async function getProjectFolders() {
  return [
    'project-1',
    'project-2',
    // Add more project folder names here
  ];
}
```

**Update it with your actual folder names:**

```javascript
async function getProjectFolders() {
  return [
    'kitchen-remodel',
    'bedroom-interior',
    'living-room-design',
    'bathroom-renovation',
    'office-interior',
  ];
}
```

### Step 5: Upload and Test
1. Upload all files to your website
2. Open the website in a browser
3. The gallery will automatically load your projects!

---

## 📸 Adding New Projects (No Code Changes Needed After Setup):

1. Create a new folder in `projects/`: e.g., `projects/new-project/`
2. Add images: `1.jpg`, `2.jpg`, `3.jpg`
3. Open `index.html` and add `'new-project'` to the folder list
4. Upload and refresh - Done!

---

## 🎨 Gallery Features:

✅ **Automatic Grid Layout** - Images arranged in responsive grid
✅ **Hover Effects** - Beautiful transitions on hover
✅ **Lightbox View** - Click any image to view full-size
✅ **Keyboard Navigation:**
   - `←` and `→` arrows to navigate images
   - `Esc` to close lightbox
✅ **Mobile Responsive** - Works perfectly on phones and tablets
✅ **Lazy Loading** - Images load as you scroll (better performance)

---

## 💡 Tips:

### Image Naming:
- **Good:** `1.jpg`, `2.jpg`, `3.jpg` or `image1.jpg`, `image2.jpg`
- **Not supported:** `IMG_0123.jpg`, `photo-kitchen.jpg`, `DSC0456.jpg`

### Image Sizes:
- Recommended: 1200-1600px width
- Keep file sizes under 500KB for fast loading
- Use JPG for photos, PNG for graphics

### Folder Naming:
- **Good:** `kitchen-remodel`, `bedroom-interior`, `living_room`
- **Avoid spaces:** Use hyphens (-) or underscores (_) instead

---

## 🆘 Troubleshooting:

**Q: Images not showing?**
- Check folder names match exactly in the code
- Verify image names (must be: 1.jpg, 2.jpg, image1.jpg, etc.)
- Check file formats (jpg, jpeg, png, webp, gif only)

**Q: Project title looks weird?**
- Folder name `kitchen-remodel` becomes "Kitchen Remodel"
- Folder name `my_new_project` becomes "My New Project"
- Use hyphens or underscores, not spaces

**Q: Want to hide a project temporarily?**
- Just remove the folder name from the list in `index.html`
- OR move the folder outside the `projects` directory

---

## 📱 Mobile Menu:
The "Projects" link has been added to the mobile hamburger menu automatically!

---

## 🌐 GitHub Pages Deployment:

Your website is ready for GitHub Pages! Just:
1. Create a repository
2. Upload all files (index.html, projects folder, logos)
3. Enable GitHub Pages in repository settings
4. Your site will be live!

---

## ✉️ Support:

If you need help, contact DJ at:
- 📞 +91-9553983094
- ✉️ jahu@jinterio.com

---

**Made with ❤️ for JInterio**
