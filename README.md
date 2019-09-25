This project has a React front-end and a Rails backend, each with its own repo. The two repos have been wrapped in a meta repo.
To install meta and clone the meta repo, run npm i -g meta && meta git clone git@github.com:stazman/daily-weight-loss-advisor-app.git. Further info about the meta app can be found here: https://github.com/mateodelnorte/meta.

It has been set up to use Webpack dev server to proxy requests to the Rails API server (http://localhost:3001) as a proxy server to avoid CORS issues.

If you already have Ruby, Bundler, Rails, Node.js and NPM installed, follow these steps to run the app:

Fork and clone this repo. cd to the directory from the terminal. In the terminal:

run bundle install to install all required gems
run bundle exec db:migrate db:seed to migrate and seed the database
run rake start to start the web server and Rails api server
NOTE: The following sections will be completed and may be altered as the project continues in development:

To install Ruby:

use Ruby version 2.3.3p222 for this project.
To install Bundler:

use Bundler version 1.17.2 for this project.
To install Rails:

use Rails version 5.2.3 for this project
To install Node.js:

To install NPM:

To install React:

More Ruby Setup Information:

System dependencies

Configuration

Database creation

Database initialization

How to run the test suite

Services (job queues, cache servers, search engines, etc.)

Deployment instructions

More Rails information:

More React information:

This project was bootstrapped with Create React App.

Available Scripts
In the project directory, you can run:

rake start
Runs the app in the development mode, with .
Open http://localhost:3000 to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console. -->

npm test
Launches the test runner in the interactive watch mode.
See the section about running tests for more information.

npm run build
Builds the app for production to the build folder.
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.
Your app is ready to be deployed!

See the section about deployment for more information.

npm run eject
Note: this is a one-way operation. Once you eject, you can’t go back!

If you aren’t satisfied with the build tool and configuration choices, you can eject at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except eject will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use eject. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

Learn More
You can learn more in the Create React App documentation.

To learn React, check out the React documentation.

Code Splitting
This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

Analyzing the Bundle Size
This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

Making a Progressive Web App
This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

Advanced Configuration
This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

Deployment
This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

npm run build fails to minify
This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify