# hugo site

Go to [https://tuwei-cmd.github.io/](https://tuwei-cmd.github.io/) for preview.

## 
1. Create a New Site
    ```sh
    hugo new site quickstart
    ```
2. Add a Theme
    See [themes.gohugo.io](https://themes.gohugo.io/) for a list of themes to consider. This quickstart uses the beautiful Ananke theme.

    First, download the theme from GitHub and add it to your site's themes directory:
    ```sh
    cd quickstart
    git init
    git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
    ```
    Then, add the theme to the site configuration:
    ```sh
    echo theme = \"ananke\" >> config.toml
    ```
3. Add Some Content
    You can manually create content files (for example as content/<CATEGORY>/<FILE>.<FORMAT>) and provide metadata in them, however you can use the new command to do a few things for you (like add title and date):
    ```sh
    hugo new posts/my-first-post.md
    ```
4. Start the Hugo server
    ```sh
    hugo server -D
    ```
5. Build static pages
    It is simple. Just call:
    ```sh
    hugo -D
    ```
    Output will be in `./public/` directory by default (`-d/--destination` flag to change it, or set `publishdir` in the config file).
