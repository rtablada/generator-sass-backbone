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
broccoli serve
```

The `Brocfile.js` injects live reload into HTML files in the `public` directory.
To take advantage of this, you will have to use `broccoli-lr` to notify the page of changes.

To install the `broccoli-lr` command run:

```bash
npm install -g broccoli-lr
```

Then instead of `broccoli serve` run the following command to run the development server:

```bash
broccoli-lr server
```

## Building the Project

To build the project into a final production build, run:

```bash
broccoli build dist
```

This will build the project into a `dist` directory that can be uploaded to services such as Firebase, Surge, or AWS.
