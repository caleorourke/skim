# Ferris

Ferris is a one-page boilerplate for publishing content on GitHub. It's designed specifically for hosting on GitHub using [GitHub Pages](http://pages.github.com) and serving up locally using [Jekyll](http://jekyllrb.com). Take a peek at the demo below and see how simple it is to roll your own site without having to use fancy code.

<a href="http://caleorourke.github.io/ferris" target="_blank">Ferris on GitHub</a>


## Quick Install

1. Clone from GitHub and go into the directory (~3 seconds). Directory size hovers around ~76 KB.

        $ git clone -o master https://github.com/caleorourke/ferris.git
        $ cd ferris


2. Install Bundler (~5 seconds).

        $ gem install bundler


3. Install runtime dependencies (~15 seconds).

        $ bundle install


## Roll Your Own

1. Make a fresh clone and go into the directory.

        $ git clone https://github.com/username/bueller.git
        $ cd bueller

2. Create a new `gh-pages` branch.

        $ git checkout --orphan gh-pages

3. Copy the contents from <samp>/ferris</samp> to <samp>/bueller</samp>.

        $ cp -r ~/ferris/* ~/bueller

4. Push your site to GitHub.

        $ git add .
        $ git commit -a -m "first commit"
        $ git push origin gh-pages


## Default Config

~~~yml
#
# * Config
# * Stores static configuration and project info
# *
# * Copyright © SoftLayer, an IBM Company
# * Released under the MIT license
#

# 1. Spaces only, no tabs.
# 2. Wrap words in quotes wherever commas are used.
# 3. For options, use Y or N. Anything else will disable the option.


# ==============================
# Project
# ==============================

github:
    title:      Name of Your Website
    tagline:    Something Catchy to Describe your Website
    owner:      Name of Whoever Owns This
    license:    MIT

# ==============================
# Social
# ==============================

twitter:
    handle:     Your Twitter Name
    hashtags:   "separate,hashtags,with,commas"
    text:       "Check out our brand new website."
keywords:       "separate,keywords,with,commas"

# ==============================
# Options
# ==============================

analytics:
    enabled:    N
blur:
    enabled:    N
easing:
    enabled:    Y
indexing:
    enabled:    Y
version:
    enabled:    N

# ==============================
# Google Analytics
# ==============================

google:
    id:         UA-X

# ==============================
# Markdown
# ==============================

markdown:       redcarpet
redcarpet:
    extensions: ["autolink",
                 "fenced_code_blocks",
                 "highlight",
                 "lax_spacing",
                 "quote",
                 "smart",
                 "strikethrough",
                 "superscript",
                 "tables",
                 "underline",
                 "with_toc_data"]

# ==============================
# Server
# ==============================

permalink:      pretty
exclude:        [".gitignore",
                 "CONTRIBUTING.md",
                 "Gemfile"]
~~~

## Contributing

Anyone is welcome to submit an issue or request. All we ask is that you glance through our [contributing guidelines](CONTRIBUTING.md) first.


## License

Our code and documentation is licensed under the MIT license. By contributing your code, you agree to license your contribution under the terms of this license.
