This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

### Environment Variables

First make sure you create a JSON key for the Google Cloud service account `my-app-screenshots`. You can create the key from the [Service Accounts page](https://console.cloud.google.com/iam-admin/serviceaccounts?project=disco-stock-218303).

Update your `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to this JSON key. Then update your `ROUTINE_DESIGN_GOOGLE_CREDS` with this command

```
export ROUTINE_DESIGN_GOOGLE_CREDS=$(cat $GOOGLE_APPLICATION_CREDENTIALS)
```

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm run render`

Runs the `./test/render` directory on [http://localhost:8080](http://localhost:8080)

### `npm run test:screenshots`

Checks that existing code matches the screenshots saved in `image.json` files in `./test/render`.

If you have a failing test, open the test's Google Cloud URL and you'll see subdirectories for each screenshot image that failed within the directory. Each subdirectory has a `new.png` and a `diff.png`. 

* `new.png` is the screenshot of the React/Sass code in the current branch
* `diff.png` is the diff between `new.png` and the image saved in `image.json`

### `npm run test:unit`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run capture`

Upload new screenshot images for each changed component, and updates the `image.json` files.

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
