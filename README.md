# Yoichii on Tech

## Overview
* This blog aims to share technical knowledge.
* Articles are written in both Japanese (my native language) and English.

## Blog Upgrades

### Enhance Layout and Styles
* Add a specific class for post types in the `<body>` tag within `_layouts/base.html`.
* Add custom styles in `_scss/minima/custom-styles`.

### Make My Blog Multilingual
* Create separate article directories for each language:
    * Set up `ja` and `en` directories.
        * Place Japanese posts in `ja/_posts` and English posts in `en/_posts`.
    * Remove `index.markdown` and add `index.html` for language-based redirection.
* Establish a permalink structure like `/lang/xxx`:
    * Update `_config.yml`.
* Assign the appropriate `lang` option for each page:
    * Update `_config.yml`.
* Adjust the page content based on the `lang` option:
    * Override `_layouts/home.html`.
* Implement the language-switching link:
    * Create a new file named `_includes/lang_link.html`.
    * Override `_includes/header.html` to incorporate the language-switching link.
