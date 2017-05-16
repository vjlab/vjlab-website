# Vijaykrishna lab research
This is a fork of Trevor Bedfords's website [bedford.io](http://bedford.io).

### Download Site Files & Ruby Bundle Install

Download this repo to your local machine with:

```
git clone https://github.com/vjlab/vjlab-website
```

Install necessary Ruby dependencies using `bundle install`, from within the `vjlab-website` folder:

```
cd path/to/vjlab-website
bundle install
```

### Activate `Projects` Submenu

The `projects` page displays a selection of repositories to the website, such as the github repos of ongoing research projects, repos of code, etc. To include the `projects` submenu, preprocessing scripts are necessary to clone project repos and update Jekyll metadata. This can be done with:

```
ruby _scripts/update-and-preprocess.rb
```

### Start Server and View Site

To view the site: 
```
jekyll build
jekyll serve
```
And navigate to `http://localhost:4000/` on your browser. 

Not working? There have been [whiffs of a known error](https://github.com/jekyll/jekyll/issues/3084) since 2014. If the last step didn't work, try this instead (builds and starts up a server):

```
bundle exec jekyll s
```

Or try installing a slightly earlier version of `gem` (that Jekyll was built with):

```
gem uninstall bundler
sudo gem install bundler -v 1.13.1
```

### References
 - Original [website repo](https://github.com/blab/blotter) by Trevor Bedford
 - Jekyll

## The MIT License (MIT)

Copyright (c) 2013-2015 Trevor Bedford

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
