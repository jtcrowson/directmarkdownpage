# Directmarkdownpage

Branching off Sander's implementation of ContentFile + Empty Path.  Issue now is that when navigating from '/' to '/bar/content' via the links on the app component, the component changes, but the scully-content doesn't refresh with the new content.  The issue resolves only one we navigate to a third link, like Foo.

Reproduction steps:

1. Navigate to localhost:1668
- Notice that the correct component is showing, denoted by the "home works!" text, and the correct bar.md markdown file content is showing.
2. Navigate to localhost:1668/bar/content by tapping on the link titled "bar".
- Notice that the correct component is showing, denoted by the "bar works!" text, but incorrectly, the bar.md markdown file content is still being shown, instead of the correct bar/content.md markdown file content.

This also happens in the inverse scenario, when first navigating to localhost:1668/bar/content, then to the empty path by tapping the 'home' link.

The issue is only resolved once navigating to the foo component.

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.1.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
