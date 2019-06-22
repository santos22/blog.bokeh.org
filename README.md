# Bokeh Project Blog

This is the GitHub repository for the Bokeh Project Blog, blog.bokeg.org. The blog is used for making release announcements, and publishing case studies, howtos, or other project news. The repository for the source code of the Bokeh itself can be found at github.com/bokeh/bokeh.

Full docs for setting up a GitHub Pages Jekyll blog [can be found here](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll).

# Building Locally

## Using Docker

After installing [`docker`](http://docker.com/), run `make serve` to build and run the website within the a container built from the [`jekyll/jekyll` image](https://hub.docker.com/r/jekyll/jekyll/) that contains all the necessary prerequisites. The site will be available at [http://localhost:4000](http://localhost:4000). Modifying source files will cause the website to rebuild in real time (refresh the browser page to see changes).

## Manually

To build manually, you will need to have Ruby >= 2.1 installed on your system. If necessary, run 

    gem install bundler
    
The first time you build locally you will need to install mnecessary dependcies by running 

    bundle install
    
in the top level directory of this repository. Then run

    bundle exec jekyll serve --future
    
to serve the site at [http://localhost:4000](http://localhost:4000) While this remains running, you can edit the source files and Jekyll will automatically rebuild the site (refresh the browser page to see changes).
