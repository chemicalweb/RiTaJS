[![Build Status](https://travis-ci.org/dhowe/RiTaJS.svg?branch=master)](https://travis-ci.org/dhowe/RiTaJS)

## RiTa: a generative language toolkit for JavaScript

<a href="http://rednoise.org/rita/js"><img height=120 src="http://rednoise.org/rita/img/RiTa-logo3.png"/></a>

#### [The RiTa website](http://rednoise.org/rita)

#### RiTa is designed to be an easy-to-use toolkit for experiments in natural language and generative
literature. It is implemented in Java and JavaScript (with a unified API for both) and optionally
integrates with Processing(JS), Android, and Node, and is available via Npm and Bower. 
It is free/libre and open-source according to the GPL license (http://www.gnu.org/licenses/gpl.txt).

About the project
--------
* Original Author:   Daniel C. Howe (http://rednoise.org/~dhowe)
* License: 			 GPL (see included LICENSE file for full license)
* Maintainers:       See included AUTHORS file for contributor list
* Web Site:          http://rednoise.org/rita
* Github Repo:       https://github.com/dhowe/RiTaJS
* Bug Tracker:       https://github.com/dhowe/RiTa/issues
* Documentation:    https://rednoise.org/rita/reference


In the browser with [Bower](http://bower.io/)
--------

First, to install do: 

```bash
$ bower install rita
```

Now, create a file on your desktop called 'first.html', add the following lines, save and drag it into a browser:

```html
<html>
  <script src="./bower_components/rita/dist/rita.js"></script>
  <script>
    window.onload = function() {
      $('#content').text(RiTa.tokenize("The elephant took a bite!"));
    };
  </script>
  <div id="content" width=200 height=200></div>
<html>
```

#### Can I contribute?
--------
Please! We are looking for more coders to help out... Just press *Fork* at the top of this github page and get started, or follow the instructions below... 

#### Development Setup
--------
1. Download and install [npm](https://www.npmjs.org/) The easiest way to do this is to just install [node](http://nodejs.org/). 
2. [Fork and clone](https://help.github.com/articles/fork-a-repo) this library. 

  a. First, login to github and fork the project

  b. Then, from a terminal/shell: 
  
    ```bash
    $ git clone https://github.com/dhowe/RiTaJS.git
    ```
3. Now navigate into the project folder and install dependencies via npm. 

  ```bash
  $ cd RiTaJS && npm install
  ```
4. To create the library from src, use gulp.

  ```bash
  $ ./node_modules/.bin/gulp build
  ```
5. Run non-graphical tests in node with gulp.

  ```bash
  $ ./node_modules/.bin/gulp test.node
  ```
6. Run all tests (in phantomJS) with gulp.

  ```bash
  $ ./node_modules/.bin/gulp test
  ```
7. Work on an existing [issue](https://github.com/dhowe/RiTa/issues?q=is%3Aopen+is%3Aissue+label%3ARiTaJS), then [submit a pull request...](https://help.github.com/articles/creating-a-pull-request)
