# Vijaykrishna lab research
This is a fork of Trevor Bedfords's website [bedford.io](http://bedford.io).

## Build site

To build the website locally, clone the repo with:

```
https://github.com/vjlab/vjlab-website
```

Then install necessary Ruby dependencies by running `bundle install` from within the `lab` directory.  After this, the site can be built with:

```
jekyll build
```

To view the site, run `jekyll serve` and point a browser to `http://localhost:4000/`.  More information on Jekyll can be found [here](http://jekyllrb.com/).

Not working? There have been [whiffs of a known error](https://github.com/jekyll/jekyll/issues/3084) since 2014. If the last step didn't work, try this instead:

```
bundle exec jekyll s
```

## Activate `Projects` Submenu
The `projects` page displays a selection of repositories to the website, such as the github repos of ongoing research projects, repos of code, etc. To include the `projects` submenu, preprocessing scripts are necessary to clone project repos and update Jekyll metadata. This can be accomplished with:

```
ruby _scripts/update-and-preprocess.rb
```

Then use `jekyll build`.

**The MIT License (MIT)**

Copyright (c) 2013-2015 Trevor Bedford

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
