# Christian Aldana — Portfolio Site

A single-page portfolio website built with HTML and CSS, designed for deployment on **GitHub Pages**. Inspired in structure by [dantsoga.github.io/dtprofile](https://dantsoga.github.io/dtprofile/).

---

## 📂 Project Structure

```
christian-aldana-portfolio/
├── index.html          ← main page
├── assets/
│   └── style.css       ← all styles
├── .nojekyll           ← tells GitHub Pages to skip Jekyll processing
└── README.md           ← this file
```

---

## 🚀 Deploy to GitHub Pages — Step by Step

### Option A: Using the GitHub Website (no command line)

1. **Create a GitHub account** at [github.com](https://github.com) if you don't already have one.

2. **Create a new repository:**
   - Click the **+** icon (top right) → **New repository**
   - **Repository name:** `christian-aldana` *(or any name you prefer — e.g., `portfolio`)*
   - Set it to **Public**
   - ✅ Check **"Add a README file"**
   - Click **Create repository**

3. **Upload the files:**
   - On your new repo page, click **Add file** → **Upload files**
   - Drag in `index.html` and the `assets` folder (with `style.css` inside)
   - Also upload the `.nojekyll` file *(see note below if you can't see it)*
   - Scroll down and click **Commit changes**

4. **Enable GitHub Pages:**
   - Go to **Settings** (top tab of your repo)
   - In the left sidebar, click **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

5. **Wait 1–2 minutes**, then refresh the Pages settings — your live URL will appear at the top:
   ```
   https://<your-github-username>.github.io/christian-aldana/
   ```

### Option B: Using the Command Line (Git)

```bash
# 1. Navigate to the project folder
cd christian-aldana-portfolio

# 2. Initialize git
git init
git add .
git commit -m "Initial portfolio site"

# 3. Create the repo on GitHub first, then connect it
git branch -M main
git remote add origin https://github.com/<your-username>/christian-aldana.git
git push -u origin main
```

Then follow **step 4** above to enable Pages.

---

## 🌐 Want a Custom URL Like the Reference Site?

The reference site lives at `dantsoga.github.io/dtprofile` because the repo is named `dtprofile`. Your URL works the same way:

| Repo name             | Live URL                                           |
| --------------------- | -------------------------------------------------- |
| `christian-aldana`    | `https://<username>.github.io/christian-aldana/`   |
| `portfolio`           | `https://<username>.github.io/portfolio/`          |
| `<username>.github.io`| `https://<username>.github.io/`  *(root domain!)*  |

💡 **Pro tip:** If you name the repo exactly `<your-username>.github.io`, the site will live at the bare root URL with no subfolder.

---

## ✏️ How to Edit the Site Later

- **Change content** (job titles, bullets, contact info): edit `index.html`
- **Change colors / fonts / spacing**: edit `assets/style.css` (look at the `:root` block at the top — all colors are CSS variables for easy theming)
- After editing, commit and push (or upload via the website) — the live site updates in ~1 minute

### Key CSS variables you can tweak

```css
--bg:        #f5f1ea;   /* page background — warm cream */
--ink:       #161a23;   /* primary text — near-black navy */
--accent:    #c9542c;   /* sharp accent — burnt orange */
--accent-2:  #1f3b5c;   /* secondary accent — deep navy */
```

---

## 📝 Note about `.nojekyll`

GitHub Pages uses Jekyll by default, which can sometimes interfere with static sites that have folders starting with `_underscore`. The empty `.nojekyll` file disables Jekyll processing.

If your file manager hides files starting with a dot, you can create it directly on GitHub: in your repo, click **Add file → Create new file**, name it `.nojekyll`, and commit (leave it empty).

---

## 🎨 Design Notes

- **Typography:** Fraunces (display serif, italic accents) + Inter Tight (body) + JetBrains Mono (metadata)
- **Aesthetic:** Editorial / refined — warm cream background with navy ink and burnt-orange accents
- **Responsive:** Works on mobile, tablet, and desktop
- **Performance:** Pure HTML + CSS, no build step, no JavaScript dependencies, no frameworks

---

© 2026 Christian Aldana
