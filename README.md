## Daily Weight Loss Advisor

This app is currently set up only for development. It doesn't currently have user accounts functionality.

The app includes two separate repos, daily-weight-loss-advisor-backend (Rails) and daily-weight-loss-advisor-frontend (React/Redux), each with its own repo, packaged in a **meta** file. 

To install **meta** and clone the entire **meta** repo, which will also clone the frontend and backend repos, run ```npm i -g meta && meta git clone git@github.com:stazman/daily-weight-loss-advisor-app.git```. 

Further info about the **meta** app: https://github.com/mateodelnorte/meta

Here are the links to the backend and frontend repos if you wish to clone them individually:

Backend: https://github.com/stazman/daily-weight-loss-advisor-backend
Frontend: https://github.com/stazman/daily-weight-loss-advisor-frontend

**Notes about cloning both repos individually:** 
  1. Currently, the Rails API (backend) server cannot be opened on its own as both the web server (frontend) and Rails API servers are bundled to open together through a **Foreman** gem procfile and rake task. **Foreman** gem repo: https://github.com/ddollar/foreman.
  2. If the repos are being cloned individually, they must be siblings in the same directory for the two servers to be started, as the app is currently configured through the **Foreman** gem.

This app has been set up to use Webpack Dev Server to proxy requests to the Rails API server (http://localhost:3001) as a proxy server to avoid CORS issues.

If you already have Ruby, Bundler, Rails, Node.js and NPM installed, follow these steps to run the app:

1. Fork and clone this **meta** repo/the two repos individually.
2. cd into the daily-weight-loss-advisor-backend directory from your terminal. 
3. Run ```bundle install``` to install all required gems
4. Run ```bundle exec db:migrate db:seed``` to migrate and seed the database
5. Run ```rake start``` to start the web server and Rails API server


## RUBY/RAILS BACKEND NOTES

* Use Ruby version 2.3.3p222 for this project.
* Use Bundler version 1.17.2 for this project.
* Use Rails version 5.2.3 for this project


## REACT/REDUX FRONTEND NOTES

This project was bootstrapped with Create React App.

**Available Scripts**

In the project directory, you can run:

## rake start
Starts both the web server (http://localhost:3000) and API server (http://localhost:3001) simultaneously.

The page will reload if you make edits.
You will also see any lint errors in the console. -->

## npm test

This app currently has no tests.

## npm run build
Builds the app for production to the build folder.
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.
Your app is ready to be deployed!

See the section about deployment for more information.

## npm run eject
Note: this is a one-way operation. Once you eject, you can’t go back!

If you aren’t satisfied with the build tool and configuration choices, you can eject at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except eject will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use eject. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More
You can learn more in the Create React App documentation.

To learn React, check out the React documentation.

**Code Splitting**
This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

**Analyzing the Bundle Size**
This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

**Making a Progressive Web App**
This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

**Advanced Configuration**
This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

**Deployment**
This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

**npm run build fails to minify**
This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
