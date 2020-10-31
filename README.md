<h1 align="center">StartQuick <span><small>v0.1.0</small></span></h1>
<h3 align="center">A Dead Simple Project Skeleton.</h3>

## Introduction
StartQuick is a dead simple project skeleton that can be used to quickly and easily get you up and running for rapid development with your next Bootstrap based website or web app.

This is accomplished by automating your workflow using [Node.js][nodejs] with [Gulp][gulpjs]. This project skeleton utilizes [BrowserSync][BrowserSync] for synchronized browser testing and automatic page refreshes upon saving your changes. It also makes testing on multiple devices within your personal LAN a breeze by automatically setting up both and internal and external LAN address.

It cuts out repetitive manual tasks such as compiling [SASS/SCSS][sass] into CSS by using [gulp-sass][gulp-sass], automatically minimizes your CSS and JavaScript files using [gulp-minify][gulp-minify], and creates sourcemaps (`.map` files) for your minified CSS and JavaScript files by using [gulp-sourcemaps][gulp-sourcemaps].

Last but not least, it renames your minified files with `.min.css` and `.min.js` file extensions using [gulp-rename][gulp-rename] and even uses [Autoprefixer][autoprefixer] to parse CSS and add vendor prefixes to CSS rules using values from [Can I Use][caniuse] (as [recommended][aprecommend] by Google and used in Twitter and Alibaba.).

## Why I Made This...
I built this helpful little kit so that way I can have a starting point in which to quickly and easily get the ball rolling with class projects as I am currently attending the [UCONN Coding Boot Camp][ucbc]'s _**Full Stack Developer**_ program (10/2020 to 04/2021).

## A Work In Progress
_**This is by no means a finished product.**_ This is just a dead simple skeleton project that I will be using and developing along the way to aid in rapid prototyping and development of my class projects.

## Features
**Frontend libraries**
 - Bootstrap v4.5.3
 - Jquery v3.5.1
 - PopperJS v1.16.1

**Project Dependencies**
 - del
 - gulp 4
 - gulp-sass
 - gulp-sourcemaps
 - gulp-autoprefixer
 - gulp-rename
 - gulp-minify
 - browser-sync
 - bootstrap
 - jquery
 - popperjs

## Installation

### Requirements

You will need Node.js and the Node Package Manager (npm) for use with this project skeleton.
 - Local Web Server (Apache 2 or Nginx) installed.
 - NodeJS >= v12.19.x LTS
 - NPM >= v6.14.x

### Install

Download the zip or clone this project.

```
git clone https://github.com/davidsaulrodriguez/startquick.git yourProjectName
cd yourProjectName/
```

Now install the required dependencies with npm.

`npm install`

## Usage

### Development

To start the live server and automatically open http://localhost:3000 on your default web browser run:

```gulp start```

The live server should have Live-Reloading automatically enabled via BrowserSync. This means that after you're done modifying any source files and saving your changes, the project will be recompiled and the browser will refresh the page.

_**Note:** When running the live server, if you modify the `gulpfile.js` and/or `package.json` files, you will have to restart the server for those changes to take effect. - This will be addressed in a later release._

### Deployment

Once you're happy with your website you can compile all your files into a `prod/` folder located at the root of the project with this command:

```gulp compile```

You can then transfer the contents of the `prod/` folder onto your production server in whatever way works for you and your workflow.

For example: `scp -r prod/* root@bsdadm.com:/usr/local/www/apache24/data`

## Gulp Tasks

StartQuick comes with very basic pre-built gulp tasks that will help aid in the development of your project and producing files for production ready deployment. You can view the available tasks in the [COMMANDS.md][commands] file.

## Configuration

Once everything is working as expected, check out the [CONFIGURATION.md][configuration] file to see how the project is structured and where to place your source files.

## Contributing

Contributions are more than welcome! If you improve on this project skeleton, please feel free to share it by submitting a Pull Request.

Before contributing, be sure to check out the [CONTRIBUTING.md][contributing] file.

## Bugs and Issues
Found a bug? Having an issue with this project skeleton? Open a new issue [here][issues].

## License
This project and all of its source code is released and permissively licensed under the [BSD 2 Clause](LICENSE.md) license.

[gulp-sass]: https://www.npmjs.com/package/gulp-sass
[gulp-rename]: https://www.npmjs.com/package/gulp-rename
[gulp-minify]: https://www.npmjs.com/package/gulp-minify
[gulp-sourcemaps]: https://www.npmjs.com/package/gulp-sourcemaps
[BrowserSync]: https://www.browsersync.io/
[nodejs]: https://nodejs.com
[gulpjs]: https://gulpjs.com/
[caniuse]: https://caniuse.com/
[autoprefixer]: https://github.com/postcss/autoprefixer
[aprecommend]: https://developers.google.com/web/tools/setup/setup-buildtools#dont_trip_up_with_vendor_prefixes
[ucbc]: https://bootcamp.uconn.edu/
[sass]: https://sass-lang.com/
[commands]: docs/COMMANDS.md
[configuration]: docs/CONFIGURATION.md
[contributing]: docs/CONTRIBUTING.md
[issues]: https://github.com/davidsaulrodriguez/startquick/issues/new/choose
