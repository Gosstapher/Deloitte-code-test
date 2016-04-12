## Prerequisites

[Node.js](http://nodejs.org/) must be installed.
[NPM](https://www.npmjs.com/) must be updated to 3.8.6.

## Installation

```shell
# Clone the repository
> git clone https://github.com/Gosstapher/Deloitte-code-test.git

# Install dependencies
> cd atm-case-study
> npm install
```
* Running `npm install` in the app's root directory will install everything you need for development.

## Development Server

* `npm start` will run the app's development server at [http://localhost:3000](http://localhost:3000) with hot module reloading.

## Running Tests

* `npm run test-utils` will run the unit tests for the Utils module.
* `npm run test-utils:watch` will run the unit tests for the Utils module on every change.


## Building

* `npm run build` creates a production build by default.

   To create a development build, set the `NODE_ENV` environment variable to `development` while running this command.

* `npm run clean` will delete built resources.

## Project structure

Here you can see the structure for this repo:

```
|-- atm-case-study
    |-- assets
        |-- balance.png
        |-- logo.png
        |-- withdraw.png
    |-- .eslintignore
    |-- .eslintrc
    |-- .gitignore
    |-- README.md
    |-- nwb.config.js
    |-- package.json
    |-- public
    |   |-- app.css
    |   |-- index.html
    |   |-- vendor.css
    |-- src
    |   |-- index.js
    |   |-- components
    |   |   |-- atm.js
    |   |   |-- balance.js
    |   |   |-- main.js
    |   |   |-- navigation.js
    |   |   |-- withdraw.js
    |   |-- router
    |   |   |-- AppRouter.js
    |   |-- utils
    |       |-- utils.js
    |-- test-helpers
    |   |-- mockState.js
    |-- test-utils
    |   |-- mocha.opts
    |   |-- utilsSpec.js
```

**Under the hood, this app is using [`nwb`](https://github.com/insin/nwb). A npm package that helps developers to built and setup Javascript projects. Some of the available scripts mentioned above are mapped to `nwb` commands**.

**For more information see the `package.json` file or run the `nwb` command on your terminal**
------------------------------------------------------------------------------------------------------

    
    This was the first time I have seen ECMAScript 6, I have learned JavaScript in the ECMAScript 5 environment. My unfamiliarity with the syntax and new features made my approach to this code test different than if it was a technology I had a stronger background with.
    The NWB framework was also brand new to me, as were some of the plugins such as Skin-Deep.

    I initially spent time following the React flow, attempting to understand how the app was working, while at the same time looking into the new syntax when it was unfamiliar. Learning the new methods of declaring constants, variables and assigning functions using arrows I feel was time well spent.

    Looking at the checklist, I approached it as TDD. I felt the user stories would be completed by first addressing the tests. Having spent time looking over the app allowed me to correct many of the mistakes in the early tests fairly quickly.

    Implementing “Utils.calculateCountNotes” proved a fun challenge. Writing code to pass tests is always preferable. The initial working answer was twice the length and had redundant if statements. The code is refactored to be a simple and readable as I can in the time frame. Given more time I would like to try a slightly different approach using forEach on an Array of the notes. 

    Refactoring “Utils.displayWithdrawnCount” to make it have a more human readable out put was relatively simple. Using picture assets could improve this further and within my abilities but untenable for me within the time constraints. 

    Implementing “Utils.areAnyNotesLeft” was tricky and I feel I was ultimately unsuccessful. The instructions for what this function should do was difficult to ascertain, the semantic name seemed at odds to the instructions given on the hard copy test. The commented instructions in the code gave another possibly for functionality. The fact that this function was supposed to also set a validationObject in motion to return a certain error message did not fit it’s perceived purpose. I wrote tests for what I thought the functionality was. I realise now that it not what this is meant for.
    I think the edge cases this is supposed to catch would need other code in place for this function to be useful. 

    I have left the app almost un-styled. CSS is not my strong point and I would rather show I understood how to implement Styling than do a rushed and ugly job. The next steps I would take would be to install CSS loader plugin for NWB to handle CSS loading for the production build. I was also confused as to why the “viewport” meta tag for resizing to handheld devices was necessary for what was named as an ATM screen. 

    Having only an intense 3 months coding experience, the 8 hour timeframe quoted was not realistic for me dealing with new technology. I feel that in work environment I would be able to ask more experienced colleagues questions, or pair program to increase my skills quicker. 

    Thank You for you time.

    Daniel Gillespie.

















