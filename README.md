This is a proof-of-concept project that explores how the [React Context](https://reactjs.org/docs/context.html) system works. It displays a simple form with a language selector at the top of the screen that can toggle the language of the form. 

The language selection is stored in the local state of the parent <App /> component. Using the LanguageContext object, the language selection communicated down to the nested <Button /> and <Field /> child components.

The application demonstrates the following key areas of technical interest:

* Using React's [Context](https://reactjs.org/docs/context.html) system to directly communicate data from a parent component to a nested child, bypassing intermediate components
* Creating Context objects, setting default data values on them and/or passing data into Context using a Provider object
* Reading data from Context either by using `this.context` or using the Consumer object
* Pulling data from multiple Contexts inside of a single component. See the Button component for an example of nested Consumers.
* Additionally, the `replace-redux` branch of this project has some additional code that demonstrates how you might use Context as a replacement for Redux by moving business logic and state management into a 'store' component. (See the LanguageStore component inside of LanguageContext.js)

All instructions for this project came from the excellent [Udemy Modern React with Redux course](https://www.udemy.com/react-redux/).

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
