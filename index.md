---
layout: page
---

# Introduction

{{site.github.title}} is a one-page boilerplate for publishing technical content on GitHub. It provides the facilities to write exclusively in [Markdown](http://en.m.wikipedia.org/wiki/Markdown) and spin-up [Jekyll](http://jekyllrb.com)-powered websites.

Browse the sections below and see just how simple it is to roll your own GitHub site for free without using fancy code.

---

# Features and Delighters

{{site.github.title}} is chock-full of nifty doodads and neat delighters, including:

* Responsive and mobile-friendly design
* Fast load times
* Centralized setup from a single configuration file
* Pretty URLs
* API calls to fetch data from your GitHub repo
* Built-in table of contents that updates automatically
* [Repo metadata](http://help.github.com/articles/repository-metadata-on-github-pages) for GitHub Pages

## Core Environment

The core for {{site.github.title}} includes:

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

Below are recommended browsers and platforms for the best usability and performance. Starting from best to worst, we suggest you get the latest version of:

* Chrome (~100%)
* Safari (~75%)
* Firefox (~50%)
* Opera (~50%)
* Internet Explorer (~25%)

Here's a comparison of each browser on different OS platforms.

| Platform    | Chrome | Firefox | Internet Explorer  | Opera | Safari |
| ----------- |:------:|:-------:|:------------------:|:-----:|:------:|
| Android     | Yes    | No      | --                 | No    | --     |
| iOS         | Yes    | --      | --                 | No    | Yes    |
| Mac OS X    | Yes    | Yes     | --                 | Yes   | Yes    |
| Windows     | Yes    | Yes     | Yes                | Yes   | No     |

> Apple no longer provides updates for Windows-native Safari browsers. Due to major lapses in critical updates, we do not recommend using Safari on Windows.

## Legacy Browsers

Support is limited to whatever legacy browsers can handle. You can try using [Modernizr](http://modernizr.com) to circumvent compatibility issues, but it's not perfect.

---

# Prerequisites

{{site.github.title}} requires the minimum version of __Ruby__ below. It also requires __Python__ to run __Pygments__, but only if you’re planning to use code highlights. Otherwise, you won't need it.

* Ruby 1.9.3
* Python 2.7
* Pygments 1.6

## Ruby

[Click here](http://www.ruby-lang.org/en/installation) to download and install Ruby. If you have Ruby, but aren’t sure which version, run `ruby -v`.

## Python

[Click here](https://www.python.org/download/releases/2.7) to download and install Python. If you have Python, but aren’t sure which version, run `python --version`.

## Pygments

[Click here](http://pygments.org/download) to download and install Pygments. If you have Pygments, but aren’t sure which version, run `pygmentize -V`.

---

# Download and Clone

The following sections walk you through downloading or cloning {{site.github.title}} from GitHub.

## Downloading {{site.github.title}}

There are a number of ways to download {{site.github.title}}. Scroll through the options below and pick one that works best for you.

### Tarball Download

[Click here]({{site.github.repository_url}}/tarball/master) or run the command below.

~~~bash
$ curl -OL {{site.github.repository_url}}/tarball/master
~~~

### ZIP Download

[Click here]({{site.github.repository_url}}/zipball/master) or run the command below.

~~~bash
$ curl -OL {{site.github.repository_url}}/zipball/master
~~~

## Cloning {{site.github.title}}

There are also a few ways to clone {{site.github.title}}. Scroll through the options below and pick one that works best for you.

### Clone over HTTPS

Run the command below to clone over HTTPS.

~~~bash
$ git clone {{site.github.repository_url}}.git
~~~

### Clone over SSH

Run the command below to clone over SSH.

~~~bash
$ git clone git@github.com:{{site.github.owner_name}}/{{site.github.repository_name}}.git
~~~

---

# Installation

The following is a "how to" for installing {{site.github.title}} and adding runtime dependencies.

1. Go into the root directory for {{site.github.title}}.
2. Run `gem install bundler` to install Bundler.
3. Run `bundle install` to load the runtime dependencies.

```bash
$ cd {{site.github.project_title}}
$ gem install bundler
$ bundle install
```

---

# Configuration

The `_config.yml` is a [YAML](http://en.m.wikipedia.org/wiki/YAML) file for storing and propagating nearly all of the site's configuration. Anything not handled by it gets handled behind the scenes by [metadata](http://help.github.com/articles/repository-metadata-on-github-pages). This means you can configure your entire site using just a single file.

## Project

1. Open "_config.yml" using any text editor.
2. Find "Project".
3. Fill in each field with details about your project.

~~~yaml
# ==============================
# Project
# ==============================

github:
    title:      Ferris
    tagline:    A one-page boilerplate for publishing content on GitHub
    owner:      "Bueller Company, LLC"
    license:    MIT
~~~

> Use spaces to separate content. Do not use tabs.

## Social

1. Scroll down to the second group of setting labeled "Social".
2. Fill in each field with details about your social network.

~~~yaml
# ==============================
# Social
# ==============================

twitter:
    handle:     BuellerLabs
    hashtags:   "css,boilerplate,github-pages"
    text:       "Try Ferris, a one-page boilerplate for posting technical content on GitHub."
keywords:       "boilerplate,css,framework,github,github pages,html5,jekyll,liquid,markdown,one-page,redcarpet"
~~~

> Wrap words in quotes wherever commas are used.

## Options

1. Scroll down to the third group called "Options".
2. Type "Y" to enable or "N" to disabled any of the options.

~~~yaml
# ==============================
# Options
# ==============================

index:
    enabled:    Y
scrolling:
    enabled:    Y
version:
    enabled:    N
~~~

Below is a brief overview of each option.

| Option     | Default | Description   |
| ---------- |:-------:| ------------- |
| Index      | Y       | Captures all H1 headers and drops them into a modal |
| Scrolling  | Y       | Enables smooth scrolling animation |
| Version    | N       | Fetches the last pegged release from GitHub and shows it under "Get Started" |

*For these options, use Y or N. Anything else will disable the option.*

---

# Deployment

Learn how to make Jekyll transform raw text into a complete, ready-to-publish static website.

## Local Deployment

Run the following command to preview a local instance of your site.

```bash
$ jekyll serve
```

Once Jekyll has started, fire up a browser and type in "localhost:4000" for the web address. This will show the site Jekyll just generated.

### Watch Jekyll

If you want to monitor changes and apply updates without having to restart Jekyll, add the `--watch` option to the command.

```bash
$ jekyll serve --watch
```

### Stopping Jekyll

Serve mode lasts forever. It won't timeout after a period of non-usage. Press "CTRL+C" to stop the service.

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

The following is a simple introduction to the directory structure and contents for {{site.github.title}}.

## Pre-Install

Below is the basic spread for {{site.github.title}} (not including `site` for Jekyll).

```
├─ _includes
├─ _layouts
└─ stylesheets

3 directories
```

> Folders beginning with an underscore tell Jekyll to use the content within them to generate your site. They're not exposed after the site is created, though.

## Post-Install

A working environment will have one more directory: `site` (Jekyll).

```
├─ _includes
├─ _layouts
├─ _site
└─ stylesheets

4 directories
```

## Directory

Here's an overview of what each directory does or contains.

| Directory     | Overview  |
| ------------- | --------- |
| `_includes`   | Semantic HTML elements and reusable content |
| `_layouts`    | Reusable templates for specific uses |
| `_site`       | Where Jekyll places generated sites after it's transformed |
| `stylesheets` | Static CSS stylesheets in `.css` format |

---

# Useful Resources

Below is nonspecific information written during development that might be useful to some, but not everyone.

## Metadata

We harness several metadata tags using GitHub's [metadata](http://help.github.com/articles/repository-metadata-on-github-pages) feature, albeit not all of them for a number of reasons.

Below is a list of metadata tags we use.

* {%raw%}{{ site.github.owner_name }}{%endraw%}
* {%raw%}{{ site.github.owner_url }}{%endraw%}
* {%raw%}{{ site.github.project_title }}{%endraw%}
* {%raw%}{{ site.github.repository_url }}{%endraw%}
* {%raw%}{{ site.github.url }}{%endraw%}

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

Sublime Text users can configure these settings manually by opening "Preferences > Settings - User", inserting the lines below, and saving your settings.

```json
{
    "translate_tabs_to_spaces": true,
    "tab_size": 4,
    "ensure_newline_at_eof_on_save": false,
    "default_encoding": "UTF-8",
    "default_line_ending": "lf",
    "trim_trailing_white_space_on_save": true
}
```

## Sublime Packages

We use Sublime exclusively. One of its few drawbacks, though, is it does not include every syntax highlight. To get certain highlights, you have to install them by hand. Use the instructions below to perform the install processes for __Jekyll__ and __Liquid__.

[Package Control](http://sublime.wbond.net), Sublime's built-in tool, can install these syntaxes. If you already have Package Control, skip the rest of this and start on the next section. If you don't, this [install guide](http://sublime.wbond.net/installation) will walk you through all the install options.

### Jekyll Packages

1. Open "Preferences > Package Control".
2. Type "Install Package" and hit "Return".
3. Type "Jekyll" and hit "Return".

The Jekyll package includes syntaxes for HTML, JSON, Markdown, and Textile.

### Liquid Packages

1. Open "Preferences > Package Control".
2. Type "Install Package" and hit "Return".
3. Type "Siteleaf Liquid Syntax" and hit "Return".

The Liquid package includes syntax for HTML.

---

# Where to Go Next

Here's a helpful serving of groovy websites that you might find helpful.

* <a href="http://pages.github.com" target="_blank">GitHub Pages</a>
* <a href="http://jekyllrb.com" target="_blank">Jekyll</a>
* <a href="http://markable.in" target="_blank">Markable.in</a>
* <a href="http://mouapp.com" target="_blank">Mou</a>
* <a href="http://prose.io" target="_blank">Prose.io</a>
* <a href="http://twitter.github.io/recess/" target="_blank">Recess</a>
* <a href="http://yizeng.me/2013/05/10/setup-jekyll-on-windows" target="_blank">Setup Jekyll on Windows</a>

---

# License

Our code and documentation is licensed under the {{site.github.license}} license</a>.
