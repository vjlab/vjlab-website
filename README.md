# Vijaykrishna lab research
This is a fork of Trevor Bedfords's website [bedford.io](http://bedford.io).

## Build site

To build the website locally, clone the repo:

```
https://github.com/vjlab/vjlab-website
```

Then install necessary Ruby dependencies by running `bundle install` from within the `vjlab` directory.  After this, the site can be built with:

```
jekyll build
```

To view the site, run `bundle exec jekyll serve` and point a browser to `http://localhost:4000/`.  

More information on Jekyll can be found [here](http://jekyllrb.com/).

## Activate `Projects` Submenu
The `projects` page displays a selection of repositories to the website, such as the github repos of ongoing research projects, repos of code, etc. To include the `projects` submenu, preprocessing scripts are necessary to clone project repos and update Jekyll metadata. This can be accomplished with:

```
ruby _scripts/update-and-preprocess.rb
```

Then use `jekyll build` or `bundle exec jekyll serve`.
