# Dartboard

A lightweight Jekyll theme created for Fisher College Spring 2021 Frontend Web Design course, with a personal financial blog in mind.

## Progress Tracking

### Week One: March 22-26
- Set up development environment
  - Install latest version of Ruby on the machine (which runs Manjaro, an Arch-based Linux distribution) by following [the instructions on Arch Linux Wiki](https://wiki.archlinux.org/index.php/ruby)
  - Resolve the "missing gem path" error
  - Install essential gems
  - Install jekyll and bundler
- Initiate a blank theme by following [a tutorial](https://www.siteleaf.com/blog/making-your-first-jekyll-theme-part-2/)
  - Write basic gemspec
  - Create the sample page index.html in root
  - Build and serve the site to make sure the sample page be properly deployed
  - Create the Github repo and push local files
- Review the basics of Jekyll site structure
- Edit the heading to resolve Favicon error

### Week Two: March 29-April 2
- Study Jekyll site structure
- Implement an outline of a Jekyll theme:
    - Create _config.yml
    - Create outlines for head, header, and footer
    - Modify default.html to include the relevant components
    - Create SCSS masterfile
    - Create 404 page
- Make a list of functionalities
    - About page
    - Post preview on the front page
    - Google Analytics
    - Social Media links
    - View posts by tag
    - Disqus comments
    - Optional: Python stock API compatibility
    
### Week Three: April 5-9
- Refine head.html
- Create google analytics plugin
- Restructure the header by splitting the menu and the social media links into external sheets
    - Create post-menu with About, Search, and an iterative list of pages
    - Create social-menu with an expanded list of social media links
    - Wrap each section of the header in div classes, with sudo-coded styling
- Modify the config to add google analytics, scroll toggle, and more social media options
- Study Jekyll scss structure
- Implement an outline of Jekyll stylesheets
    - Create stylesheets for each functionality, separated by category
    - Edit main.scss to import the newly created stylesheets
    - Find font, color, and icon set for the theme

### Week Four: April 12-16
- Scrap search and disqus comments functionality, as Javascript is out of the scope of this course and disqus cannot function offline (which is where this site would be viewed)
- Simplify scss structure
- Containerize the footer into columns
- Stylize the footer
  - Fix the spacing between footer elements

### Week Five: April 19-23
- Import ionicons and create stylesheet for icons
- Add icons to each social media category supported by the theme
- Stylize the header
  - Vertically center social icons within the header
  - Add Website title to the header; fix spacing between title and social links
- Add global colors and fonts to the color.scss
- Create the default styles for html elements in the form of _base.scss
- Add a sample pure-text post to test out global styles

### Week Six: April 26-30
#### **Emergency: due to a recent Archlinux update, the original theme in the he-fp-theme repo cannot be served on my machine. I spent four hours trying to fix it, the only solution seems to be to import the default Jekyll theme Minima and merge my previous work with it.**
- Resolve compatibility issues between existing code and Minima
- Replace overlapping html and css with my own work
- Implement drop-down menu within the header
- Create sample posts for multimedia

### Week Seven: May 3-6
- Final debug
- Write up a simple installation guide based on jekyll's official documentation
- Add the final sample post, with datatables from ArcelorMittal's May 6th earnings to demonstrate html tables under this theme
- Upload project to Github

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
