> ⚠️ Warning: This repo is not actively maintained at this time.

# Vue Lambda Starter

This project is based on [Vue CLI's](https://github.com/vuejs/vue-cli) starter template.

The main addition is a new folder: `src/lambda`. Each JavaScript file in there will automatically be prepared for Lambda function deployment.

As an example, we've included a small `src/lambda/hello.js` function, which will be deployed to `/.netlify/functions/hello`.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/netlify/vue-lambda-starter)

## Babel/webpack compilation

All functions are compiled with webpack using the Babel Loader, so you can use modern JavaScript, import npm modules, etc., without any extra setup.

## Local Development

Before developing, clone the repository and run `yarn` from the root of the repo to install all dependencies.

### Run the functions dev server

From inside the project folder, run:

```
yarn serve
```

This will start the normal dev server and open your app at `http://localhost:8080`.

Local in-app requests to the relative path `/.netlify/functions/*` will automatically be proxied to a local functions dev server running on port 9000.
