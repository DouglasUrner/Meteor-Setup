# Meteor-Setup:

Notes on setting up a Meteor development environment.

## Install [Meteor](http://meteor.com)

```
curl https://install.meteor.com | /bin/sh
```

This command installs Meteor for you. The default location is ~/.meteor.

## Adding Packages

In general the process for adding Meteor packages is:

1. Find the name of the package.
  - If you already found a package name (in the format username:package), great!
  - If not, you can search for packages at atmospherejs.com
  - You can also search for packages using `meteor search foo`
2. `meteor install username:packagename`

## Development Tools

### Debugging

### Testing Tools

#### [Velocity](https://github.com/meteor-velocity/velocity)

Velocity is a "meta framework" for testing in Meteor, it is the first thing to
install, but by itself it doesn't do anything useful.

To add Velocity add one of the testing frameworks below. You don't
need to (can't) add Velocity directly.

#### Testing Frameworks

##### [Chai]()

##### [Jasmine]()

Jasmine is a "behavior-driven development framework for testing JavaScript code."

This package supports writing
[Jasmine 2.0](http://jasmine.github.io/2.0/introduction.html)
client and server tests in Meteor.
Client tests run in a browser with the app context.
Server tests run in a mocked server environment.

The Jasmine source on GitHub is [here](https://github.com/pivotal/jasmine).

```
meteor add sanjo:jasmine
```

##### [Mocha]()

```
meteor add mike:mocha
```

### [Nightwatch]()

```
meteor add clinical:nightwatch
```

### Testing Reporters

#### [HTML Reporter]()

HTML Reporter adds a dot in the corner (upper right by default) that
shows the status of tests on the page. Clicking on the dot takes you
to a page of test details.

```
meteor add velocity:html-reporter
```
