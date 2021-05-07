---
title: Home
layout: default
---
# Dartboard

A lightweight Jekyll theme created for CS234 (Spring 2021), with a personal financial blog in mind. This theme uses the default jekyll theme [Minima](https://github.com/jekyll/minima) as its framework.

## Demo

Check out the three sample posts on the "All Posts" page for the styling of texts, tables, and multimedia in this theme.

## Installation

1. Make sure you have the up-to-date version of Ruby and RubyGems with the commands `ruby -v` and `gem -v`
2. Install jekyll and bundler, the basic gems we need for our environemnt, with the command `gem install jekyll bundler`
3. Clone [the repository from Github](https://github.com/JasonBourbaki/final-project-theme)
4. In the project folder, edit `Gemfile` to include the gems you intend to use
> Warning: Do not replace the line `gem "webrick"`; as of jekyll 5.4.0, the site would not serve without adding this depricated gem
5. Run `bundle install` in the root of project to install the required gems
6. Run `bundle exec jekyll serve --watch` to build and serve your site
7. Open your browser at `http://localhost:4000` to see it!

## Development

Add posts, pages, documents, data, etc. to test your theme's contents. 

If you want to see the real-time effects of your modifications, add `--livereload` when serving the site.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.

To add a custom directory to your theme-gem, please edit the regexp in `final-project-theme.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
