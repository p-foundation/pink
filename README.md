# Frontend of the Pink App project

[Figma mockup](https://www.figma.com/file/TYlLseXoMXDflJYbU1DGHa/HTML-2-%2F-%D0%9F%D0%B8%D0%BD%D0%BA?type=design&node-id=1-323&mode=design&t=03daQbmntoeCoxSu-0)


**Important:** _do not delete or modify the following files and folders without authorization:_
_`.editorconfig`, `.gitignore`, `.nojekyll`, `.github`_

To get familiar with our guidelines, please refer to [CONTRIBUTING.md](Contributing.md) for instructions.

## Installation

```bash
# Clone the repository
git clone https://github.com/p-foundation/pink-app.git

# Enter the project directory
cd pink-app
```

## UI Playground

The `/components.html` page acts as a components library, allowing us to collaborate on UI elements (smaller BEM blocks) in an isolated setting. Use this page to focus on individual blocks without distractions from the entire application.

Here's a simple guide to get the most out of it:
### 1. Open /components.html with your local server:
Access the UI library by opening this page through your local server and adding `/components.html` to the server's address.

### 2. Creating a New Component:
To add a new component, use the template below within the `/components.html` file:

```html
<li class="component">
    <!-- Fill out your block name -->
    <h2 class="component__name">UI Component (Block) Name</h2>
    <!-- Add a description to explain details about the block. Remove the line if no description is provided. -->
    <p class="component__description">UI Component description (optional)</p>
    <div class="component__wrapper component__wrapper_theme_light">
        <!-- Your component goes here -->
    </div>
</li>
```

### 3. Choose contrast background
There are two background options available for the component container to create contrast with differently colored elements. Pick a background to ensure optimal visibility and aesthetics within the UI library.
- `component__wrapper_theme_light` - for a light background, and
- `component__wrapper_theme_dark` - for a dark background.

### 4. Use `pages/components.css` for importing your styles

---

<a href="https://pgds.xyz/"><img width="250" height="54" alt="Palianytsia Foundation" src="https://raw.githubusercontent.com/naumch1k/palyanitsa/main/src/shared/images/full-logo.png"></a>

The repository is created for learning adaptive web design and team collaboration through git and GitHub

---
