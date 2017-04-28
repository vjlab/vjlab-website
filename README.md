# Vijaykrishna lab research
This is a fork of Trevor Bedfords's website [bedford.io](http://bedford.io).

## Build site

To build the website locally, clone the repo with:

```
git clone https://github.com/vjlab/vjlab-website.git
```

CD into the `vjlab-website` directory, and install the necessary Ruby dependencies:

```
bundle install
```

After this, the site can be built with:

```
jekyll build
```

Not working? There have been [whiffs of a known error](https://github.com/jekyll/jekyll/issues/3084) since 2014 about some kind of dependency not updating correctly. In that case, instead try:

```
bundle exec jekyll s
```
to start up the local web server.

To view the site, run `jekyll serve` and point a browser to `http://localhost:4000/`.  More information on Jekyll can be found [here](http://jekyllrb.com/).

To include projects, preprocessing scripts are necessary to clone project repos and update Jekyll metadata. This can be accomplished with:

```
ruby _scripts/update-and-preprocess.rb
```

Then `jekyll build` works as normal.

**The MIT License (MIT)**

Copyright (c) 2013-2015 Trevor Bedford

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
