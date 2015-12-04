generator-angular-wakanda
=========================
[![ angular-wakanda ](https://wakanda.github.io/angular-wakanda/images/angular-wakanda.png)](https://wakanda.github.io/angular-wakanda/)

[![MIT Licensed](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](#license)

*Wakanda® is a registered trademark of WAKANDA SAS in France and/or other countries. All other names mentioned may be trademarks or registered trademarks of their respective owners.*

This generator lets you scaffold your AngularJS/Wakanda website.

## Prerequisite

Of course you need node, but you will also need the following modules to get the generator (and its grunt scripts) running :

* bower (client dependencie) `npm install bower -g`
* grunt-cli (grunt command line) `npm install grunt-cli -g`
* yo (yeoman command line) `npm install yo -g`
* karma (test runner - optionnal) `npm install karma -g`

If you get into some troubles for the installation - see [notes](#notes) part.

## Usage

Install `generator-angular-wakanda` :

```
npm install -g generator-angular-wakanda
```

Go to your Wakanda project directory

```
cd MyWakandaSolution/MyWakandaProject
```

Run `yo angular-wakanda`, optionally passing an app name (the app name of your angular app) :

```
yo angular-wakanda [app-name]
```

You will be asked a couple of questions like :

* The name of the folder you want to put all the usual yo angular scaffold
* Whether you want to use Sass/Compass or not
* Whether you want to use Bootstrap or not
* Which angular modules you wish to include

Example of output directory tree :

```
WakandaProjectFolder
├─┬ angularApp
  ├─┬ app
    ├── scripts
    ├── styles
    ├── index.html
  ├── bower.json
  ├── Gruntfile.js
  ├── node_modules
  ├── package.json
  ├── test
├── Gruntfile.js
├── node_modules
├── package.json
├── WebFolder
├── .gitignore
```
In result, you will have two levels of Gruntfile.js :

* The one at the root where you can call tasks like `grunt wakCopy`
* The one in your angularApp folder which contains exactly the same kind of tasks as you would expect from a regular Gruntfile.js made with `yo angular` like `grunt serve`, `grunt build` …

## Angular subgenerators available

In your `angularApp` folder, you can run any of the [official yeoman generator-angular subgenerators](https://github.com/yeoman/generator-angular/blob/master/readme.md#generators).

## Resources

* [angular-wakanda connector](https://github.com/Wakanda/angular-wakanda)
* [Home page](https://wakanda.github.io/angular-wakanda/)

## Contributors

* If you don't have yo : `npm install -g yo`
* Clone the repo
* `npm install`
* If you already work with the genrator-angular-wakanda, you'll need to uninstall it : `npm uninstall generator-angular-wakanda -g`
* In the repo directory : `npm link` (will let you use your local version of the generator)

## Notes

* If you have troubles installing modules, sometimes a `npm cache clean` can do the trick
* If you are behind a proxy that doesn't allow git:// urls (problems for the bower install), take a look at [this link](https://coderwall.com/p/sitezg)

## License

The MIT License (MIT)

Copyright (C) 2015 WAKANDA SAS

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
