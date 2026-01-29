# Architecture Portfolio Website - User Guide

## 📁 Folder Structure

Before you start, create these folders in the same location as your HTML files:

```
your-website/
│
├── index.html
├── projects.html
├── about.html
├── contact.html
├── project-detail-1.html
├── style.css
├── README.md
│
└── images/
    ├── home/          (Put home page images here)
    ├── projects/      (Put project thumbnail images here)
    └── project-details/   (Put detailed project images here)
```

## 🏠 HOME PAGE (index.html)

### To Add Images:
1. Place your images in the `images/home/` folder
2. Open `index.html` in any text editor (Notepad, TextEdit, etc.)
3. Find the section with image grid items
4. Copy this block:
```html
<div class="grid-item grid-medium">
    <img src="images/home/YOUR-IMAGE-NAME.jpg" alt="Architecture">
</div>
```
5. Paste it where you want the new image
6. Replace `YOUR-IMAGE-NAME.jpg` with your actual filename
7. Choose a size class:
   - `grid-small` - Small square
   - `grid-medium` - Medium rectangle
   - `grid-large` - Large rectangle (2 columns wide)
   - `grid-wide` - Wide rectangle (2 columns wide, shorter)

### To Remove Images:
Simply delete the entire `<div class="grid-item">...</div>` block

---

## 📂 PROJECTS PAGE (projects.html)

### To Add a New Project:

1. **Add project thumbnail to folder**: Put the main project image in `images/projects/`

2. **Add project card**: Open `projects.html` and copy this entire block:
```html
<a href="project-detail-YOUR-PROJECT.html" class="project-card">
    <div class="project-image">
        <img src="images/projects/YOUR-IMAGE.jpg" alt="Project Name">
    </div>
    <div class="project-info">
        <h3>Your Project Name</h3>
        <div class="project-details">
            <p><strong>Location:</strong> City, Country</p>
            <p><strong>Area:</strong> 0000 sq ft</p>
            <p><strong>Completion:</strong> 2024</p>
        </div>
    </div>
</a>
```

3. **Update the information**:
   - Change `href="project-detail-YOUR-PROJECT.html"` to your project detail page name
   - Change `YOUR-IMAGE.jpg` to your image filename
   - Update project name, location, area, and completion year

4. **Create the detail page**: See next section

---

## 📄 PROJECT DETAIL PAGES

### To Create a New Project Detail Page:

1. **Copy the template**: Make a copy of `project-detail-1.html` and rename it (e.g., `project-detail-villa.html`)

2. **Update the title**: Change the `<title>` in the `<head>` section

3. **Update project information**:
   - Change the `<h1>` to your project name
   - Update Location, Area, and Completion in the `.project-meta` section
   - Replace the paragraph in `.project-description` with your project description

4. **Add images**:
   - Put all project images in `images/project-details/` folder
   - Find the `.project-images` section
   - Add images like this:
```html
<img src="images/project-details/your-image-1.jpg" alt="Description">
<img src="images/project-details/your-image-2.jpg" alt="Description">
```
   - Add as many images as you want - just keep copying the `<img>` tag

---

## 👤 ABOUT PAGE (about.html)

### To Update the Timeline Table:

1. Open `about.html` in a text editor
2. Find the `<tbody>` section inside the table
3. Each row looks like this:
```html
<tr>
    <td>2024</td>
    <td>Education info</td>
    <td>Professional work info</td>
    <td>Own work info</td>
</tr>
```

### To Edit a Row:
- Change the year in the first `<td>`
- Update text in any column
- Leave empty with `<td>-</td>` if nothing for that year

### To Add a New Row:
Copy an entire `<tr>...</tr>` block and paste it, then edit the information

### To Delete a Row:
Delete the entire `<tr>...</tr>` block

---

## 📧 CONTACT PAGE (contact.html)

### To Update Contact Information:

1. Open `contact.html`
2. Find the email section and change:
```html
<p><a href="mailto:YOUR-EMAIL@example.com">YOUR-EMAIL@example.com</a></p>
```

3. Find the phone section and change:
```html
<p><a href="tel:+919876543210">+91 98765 43210</a></p>
```

---

## 🎨 CUSTOMIZE YOUR NAME/LOGO

In **ALL** HTML files, find this line:
```html
<div class="logo">YOUR NAME</div>
```
Replace "YOUR NAME" with your actual name or studio name

---

## 🌐 UPLOADING TO YOUR DOMAIN

1. Get hosting from your domain provider or services like:
   - GitHub Pages (free)
   - Netlify (free)
   - Vercel (free)
   - Your domain's hosting service

2. Upload all files maintaining the folder structure:
   - All HTML files
   - style.css
   - images/ folder with all subfolders

3. Make sure `index.html` is in the root directory

---

## ⚠️ IMPORTANT TIPS

1. **Always backup** your files before making changes
2. **Image formats**: Use .jpg, .png, or .webp files
3. **Image names**: Avoid spaces in filenames (use dashes or underscores)
4. **File paths**: Make sure image paths match exactly (case-sensitive on some servers)
5. **Testing**: Open the HTML files in a web browser before uploading to check everything works

---

## 🆘 TROUBLESHOOTING

**Images not showing?**
- Check that the image file is in the correct folder
- Check that the filename in the HTML matches exactly (including .jpg or .png)
- Check that the path is correct (e.g., `images/home/photo.jpg`)

**Layout looks broken?**
- Make sure `style.css` is in the same folder as your HTML files
- Check that you didn't accidentally delete any closing tags like `</div>`

**Links not working?**
- Make sure the href matches the actual filename exactly
- Check that all HTML files are in the same main folder

---

## 📝 QUICK REFERENCE

### Image Sizes for Best Results:
- Home page images: 1200px - 2000px width
- Project thumbnails: 800px - 1200px width  
- Project detail images: 1500px - 2500px width

### Common HTML Tags You'll Use:
- `<img src="path/to/image.jpg" alt="description">` - Add an image
- `<p>Your text here</p>` - Add a paragraph
- `<h3>Heading</h3>` - Add a heading
- `<a href="page.html">Link text</a>` - Add a link

---

Need more help? Keep this file as a reference when updating your website!
