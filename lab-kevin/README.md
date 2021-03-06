># Lab 28: To Do

Using react and react, create a simple application for creating and deleting notes. The application has a simple landing page with a navbar. The app has a dashboard view with links to a input form and a note view form.  Currently the application persistance is per session.  All Data is reset on page reload.

>## Install

```BASH
    npm i
```


```BASH
    npm run build
```

```BASH
    npm run watch
```

### Dependencies 

- This project has the following dependencies:

```JSON
  "devDependencies": {
    "babel-core": "^6.26.0",
    "babel-loader": "^7.1.2",
    "babel-plugin-transform-object-rest-spread": "^6.26.0",
    "babel-preset-env": "^1.6.1",
    "babel-preset-react": "^6.24.1",
    "css-loader": "^0.28.9",
    "enzyme": "^3.3.0",
    "enzyme-adapter-react-16": "^1.1.1",
    "eslint-plugin-react": "^7.7.0",
    "extract-text-webpack-plugin": "^3.0.2",
    "html-webpack-plugin": "^2.30.1",
    "jest": "^22.4.0",
    "node-sass": "^4.7.2",
    "react": "^16.2.0",
    "react-dom": "^16.2.0",
    "react-router-dom": "^4.2.2",
    "resolve-url-loader": "^2.2.1",
    "sass-loader": "^6.0.6",
    "uuid": "^3.2.1",
    "webpack": "^3.11.0",
    "webpack-dev-server": "^2.11.1"
  }
```

### npm scripts

- The following npm scripts are available:

```JSON
  "scripts": {
    "test": "jest --verbose -i",
    "build": "webpack",
    "watch": "webpack-dev-server --inline --hot"
  }
```

### Tests

  - There are two tests for the existence of initial state, one for the dashboard and one for the form.  Tests can be run with the following command:

```BASH
    npm test
```


>## Architecture 

  ### App

    - The App component renders the header, footer and sets of the routes for the main navbar

  ### Landing

    - The landing component contains the home view of the application and is the endpoint for the Home link in the navbar

  ### Dashboard

    - The dashboard contains the main state of the dynamic components for creating and deleting notes.  The dashboard state contains the array of notes. 

    - There is a secondary navbar with links to the create form and the note view

  ### Note-create-form

    - This component contains a view with a form for creating notes.

    - The form has a title and content field and a "Rock the Boat" submit button.

    - Notes at minimum, have to have a title or content to submit

    - To view the note, once submitted, click the 'View Notes" link

  ### Note-list

    - This component creates a view of note items

    - Each note item has a "tip the boat over' button that deletes the note





