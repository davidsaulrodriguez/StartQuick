# Configuration

When it comes to the configuration of this skeleton project, I tried my best to keep it as simple as possible.

### src
The **src** folder is the container for all of your source files. All of your
```.html``` files should be placed into this directory.

### src/scss
This is the folder that you should place all of your ```.sass``` and ```.scss``` files into.

### src/js
This is the folder that you should place all of your ```.js``` files into

### src/imgs
And, this is the folder that you should place all of your image files into

## After compilation...
Once compiled you will see a folder in the root directory of the project named `prod/`. In the root of the 'prod' folder, it will contain all of your `.html` files. You should also see another folder called `dist/` which contains all of your assets.

```
prod/
├── dist
│   ├── css
│   │   ├── bootstrap.min.css
│   │   ├── main.min.css
│   │   └── sourcemaps
│   │       ├── bootstrap.min.css.map
│   │       └── main.min.css.map
│   ├── imgs
│   │   └── index.html
│   └── js
│       ├── bootstrap.min.js
│       ├── jquery.min.js
│       ├── main.min.js
│       ├── popper.min.js
│       └── sourcemaps
│           ├── bootstrap.min.js.map
│           ├── jquery.min.js.map
│           ├── main.min.js.map
│           └── popper.min.js.map
└── index.html

6 directories, 14 files
```

<p style="text-align:center">Example of `prod/` folder contents that can be used for production ready deployment.</p>

***NOTE: Make sure that when you link to your CSS and JS files, you are linking to the `dist/` directory, since this is where the assets are placed by default.***

_** For example:**_
```html
<!-- Linking to main.min.css-->
<link rel="stylesheet" href="/dist/css/main.min.css" />
<!-- Linking to main.min.js-->
<script src="/dist/js/main.min.js" charset="utf-8"></script>
```
---

## Customizing The Configuration

You are welcome to customize this configuration yourself, to suit your exact needs or the needs of your project.

Changing the configuration around is as easy as altering the `gulpfile.js` file located in the root directory of this project.
