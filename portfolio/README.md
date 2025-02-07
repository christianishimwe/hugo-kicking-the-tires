# hugo-kicking-the-tires

We are using hugo to create awesomness

# 🚀 Hugo Kicking the Tires

**Practicing Static Site Generation with Hugo**  

![Hugo Logo](https://gohugo.io/images/hugo-logo-wide.svg)

## 📌 About This Project
This repository contains my practice work as I explore **Hugo**, a fast and flexible **static site generator** written in Go. Through this practice, I have learned to create and structure a Hugo site, define templates, work with layouts, and generate static pages.

---

## 🚀 What I Did in This Project

### 1️⃣ Installed and Set Up Hugo
- Installed Hugo using Homebrew (macOS) or Chocolatey (Windows).
- Verified the installation with:  
  ```bash
  hugo version
2️⃣ Created a New Hugo Site
This created the following directory structure:
portfolio/
├── archetypes/
├── content/
├── layouts/
├── static/
├── themes/
├── config.toml
3️⃣ Configured the Site
Updated config.toml with:
title = "My Hugo Practice Site"
4️⃣ Built the Home Page Layout
Created layouts/index.html to define the home page structure:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>{{ .Site.Title }}</title>
</head>
<body>
    <h1>{{ .Site.Title }}</h1>
    {{ .Content }}
</body>
</html>
Used Hugo's templating syntax ({{ .Site.Title }}) to pull the site title dynamically.
5️⃣ Added Content Using Markdown
Created content/_index.md for the home page:
---
title: "Welcome to My Hugo Practice Site"
date: 2025-02-07
draft: false
---
This is my portfolio site where I'm practicing Hugo.
6️⃣ Created Additional Pages
Used archetypes to generate new pages:
hugo new about.md
Edited content/about.md:
markdown
Copy
Edit
---
title: "About Me"
date: 2025-02-07
draft: false
---
This is the About page.
7️⃣ Created a Layout for Single Pages
Created layouts/_default/single.html for individual content pages:
html
Copy
Edit
<body>
    <h1>{{ .Site.Title }}</h1>
    <h2>{{ .Title }}</h2>
    <p>{{ .Date }}</p>
    {{ .Content }}
</body>
8️⃣ Ran the Hugo Development Server
Used Hugo's live preview mode to test my site locally:
hugo server
Previewed my site at http://localhost:1313.
9️⃣ Generated the Static Site
Built the final static version of the site using:
bash
Copy
Edit
hugo
This generated files in the public/ directory, ready for deployment.
💡 Key Takeaways
✅ Understood Hugo’s file structure (archetypes, content, layouts, static, themes).
✅ Created and managed content using Markdown and archetypes.
✅ Used Hugo templates to generate dynamic layouts.
✅ Ran a local Hugo server for testing before deployment.
✅ Generated a fully static site using Hugo's build process.

📌 How to Run This Project
Clone the Repository
git clone https://github.com/your-username/hugo-kicking-the-tires.git
cd hugo-kicking-the-tires
Run the Hugo Development Server
hugo server
Open http://localhost:1313 in your browser.
Build the Static Site
hugo
The site will be generated in the public/ directory.
📢 Future Enhancements
🔹 Add themes for a better design.
🔹 Improve layouts with partials and custom styling.
🔹 Explore Hugo shortcodes to add reusable components.
