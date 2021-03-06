# Workshop for this step

Your instructor may have changes to the workshops, as our curriculum
is under continuous improvement.

## Example application

Our example application is available at the following URL:

http://videomanager.angularbootcamp.com

The features in it have been chosen to provide good examples and
context to explain, demonstrate, and workshop Angular features. Your
instructor will work on re-creating (portions of) an application
similar to this one in class.

## Start a new project

Throughout many of the remaining workshops, you will be creating an
Angular application using the Angular CLI. Your instructor may suggest
problem domain and feature ideas.

## StackBlitz users, read this!

While StackBlitz makes it very easy to get started, it also means you
are not working at the command line, so you can't use the Angular CLI
commands as described. Rather, some of the same capabilities are
available by clicking in the StackBlitz interface. Behind the scenes,
StackBlitz is using code from Angular CLI, so it produces
approximately the same results. We will mention where to click the
first few times it comes up.

It is wise to also keep an eye on the CLI instructions, as you are
much more likely to use those in a real Angular project.

Proceed to step 4.

## Developing the workshops on your computer

## Step 0: Node.js

Node.js is a JavaScript runtime environment used by many
Angular-related tools. Please download and install Node.js from [the
Node.js web site](http://nodejs.org/). The Node.js installer also
includes npm.

Angular CLI requires Node.js 10.13 or later. We recommend
**Node.js version 12.16.2 or later "LTS"**.

## Step 1: Install Angular CLI

To create an Angular application from scratch, you will need to use
the Angular CLI, a command-line tool for quickly generating an Angular
project. The Angular CLI tool is available on NPM. To install it,
issue the following command from your OS terminal:

```
npm install -g @angular/cli
```

The above command will add the Angular CLI tool to your computer and
make it accessible from the command line.

## Step 2: Create an Angular Project

Use your terminal to navigate to the desired location for your new
project. Once you are there, type the following command:

```
ng new workshop-app --routing
```

This command will create a new folder for your project and initialize
an Angular application within it.

## Step 3: Start your application

Change directories into the workshop-app folder that was generated by
Angular CLI:

```
cd workshop-app
```

Then start Angular CLI in development mode:

```
npm start
```

Once the terminal reports that "Ready for changes", the
application is ready to load.

Open a browser and navigate to http://localhost:4200/

You should see the resulting application.

## Step 4: (OPTIONAL) Add third-party CSS library

While fully-handcrafted CSS has advantages, an off-the-shelf CSS
framework is very helpful for getting up and running quickly. Typical
choices include:

### Bootstrap

http://getbootstrap.com/

Angular CLI has instructions for easily including the Bootstrap CSS in
your project:

https://github.com/angular/angular-cli/wiki/stories-include-bootstrap

There are also Angular libraries which wrap Bootstrap and provide
behavior as well as appearence, but those are too complex to start with.

### Materialize CSS

At Oasis Digital, we often use Materialize CSS, which provides a look
similar to the Google Material Design guide.

http://materializecss.com/

The CSS can be included in an Angular CLI application by a means
similar to the above instructions.

```
npm install materialize-css
```

(then edit your angular.json file)
```
"styles": [
  "node_modules/materialize-css/dist/css/materialize.css",
  "src/styles.css"
],
```

(On StackBlitz, add materialize by adding
@import url('https://cdnjs.cloudflare.com/ajax/libs/materialize/0.100.2/css/materialize.min.css')
to the styles.css file.)
