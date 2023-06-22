# About this site

This is a test of the Hugo static site generator to build The Carpentries website. Using the Ananke theme, this creates a few landing pages and pulls in Carpentries data feeds.  

## Using Hugo

* [Install Hugo](https://gohugo.io/installation/)
* Clone this repository
* Inside this repository, start the Hugo server with `hugo server` and go to http://localhost:1313/

For more information review the [Hugo getting started guide](https://gohugo.io/getting-started/quick-start/).  


## Customization

Here I will list steps I've taken to set up a mockup website.

* Downloaded a theme and configured Hugo to use it:
```
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
echo "theme = 'ananke'" >> hugo.toml
```

* Created a sample blog post in draft status.  Blog posts go in `content/posts`

* Created a few sample pages.  Pages are in `content/pages`. Frontmatter of a page includes:
    * `url`: like permalink
    * `weight`: sequential idenfier for position on menu bar


* Created `_index.md` in `content/pages` (note the underscore). This blank file automatically creates a lising page for all pages in that directory.

* Created `shortcodes` inside the `layouts` folder.  Unlike Jekyll/Liquid, data feeds can not be identified in the page markdown. They must be identified in the layouts and shortcodes.  For example:
    * In `layouts/shortcodes/lessons.html` we set a value to `$all_lessons` to get a json feed and create an HTML block for what that block should look like.
    * This is called in `/content/pages/lessons.md` for each lesson program with the first parameter for the json key and the second for the value.

* Junk drawer: `misc.md` is a placeholder/sandbox for various things

