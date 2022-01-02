# Hugo-Doodle

A simple hand drawn HTML/CSS theme made by [Chris McCormick](https://chr15m.github.io/DoodleCSS/), now powered and automated with [Hugo](https://gohugo.io), made by [1hiking](https://github.com/1hiking) for bloggers and interested alike.

Features:

- It's cute!
- 100% made with HTML & CSS
- Easy to host on your favorite provider (Netlify, GH Pages, Cloudfare, etc)
- Support for OpenGraph

## Installation and Demo

Download the theme:

```bash
git submodule add https://github.com/1hiking/Hugo-Doodle.git themes/Hugo-Doodle
```

you can alternatively use the zipped archive. To preview the site:

```bash
cd themes/Hugo-Doodle/exampleSite/
hugo server --themesDir ../.. --minify --gc
```

## Configuration file

A TOML example config is the following, although it could be JSON or YAML.

```TOML
baseURL = "https://Hugo-Doodle.netlify.com"
copyright = "Copyright © 2008-2019, Steve Francia and the Hugo Authors; all rights reserved."
languageCode = "en-us"
title = "Hugo-Doodle"

[params]
description = "Hugo-Doodle is a playful and simple Hugo theme for bloggers and writers alike"
footerText = "Nice footer"

[menu]

[[menu.main]]
identifier = "about"
name = "About"
url = "/about/"
weight = 10

[[menu.main]]
homepage = "Posts"
name = "Posts"
url = "/post/"
weight = 10

[markup]
[markup.highlight]
noClasses = true
style = "solarized-light"

```

Use `[[menu.main]]` tables to add more elements to your navigation.

## Frontmatter

These are the following frontmatter parameters that should work. As in the site config, these are in TOML (+++) but could be YAML (---):

```TOML
+++
title = "About"
description = "Hugo, the world's fastest framework for building websites"
date = "2019-02-28"
author = "Hugo Authors"
tags = ["markdown","css","html"]
categories = ["themes","syntax"]
+++
```

## Credits

- [DoodleCSS](https://github.com/chr15m/DoodleCSS) was made by Chris McCormick et alii.
- [exampleSite](https://github.com/gohugoio/hugoBasicExample) was made by Steve Francia et alii.
