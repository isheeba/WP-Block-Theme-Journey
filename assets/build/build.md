[⬅️ Take me back Home 🏡](../../README.md)

# How to build a block theme

## Table of Contents
- [Basic theme structure](#basic-theme-structure)
- [Setting up theme.json](#setting-up-themejson)
- [Creating templates](#creating-templates)
- [Building template parts](#building-template-parts)
- [Adding custom block patterns](#adding-custom-block-patterns)
- [Exporting](#exporting)
- [Minimum requirement](#minimum-requirement)
- [Steps I followed](#steps-i-followed)
- [Troubleshooting/FAQ](#troubleshootingfaq)

## Basic theme structure

## Setting up theme.json
- [JSON Guide](https://developer.wordpress.org/block-editor/reference-guides/theme-json-reference/theme-json-living/)
- [version](https://developer.wordpress.org/block-editor/reference-guides/theme-json-reference/)


### Loading Preference (lowest to highest)
- `wp-includes/theme.json` -  defines the default settings and styles.
- `<child_theme_name>/theme.json` - takes precedence over the theme.json file in the parent theme.
- `<theme_name>/theme.json` - Theme settings
- `User Configured` - Within the Site Editor any changes that are added to the database through changes made to global styles or even templates and saved. This will override and takes priority over all other levels in the hierarchy.


## Creating templates
#### Common Templates
- <b>Single:</b> used when a visitor requests a single post as we saw in our example.
- <b>Page:</b> used when visitors request individual pages.
- <b>Archive:</b> used when visitors request posts by archive type, for example, category or author.
- <b>Search:</b> used for search results when a visitor does a search on a website
- <b>404:</b> used when WordPress cannot find a post page or other content that matches the visitors request.



## Building template parts
## Adding custom block patterns
## Exporting


### Minimum requirement

#### [For theme](https://developer.wordpress.org/themes/basics/organizing-theme-files/)

| [Classic](https://developer.wordpress.org/themes/releasing-your-theme/required-theme-files/)    | [Block](https://make.wordpress.org/themes/handbook/review/required/#11-block-themes) | Required/download |
| -------- | ------- | ------- |
| style.css  | style.css   |Required   |
| index.php  | index.html   |Required   |
| :x:   |  theme.json   |Distribute Theme   |
| :x:   |  readme.txt   |Distribute Theme     |
| screenshot.png   |  screenshot.png   |Distribute Theme   |

#### Minimum requirement for child theme 
  style.css (template name and theme name)

 

### Steps I followed
* Add `style.css` + `index.html` : shows `Empty template: Index` on front-end
* Added header and footer : Site-editor => Patterns => Add New patterns
*


### [Troubleshooting/FAQ](debugging.md)
* [How does WordPress identify theme type?](debugging.md#how-does-wordpress-identify-theme-type)
* [How to identify theme type from backend?](debugging.md#how-to-identify-theme-type-from-backend)
* [What displays with minimum files?](debugging.md#what-displays-with-minimum-files)