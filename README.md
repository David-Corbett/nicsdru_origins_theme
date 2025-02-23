# nicsdru_origins_theme
This repository contains code for a Drupal 8 theme from which NICS sites should be sub-themed from.

## Table of contents

- [Quick start](#quick-start)
- [What's included](#whats-included)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [Using the NPM scripts](#using-the-npm-scripts)
- [Sub-theming](#sub-theming)
- [Documentation](#documentation)

## Quick start
- [Download the latest release](https://github.com/dof-dss/nicsdru_origins_theme/archive/master.zip) or clone the repo: `git clone https://github.com/dof-dss/nicsdru_origins_theme.git`
- `npm install`

## What's included

The theme uses [NPM scripts](https://docs.npmjs.com/misc/scripts) and packages to create tooling to:

* write and compile scss to css
* apply appropriate prefixing for css rules
* write and uglify js
* detect features the user’s browser has to offer (via Modernizr)
* code linting
* optimise and compress images for the web



Within the download you'll find the following directories and files, logically grouping common assets, you'll see something like this:

```
nicsdru_origins_theme/
└── config/
│   ├── install/
│   ├── .sass-lint.yml
│   ├── modernizr-config.json
└── css/
└── docs/
└── js/
└── src/
│   ├── images/
│   ├── js/
│   ├── scss/
│   ├── styleguide/
└── templates/
└── .gitignore
└── composer.json
└── mkdocs.yml
└── nicsdru-origins-theme.breakpoints.yml
└── nicsdru-origins-theme.info.yml
└── nicsdru-origins-theme.layouts.yml
└── nicsdru-origins-theme.libraries.yml
└── nicsdru-origins-theme.theme
└── package.json
└── README.md
└── screenshot.png
```

## Using the NPM scripts
The `package.json` includes the following commands and tasks:

| Task | Description |
| --- | --- |
| `npm run build` | `npm run build` compiles files into their build directories ready for use in a production environment. **Uses [Sass](https://sass-lang.com/), [Autoprefixer][autoprefixer], [Modernizr](https://modernizr.com) and [UglifyJS](https://github.com/mishoo/UglifyJS2).** |
| `npm run watch` | Watches for changes to scss and js files & compiles them for development purposes.|
| `npm run lint`  | Will run all `.scss` and `.js` files through their respective linting tools - [eslint]() & [sass-lint](https://github.com/sasstools/sass-lint) |
| `npm run lint-scss`  | Will run all `.scss` files through [sass-lint](https://github.com/sasstools/sass-lint). The command can also accept a parameter to lint an individual file. To do this `npm run lint-scss -- scssfile:name-of-file` where `name-of-file` is the file you want to lint relative to the package.json for the project. |

Run `npm run` to see all the npm scripts.

## Sub-theming

TODO: add in how to sub-theme from this theme.

## Documentation

TODO: add documentation.

[autoprefixer]: https://github.com/postcss/autoprefixer


