# sotilrac.github.io
Personal site and project portfolio


# Installation

## Git

```
$ jekyll new sotilrac.github.io
$ cd sotilrac.github.io
$ git init
$ git add .
$ git commit -m "Generated by Jekyll"
$ git remote add origin git@github.com:sotilrac/sotilrac.github.io.git
$ git push -u origin master
```
Setup gh-pages branch to host built site
```
$ git checkout --orphan gh-pages
$ git reset .
$ rm -r *
$ rm .gitignore
$ echo 'Coming soon' > index.html
$ git add index.html
$ git commit -m "init"
$ git push -u origin gh-pages
$ git checkout master
$ git clone git@github.com:aymerick/sotilrac/sotilrac.github.io.git -b gh-pages _site
```

Derived [aymerick|from http://www.aymerick.com/2014/07/22/jekyll-github-pages-bower-bootstrap.html]

## Build Environment
```
$ sudo npm install -g bower
$ bower install bootstrap
$ bower init
```

# Serve and Build

Serve locally to http://127.0.0.1:4000/ 
```
jekyll serve
```

Build on changes automatially
```
jekyll build --watch
```