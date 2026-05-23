# Dylan Smith — Portfolio

Editorial communications portfolio built with HTML/CSS. Designed to be hosted free on GitHub Pages.

---

## 🚀 How to publish on GitHub Pages (step by step)

### Step 1 — Create a new repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon (top right) → **New repository**
3. Name it exactly: `dylansmith.github.io`  
   *(replace `dylansmith` with your actual GitHub username)*
4. Set it to **Public**
5. Click **Create repository**

### Step 2 — Upload your files
1. On your new repo page, click **uploading an existing file**
2. Drag and drop ALL these files and folders:
   - `index.html`
   - `css/` folder (with `style.css` inside)
   - `pages/` folder (with all the `.html` files inside)
3. Scroll down, click **Commit changes**

### Step 3 — Enable GitHub Pages
1. In your repo, click **Settings** (top tab)
2. Scroll down to **Pages** (left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, select **main** and **/ (root)**
5. Click **Save**
6. Wait ~60 seconds, then your site will be live at:  
   `https://dylansmith.github.io` ✨

---

## 📁 File structure

```
dylansmith.github.io/
├── index.html              ← Main landing page
├── css/
│   └── style.css           ← All shared styles
└── pages/
    ├── projects.html        ← Independent Projects
    ├── writing.html         ← Writing samples
    ├── design.html          ← Design work
    ├── campaigns.html       ← Campaigns
    ├── newsletters.html     ← Newsletters
    ├── pr.html              ← Public Relations
    └── contact.html         ← Contact page
```

---

## ✏️ How to customize

### Replace placeholder content
Every page has placeholder items marked with comments like:
```
<!-- Replace with your real campaigns -->
```
Just edit the HTML in any text editor (Notepad, TextEdit, VS Code) and replace the placeholder text/links with your real work.

### Add your photo
In `index.html`, find:
```html
<div class="intro-photo-placeholder">Your photo</div>
```
Replace with:
```html
<img src="images/your-photo.jpg" alt="Dylan Smith">
```
Then create an `images/` folder and upload your photo there.

### Add your resume PDF
In `index.html`, find:
```html
<a class="doc" href="#" target="_blank">
```
Replace `#` with the path to your PDF, e.g.:
```html
<a class="doc" href="files/dylan-smith-resume.pdf" target="_blank">
```
Create a `files/` folder and upload your PDFs there.

### Update contact info
Search for `dylansmith@gmail.com`, `(407) 479-0765`, and `linkedin.com/in/dylansmith` across the HTML files and replace with your real details.

### Change colors
Open `css/style.css` and edit the variables at the top:
```css
:root {
  --cream:    #F0EBE1;   /* background */
  --crimson:  #9B2A1A;   /* signature red */
  --ink:      #1A1008;   /* dark sections */
}
```

---

## 🔤 Fonts used
- **Playfair Display** — display headings (via Google Fonts, free)
- **Cormorant Garamond** — body text (via Google Fonts, free)
- **DM Sans** — UI labels (via Google Fonts, free)

All fonts load automatically from Google Fonts — no installation needed.

---

## 🆘 Need help?
If something looks broken, the most common fix is making sure the file paths are correct.  
Pages inside the `pages/` folder link to CSS with `../css/style.css` (two dots = go up one folder).  
The main `index.html` links to CSS with `css/style.css` (no dots needed).
