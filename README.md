# SASS Broccoli Yeoman Generator

This Yeoman generator will create a simple Broccoli project that comes setup for web development with SASS.
It also will install [Yoga Sass](http://rtablada.github.io/yoga-sass), [Font Awesome](http://fontawesome.io), and [Normalize CSS](https://necolas.github.io/normalize.css/).

## Installing the Generator

```bash
npm install -g broccoli-cli yo generator-sass-broccoli
```

## Creating Projects

To create a project with this generator run:

```bash
yo sass-broccoli
```

This will ask you for your project name, and a few details to get up and started.

## Running the Development Server

Once the project has been created, move into the directory and then run:

```bash
npm run serve
```

The `Brocfile.js` injects live reload into HTML files in the `public` directory.
This command is backed by `broccoli-lr` which will fire a reload whenever Broccoli rebuilds any trees.

## Building the Project

To build the project into a final production build, run:

```bash
npm run build
```

This will build the project into a `dist` directory that can be uploaded to services such as Firebase, Surge, or AWS.
