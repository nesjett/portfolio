# 🌐 Néstor's Portfolio Static Site

![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![GitHub](https://img.shields.io/badge/-GitHub%20Pages-181717?style=flat-square&logo=github&logoColor=white) ![WordPress](https://img.shields.io/badge/-WordPress-21759B?style=flat-square&logo=wordpress&logoColor=white) ![Plugin](https://img.shields.io/badge/-Simply%20Static-5FC9F8?style=flat-square&logo=wordpress&logoColor=white)

This repository contains a static version of my portfolio website, originally built with WordPress and converted to static HTML for deployment on GitHub Pages.

## 🔄 How It Works

The site is generated using the [Simply Static](https://wordpress.org/plugins/simply-static/) WordPress plugin, which creates a complete static version of the WordPress site.

### 📋 Workflow

1. 📝 Updates are made on the WordPress admin interface
2. 🛠️ Simply Static plugin generates a ZIP file of the entire site as static HTML/CSS/JS
3. 📦 The ZIP file is downloaded and extracted
4. 🚀 The static files are pushed to this repository
5. 🌍 GitHub Pages serves the static site

### ⚙️ Configuration

- 🔗 The site is configured to use a path prefix `/portfolio` which is set in the Simply Static plugin
- 🌐 This allows the site to be hosted at `username.github.io/portfolio`

### 🎨 Custom Modifications

After generating the static site, a few manual customizations are needed:

```css
/* Hide search bar and login button in the static version */
.search-trap-focus {
    visibility: hidden;
}

#menu-item-2584 {
    display: none;
}
```

These CSS modifications are added to the index.html file to hide elements that aren't functional in the static version (search functionality and login button).

## 💻 Development

To make changes to the site:

1. 📝 Update the WordPress installation
2. 🔄 Generate a new static version using Simply Static
3. ✏️ Apply any required custom modifications
4. 📤 Push the changes to this repository
