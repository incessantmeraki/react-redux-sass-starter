# React-boilerplate

This project acts a boilerplate for a project that uses react, redux, and sass. Just clone the repository and being adding things required.


## Structure

The main project resides inside ```/src``` directory and has following hierarchy

```
  ├── containers
  ├── components
  ├── actions
  ├── reducers
  ├── store
  ├── selectors
  ├── routers
  ├── graphql
  ├── index.js
  ├── index.css
  ├── registerServiceWorker.js
  ├── setupTests.js
  ├── static
  ├── styles
  │   ├── abstracts
  │   ├── base
  │   ├── components
  │   ├── index.scss
  │   ├── layout
  │   ├── pages
  │   ├── themes
  │   └── vendors
  └── tests
      ├── actions
      ├── components
      ├── fixtures
      ├── __mocks__
      ├── reducers
      └── selectors
```


## Architecture

#### React
React is used to build the interfaces which reside in the folder ```components``` and ```containers```. containers contains code for interfaces that are complex and needs to manage state for various data. components contains code for simple interfaces which usually receive data from the containers and do not need to manage their own state.

#### Redux
Redux is used as a single source of truth for data used in the application. The directories ```actions```, ```reducers```, and ```store``` contain the redux code. ```selectors``` directory contains the utlility functions that is used by components to filter out the data they recieve from redux store.

#### CSS
This project uses SASS as a proce-pocessor for CSS. It resides inside ```styles``` directory and follows a 7-1 pattern where 6 different directories contain css for various aspects of the website and all these are imported by 7th file ```index.scss```. This is the file that's compiled into ```index.css``` during dev and build process.

#### Tests
The code that does testing resides in ```tests``` directory. Enzyme is used as the main testing library and jest as an assertion library. 


## Setup

#### ``` npm start ```
This command runs the development server in watch mode.

#### ```npm run build```
This command builds the production version of the website inside build folder

#### ```npm test```
This command runs the tests
