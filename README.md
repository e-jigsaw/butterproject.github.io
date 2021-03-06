Butter Project Website
======================

### Branches
There are 2 Branches of this Repo [Source](https://github.com/butterproject/butterproject.github.io/tree/source) and [Master](https://github.com/butterproject/butterproject.github.io/tree/master)
The Reason behind this is so that we can fully develop the site and make changes and test these changes via the source branch and find errors before the site is made live via the master branch

`Please only submit patches to the source branch`

### Setup for production
Setting up the website for production is easy
  1. Run `npm install` in the root directory to pull in the build dependencies
  2. Run `grunt dist` to compile and build the site
  3. Setup a webserver to serve the `compiled` folder
  4. Enjoy!

### Setup for developers
Setting up the website for development is just as easy
  1. Run `npm install` in the root directory
  2. Run `grunt`
  3. Run `grunt develop` 
  4. Visit [http://localhost:8080/](http://localhost:8080/) 
  5. Edit any file and refresh the page!
  6. Enjoy!

### Updating translations
Updating the translations from Transifex is easy too, of course
  1. Make sure you have the [Transifex command-line client](https://github.com/transifex/transifex-client) installed
  2. Run `tx pull -a` in the root directory
  3. Run `grunt copy:locales` to update the `locales` directory in the `compiled` folder
