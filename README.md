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


## Contributing

Anyone is welcome to submit an issue or request. All we ask is that you glance through our [contributing guidelines](CONTRIBUTING.md) first.


## License

Our code and documentation is licensed under the MIT license. By contributing your code, you agree to license your contribution under the terms of this license.
