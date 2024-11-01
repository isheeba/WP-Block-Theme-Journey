# How to Step-by-Step Develop the theme 

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


<details>

<summary>Minimum requirement</summary>

### [For theme](https://developer.wordpress.org/themes/basics/organizing-theme-files/)

| [Classic](https://developer.wordpress.org/themes/releasing-your-theme/required-theme-files/)    | [Block](https://make.wordpress.org/themes/handbook/review/required/#11-block-themes) | Required/download |
| -------- | ------- | ------- |
| style.css  | style.css   |Required   |
| index.php  | index.html   |Required   |
| :x:   |  theme.json   |Distribute Theme   |
| :x:   |  readme.txt   |Distribute Theme     |
| screenshot.png   |  screenshot.png   |Distribute Theme   |
  <details>

  <summary>Minimum requirement for child theme</summary>
  style.css (template name and theme name)

  </details>
</details> 