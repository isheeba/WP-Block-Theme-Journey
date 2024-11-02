[⬅️ Take me back Home 🏡](../../README.md)

# Core Concepts

## Table of Contents
- [Theme.json Configuration](#themejson-configuration)
- [Block Templates & Template Parts](#block-templates--template-parts)
  - [Templates](#templates)
  - [Template Parts](#template-parts)
- [Block Patterns](#block-patterns)
- [Global Styles](#global-styles)
- [Theme Blocks vs Core Blocks](#theme-blocks-vs-core-blocks)
  - [Core Blocks](#core-blocks)
  - [Theme Blocks](#theme-blocks)
  - [Custom Block Example](#custom-block-example)

## Theme.json Configuration
Theme.json is the foundation of block themes, controlling:

- 🎨 Global styles and typography
- ⚙️ Block-level settings
- 🎯 Custom properties
- 🖼️ Layout defaults

## Block Templates & Template Parts
| Feature             | Template                                                 | Template Part                                              |
|---------------------|----------------------------------------------------------|------------------------------------------------------------|
| **Purpose**         | Defines overall page layout                              | Defines reusable sections within a template                |
| **Scope**           | Full page or post layout                                 | Specific parts like headers, footers, or sidebars          |
| **Editing Location**| Accessible in Full Site Editor                           | Managed within Template Part editor or Full Site Editor    |
| **Reusability**     | Limited to the specific page/post types                  | Can be reused across multiple templates and parts of a site|
| **Modification**    | Changes apply to the specific template only              | Changes apply to all instances of the template part        |

### Templates
Core templates that define your site's structure:
- `index.html` (required)
- `single.html`
- `archive.html`
- `page.html`
- `404.html`
- `search.html`

### Template Parts
Reusable components like:
- `header.html`
- `footer.html`
- `sidebar.html`

## Block Patterns
Pre-designed block layouts that can be:
- ♻️ Reused across pages
- 🎨 Customized for consistency
- 📦 Packaged with themes

| Feature            | Template Part                                         | Pattern                                          |
|--------------------|-------------------------------------------------------|--------------------------------------------------|
| **Purpose**        | For reusable structural elements (header, footer)      | For quick layout and design of complex block setups |
| **Definition**     | Defined in PHP, often used in theme templates          | Created in the block editor; no coding required    |
| **Customization**  | Limited; generally consistent across pages             | Highly customizable; users can adjust blocks and styles |
| **Use Cases**      | Headers, footers, sidebars                             | Call-to-action sections, testimonials, galleries   |
| **User Access**    | Mostly for theme developers                            | Accessible to any editor within the block editor   |

## Global Styles
Control site-wide appearance through:
- 🎨 Color schemes
- 📝 Typography settings
- 📏 Spacing defaults
- 🖼️ Layout preferences

## Theme Blocks vs Core Blocks

### Core Blocks
- Built into WordPress
- Always available
- Maintained by WordPress

### Theme Blocks
- Custom functionality
- Theme-specific features
- Requires maintenance
- Created using block.json

### Custom Block Example
```json
{
    "apiVersion": 2,
    "name": "mytheme/custom-block",
    "title": "Custom Block",
    "category": "widgets",
    "icon": "smiley",
    "description": "A custom block example",
    "supports": {
        "html": false
    },
    "textdomain": "mytheme",
    "editorScript": "file:./index.js",
    "editorStyle": "file:./index.css",
    "style": "file:./style-index.css"
}
```