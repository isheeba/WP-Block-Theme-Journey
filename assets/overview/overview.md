[⬅️ Take me back Home 🏡](../../README.md)

- What is a Block Theme?

  - [WordPress Block Theme Documentation](https://developer.wordpress.org/block-editor/how-to-guides/themes/block-theme-overview/)
  - [Introduction to Block Themes](https://learn.wordpress.org/tutorial/introduction-to-block-themes/)
  - [Block Theme Definition - WordPress.org](https://wordpress.org/documentation/article/block-themes/)

- Why use Block Themes?

  - [Benefits of Block Themes](https://developer.wordpress.org/block-editor/how-to-guides/themes/block-theme-overview/#benefits)
  - [Block Themes vs Classic Themes](https://kinsta.com/blog/wordpress-block-themes/)
  - [The Future of WordPress Themes](https://wordpress.org/news/2021/12/wordpress-5-9-features-block-themes/)

- Key differences from Traditional(classic) Themes
  - [Block vs Classic Theme Comparison](https://fullsiteediting.com/lessons/block-themes-vs-classic-themes/)
  - [Theme Architecture Changes](https://developer.wordpress.org/block-editor/how-to-guides/themes/theme-json/)
  - [Block Theme Structure Guide](https://developer.wordpress.org/themes/block-themes/block-theme-structure/)

| Key                 |      Classic       | Block                      |
| ------------------- | :----------------: | -------------------------- |
| Editable            |      Content       | layout, content            |
| Basic Customization |     Customizer     | FSE                        |
| Displays from       |    Theme Files     | Database & Theme.json      |
| Migrate             |      Git/FTP       | Export, Git                |
| Export Theme        |        :x:         | combines DB + theme files. |
| Child Theme         | :white_check_mark: | :white_check_mark:         |
|                     |                    |                            |

> [!NOTE]
> Block themes are great for creative clients, traditional themes suit corporate branding

<details>
<summary>When block Theme is ideal</summary>
- Clients who prefer hands-on design and are comfortable using WordPress's design tools.
</details>

<details>
<summary>When block Theme might not work</summary>
-  Large businesses with strict branding standards where design consistency is crucial.
- If a client is not involved in creating content beyond simple text, a traditional theme is the best choice.

</details>

<details>
<summary>What is Block Editor and Site Editor?</summary>

The Block Editor only allows us to add content to pages and posts.
Site Editor gives you the ability to edit your site cohesively. You can edit the look and feel, modify templates, and add content to pages.

</details>

## Required tools and setup

- [Block Theme Development Tools](https://developer.wordpress.org/block-editor/getting-started/devenv/)
- [Create Block Theme Plugin](https://wordpress.org/plugins/create-block-theme/)
- [Theme Development Environment Setup](https://developer.wordpress.org/block-editor/getting-started/tutorials/block-based-themes/)

<details open>
<summary> What I use </summary>

- IDE : [Cursor](https://www.cursor.com) based on [vscode](https://code.visualstudio.com)
- Local Env setup : [Local](https://localwp.com) (alternative [studio](https://developer.wordpress.com/studio/) )
</details>