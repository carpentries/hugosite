# About this site

This is a test of the Hugo static site generator to build The Carpentries website.

## Using Hugo

* [Hugo getting started guide](https://gohugo.io/getting-started/quick-start/)

## Customization

Here I will list steps I've taken to set up a mockup website.

* Downloaded a theme and configured Hugo to use it:
```
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
echo "theme = 'ananke'" >> hugo.toml
```

* Created a sample blog post in draft status.  Blog posts go in `content/posts`