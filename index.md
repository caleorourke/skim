---
layout: page
---

# Introduction

__Voted best boilerplate in North Dallas by our Grandmothers.__

{{site.github.title}} is a one-page boilerplate for publishing technical content on GitHub. It provides the facilities to write exclusively in [Markdown](http://en.m.wikipedia.org/wiki/Markdown) or HTML and spin-up [Jekyll](http://jekyllrb.com)-powered websites.

Browse the sections below and see just how simple it is to roll your own GitHub site for free without using fancy code.

---

# Features and Delighters

__{{site.github.title}} is chock-full of nifty doodads.__

## Features

* Responsive and mobile-friendly
* Fast load times
* Centralized setup from a single configuration file
* [Google Analytics](http://github.com/{{site.github.owner_name}}/{{site.github.project_title}}/blob/gh-pages/_includes/options/analytics.html)
* WDM gem for supporting modern Windows OSes
* Pretty URLs
* [Version](http://github.com/{{site.github.owner_name}}/{{site.github.project_title}}/blob/gh-pages/_includes/options/version.html) to fetch the most recent release peg from GitHub
* [Top](http://github.com/{{site.github.owner_name}}/{{site.github.project_title}}/blob/gh-pages/_includes/options/top.html) for setting offset thresholds while scrolling
* [Index](http://github.com/{{site.github.owner_name}}/{{site.github.project_title}}/blob/gh-pages/_includes/options/index.html) to build table of contents on-the-fly
* [Metadata](http://help.github.com/articles/repository-metadata-on-github-pages) for GitHub Pages

## Core Environment

* CSS3/HTML5
* JavaScript/jQuery
* Python
* Ruby
* [Font Awesome](http://fortawesome.github.io/Font-Awesome) iconic font
* [Jekyll](http://jekyllrb.com) for free web hosting using GitHub Pages
* [Liquid](http://liquidmarkup.org) template language
* [Normalize](http://necolas.github.io/normalize.css) for CSS normalization and resets
* [Pygments](http://pygments.org) for code highlighting
* [Redcarpet](http://github.com/vmg/redcarpet) for Markdown-compatibility and rendering
* [Bootstrap](http://twitter.github.io/bootstrap) grids and media queries

---

# Browser Compatibility

__Recommended browsers and platforms for the best usability and performance.__

Starting from best to worst, we recommend the latest versions of the following browsers.

* Chrome (~100%)
* Safari (~75%)
* Firefox (~50%)
* Opera (~50%)
* Internet Explorer (~25%)

Below is a comparison of each browser on different OS platforms.

| Platform    | Chrome     | Firefox     | Internet Explorer      | Opera     | Safari     |
| ----------- |:----------:|:-----------:|:----------------------:|:---------:|:----------:|
| Android     | __Yes__    | No          | N/A                    | No        | N/A        |
| iOS         | __Yes__    | N/A         | N/A                    | No        | __Yes__    |
| Mac OS X    | __Yes__    | __Yes__     | N/A                    | __Yes__   | __Yes__    |
| Windows     | __Yes__    | __Yes__     | __Yes__                | __Yes__   | __Yes__    |

> Apple no longer provides updates for Windows-native Safari browsers. Due to major lapses in critical updates, we do not recommend using Safari on Windows.

## Legacy Browsers

As for legacy browsers, support is limited to whatever the browser can handle. You can try using [Modernizr](http://modernizr.com) to circumvent compatibility issues, but it's not perfect.

~~~html
<script src="//cdnjs.cloudflare.com/ajax/libs/modernizr/2.8.2/modernizr.min.js"></script>
~~~

---

# Prerequisites

__What you'll need to bring before arriving to the party.__

{{site.github.title}} requires the minimum version of __Ruby__ below. It also requires __Python__ to run __Pygments__, but only if you’re planning to use code highlights. Otherwise, you won't need it.

* Ruby 1.9.3
* Python 2.7
* Pygments 1.6

## Ruby

{{site.github.title}} requires __Ruby 1.9.3__ at minimum. To download and install Ruby, click the button below.

<a class="button solid-green" href="http://www.ruby-lang.org/en/installation" target="_blank">Download</a>

> If you have Ruby, but aren’t sure which version, run `ruby -v`. This will show which version you have.

## Python

{{site.github.title}} requires __Python 2.7__. To download and install Python, click the button below.

<a class="button solid-green" href="https://www.python.org/download/releases/2.7" target="_blank">Download</a>

> If you have Python, but aren’t sure which version, run `python --version`. This will show which version you have.

## Pygments

{{site.github.title}} requires __Pygment 1.6__. To download and install Pygments, click the button below.

<a class="button solid-green" href="http://pygments.org/download" target="_blank">Download</a>

> If you have Pygments, but aren’t sure which version, run `pygmentize -V`. This will show which version you have.

---

# Download and Clone

__How to download or clone {{site.github.title}} from GitHub.__

## Downloading {{site.github.title}}

There are a number of ways to download {{site.github.title}}. Scroll through the options below and pick one that works best for you.

### Tarball Download

Click <a href="{{site.github.repository_url}}/tarball/master" target="_blank">download <i class="fa fa-cloud-download"></i></a> or run the command below.

~~~bash
$ curl -OL {{site.github.repository_url}}/tarball/master
~~~

### ZIP Download

Click <a href="{{site.github.repository_url}}/zipball/master" target="_blank">download <i class="fa fa-cloud-download"></i></a> or run the command below.

~~~bash
$ curl -OL {{site.github.repository_url}}/zipball/master
~~~

## Cloning {{site.github.title}}

There are also a few ways to clone {{site.github.title}}. Scroll through the options below and pick one that works best for you.

### HTTPS Clone

Run the command below to clone over HTTPS.

~~~bash
$ git clone {{site.github.repository_url}}.git
~~~

### SSH Clone
Run the command below to clone over SSH.

~~~bash
$ git clone git@github.com:{{site.github.owner_name}}/{{site.github.repository_name}}.git
~~~

---

# Installation

__How to install and add runtime dependencies.__

1. Go into the root directory for {{site.github.title}}.
2. Run the command to install Bundler.
3. Run `bundle install` to load the runtime dependencies.

```bash
$ cd {{site.github.project_title}}
$ gem install bundler
$ bundle install
```

---

# Configuration

__Who's your Daddy and what does he do?

The `_config.yml` is a [YAML](http://en.m.wikipedia.org/wiki/YAML) file for storing and propagating nearly all of the site's configuration. Anything not handled by it gets handled behind the scenes by [metadata](http://help.github.com/articles/repository-metadata-on-github-pages). This means you can configure your entire site using just a single file.

## Project

1. Open `_config.yml` using any text editor.
2. Find `Project`.
3. Fill in each field with details about your project.

~~~yaml
# ==============================
# Project
# ==============================

github:
    title:      Ferris
    tagline:    A one-page boilerplate for publishing content on GitHub
    owner:      "SoftLayer, an IBM Company"
    license:    MIT
~~~

> Use spaces to separate content. Do not use tabs.

## Social

1. Scroll down to the second group of setting labeled `Social`.
2. Fill in each field with details about your social network.

~~~yaml
# ==============================
# Social
# ==============================

twitter:
    handle:     SoftLayerLabs
    hashtags:   "css,boilerplate,github-pages"
    text:       "Try Ferris, a one-page boilerplate for posting technical content on GitHub."
keywords:       "boilerplate,css,feo,framework,github,github pages,html5,IBM,jekyll,liquid,markdown,one-page,redcarpet,softlayer"
~~~

> Wrap words in quotes wherever commas are used.

## Options

1. Scroll down to the third group called `Options`.
2. Type <kbd>Y</kbd> to enable or <kbd>N</kbd> to disabled any of the options.

~~~yaml
# ==============================
# Options
# ==============================

analytics:
    enabled:    N
index:
    enabled:    Y
smooth:
    enabled:    Y
version:
    enabled:    N
~~~

Below is a brief overview of each option.

| Option     | Default | Description   |
| ---------- |:-------:| ------------- |
| Analytics  | N       | Google service that generates detailed statistics about your site's traffic |
| Index      | Y       | Captures all the H1 headers and drops them into a modal |
| Smooth     | Y       | Provides thresholds and smooth animation for page scrolling |
| Version    | N       | Fetches the last pegged release from GitHub and shows it under <kbd>Get Started</kbd> |

> For these options, use Y or N. Anything else will disable the option.

## Google Analytics

1. Go to [Google Analytics](http://www.google.com/analytics).
2. Create a free account.
3. Setup properties for things we want to track, such as demographics, bounce rates, and session count.
4. Request a UA number for your site.
5. Add your UA number to the `id`.

~~~yaml
# ==============================
# Google Analytics
# ==============================

google:
    id:         UA-40037365-5
~~~

---

# Deployment

__Learn how to make Jekyll transform raw text into a complete, ready-to-publish static website.__

## Local Deployment

Run the following command to preview a local instance of your site.

```bash
$ jekyll serve
```

Once Jekyll has started, fire up a browser and type in <kbd>localhost:4000</kbd> for the web address. This will show the site Jekyll just generated.

### Watch Jekyll

If you want to monitor changes and apply updates without having to restart Jekyll, add the `--watch` option to the command.

```bash
$ jekyll serve --watch
```

### Kill Jekyll

Serve mode lasts forever. It won't timeout after a period of non-usage. Press <kbd>CTRL+C</kbd> to kill the process.

## Web Deployment

GitHub Pages are public web pages hosted on GitHub’s `github.io` domain. Jekyll powers it behind the scenes, which makes this a snazzy way to host a free, Jekyll-powered website.

Hosting on GitHub works by storing content in a branch called `gh-pages`. This means your website can be kept in the same repository as your codebase. This branch, however, will be rendered using Jekyll, and your site will get served up under a subpath of your user pages subdomain, such as `username.github.io/project`.

### Roll Your Own

Start by creating a new orphan branch (e.g. a branch that has no common history with an existing branch) in your repository. The safest way to do this is to make a fresh clone. In this example, we're going to create one called `bueller`.

```bash
$ git clone https://github.com/username/bueller.git
```

> The example above has `username` as a placeholder. This is where you want to type your actual GitHub username.

Once you have a fresh clone, you'll need to create the new `gh-pages` branch and remove any content from the working directory.

```bash
$ cd bueller
$ git checkout --orphan gh-pages
$ git rm -rf .
```

Next, copy all the content from `/{{site.github.project_title}}` to your `/bueller` directory.

```bash
$ cp -r ~/{{site.github.project_title}}/* ~/bueller
```

Now that you have content in your own directory, you can push it to GitHub.

```bash
$ git add .
$ git commit -a -m "first commit"
$ git push origin gh-pages
```

After you push to `gh-pages`, your site will be available at `username.github.io/bueller`.

> It can take up to ten minutes before your site is available, but in most cases, it's ready instantly.

---

# Code Organization

__Deep dive into the directory structure, workflow, and content for {{site.github.title}}.__

## Pre-Install

Below is the basic spread for {{site.github.title}} (not including `site` for Jekyll).

```
├─ _includes
│  └─ options
├─ _layouts
├─ public
│  ├─ css
│  └─ images

3 directories, 3 subdirectories
```

> Folders beginning with an underscore tell Jekyll to use the content within them to generate your site. They're not exposed after the site is transformed, though.

## Post-Install

A working environment will have one more directory: `site` (Jekyll).

```
├─ _includes
│  └─ options
├─ _layouts
├─ _site
├─ public
│  ├─ css
│  └─ images

4 directories, 3 subdirectories
```

## Directory

Here's an overview of what each directory does or contains.

| Directory                       | Overview  |
| ------------------------------- | --------- |
| `_includes`          | Semantic HTML elements and reusable content |
| `_includes/options`  | Components configured to run requests for specific content |
| `_layouts`           | Reusable templates for specific uses |
| `_site`              | Where Jekyll places generated sites after it's transformed |
| `public`             | Static directory for CSS stylesheets and images |
| `public/css`         | Static CSS stylesheets in `.css` format |
| `public/images`      | Static images files in `.ico`, `.jpg`, and `.png` formats |

---

# Useful Resources

__Nonspecific information written during development that might be useful to some but not everyone.__

## DOM Elements

As an optional feature, you can render the `#github-version` DOM element that we embedded within JavaScript. This element will pull in the tag/version number for the last pegged release. To enable or disable this option, check out the [Options](#options) section.

## Handlers

{{site.github.title}} initializes event handlers whenever the DOM is fully loaded. It also has controls for animating scroll events and a built-in handler to process callbacks for fetching JSON data from GitHub.

## Metadata

We harness several metadata tags using GitHub's [metadata](http://help.github.com/articles/repository-metadata-on-github-pages) feature, albeit not all of them for a number of reasons.

Below is a list of metadata tags we use.

* {%raw%}`{{site.github.owner_name}}`{%endraw%}
* {%raw%}`{{site.github.owner_url}}`{%endraw%}
* {%raw%}`{{site.github.project_title}}`{%endraw%}
* {%raw%}`{{site.github.repository_url}}`{%endraw%}
* {%raw%}`{{site.github.url}}`{%endraw%}

## Code Styles

Use the settings below to help unify coding styles across different editors.

```
indent_style = space
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = false
indent_size = 4
```

Sublime Text users can configure these settings manually by opening `Preferences > Settings - User`, inserting the lines below, and saving your settings.

```
"translate_tabs_to_spaces": true,
"tab_size": 4,
"ensure_newline_at_eof_on_save": false,
"default_encoding": "UTF-8",
"default_line_ending": "lf",
"trim_trailing_white_space_on_save": true
```

## Sublime Packages

We use Sublime exclusively. One of its few drawbacks, though, is it does not include every syntax highlight. To get certain highlights, you have to install them by hand. Use the instructions below to perform the install processes for __Jekyll__ and __Liquid__.

[Package Control](http://sublime.wbond.net), Sublime's built-in tool, can install these syntaxes. If you already have Package Control, skip the rest of this and start on the next section. If you don't, this [install guide](http://sublime.wbond.net/installation) will walk you through all the install options.

### Jekyll Packages

1. Open `Preferences > Package Control`.
2. Type <kbd>Install Package</kbd> and hit <kbd>Return</kbd>.
3. Type <kbd>Jekyll</kbd> and hit <kbd>Return</kbd>.

The Jekyll package includes syntaxes for HTML, JSON, Markdown, and Textile.

### Liquid Packages

1. Open `Preferences > Package Control`.
2. Type <kbd>Install Package</kbd> and hit <kbd>Return</kbd>.
3. Type <kbd>Siteleaf Liquid Syntax</kbd> and hit <kbd>Return</kbd>.

The Liquid package includes syntax for HTML.

---

# Where to Go Next

__A helpful serving of groovy websites that you might find helpful.__

* <a href="http://pages.github.com" target="_blank">GitHub Pages</a>
* <a href="http://jekyllrb.com" target="_blank">Jekyll</a>
* <a href="http://markable.in" target="_blank">Markable.in</a>
* <a href="http://mouapp.com" target="_blank">Mou</a>
* <a href="http://prose.io" target="_blank">Prose.io</a>
* <a href="http://twitter.github.io/recess/" target="_blank">Recess</a>
* <a href="http://yizeng.me/2013/05/10/setup-jekyll-on-windows" target="_blank">Setup Jekyll on Windows</a>
* <a href="http://www.spurapp.com" target="_blank">Spur</a>

---

# License

__Some incomprehensible words from some high-strung people in suits.__

Our code and documentation is licensed under the {{site.github.license}} license</a>. By contributing your code, you agree to license your contribution under the terms of this license.
