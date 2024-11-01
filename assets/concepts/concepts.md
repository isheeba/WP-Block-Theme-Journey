[⬅️ Take me back Home 🏡](../../README.md)

# Core Concepts

## Theme.json Configuration
Theme.json is the foundation of block themes, controlling:

- 🎨 Global styles and typography
- ⚙️ Block-level settings
- 🎯 Custom properties
- 🖼️ Layout defaults

### Key Sections
```json
{
    "version": 2,
    "settings": {
        "color": {
            "palette": [],
            "gradients": []
        },
        "typography": {
            "fontSizes": [],
            "fontFamilies": []
        },
        "layout": {}
    },
    "styles": {}
}
```

## Block Templates & Template Parts

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

### Pattern Registration
```php
register_block_pattern(
    'mytheme/my-pattern',
    array(
        'title'       => __('My Pattern', 'mytheme'),
        'description' => __('A custom pattern.', 'mytheme'),
        'content'     => '<!-- wp:group -->'
    )
);
```


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

gc### Custom Block Example
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