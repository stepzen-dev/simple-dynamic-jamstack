# Simple Dynamic Jamstack application

## Deploy this to Netlify

[![Deploy to netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/stepzen-samples/deploy-to-netlify-btn-test)

## What is this?

This is a simple "jamstack" application: HTML markdown, JavaScript, and an API. The API in this case is a GraphQL API hosted on [StepZen](https://stepzen.com). The GraphQL API is built on top of the [DEV](https://dev.to/) API, using StepZen's `@rest` directive to [connect a REST service](https://stepzen.com/docs/features/connect-a-rest-service). Learn more about using StepZen to easily create GraphQL APIs [here](https://stepzen.com/docs/what-is-stepzen).

You don't need a StepZen account to run this sample, but we've included a schema definition for the API in the `stepzen` directory of this repository in case you want to run it on your own account. The schema we've included is much more complete than necessary for this application; it covers much more of the DEV api. Feel free to use it to build something cool!

## How it works
This application has a form where you can provide a DEV.to username. Hitting submit queries the GraphQL API for some of the user's profile information (website and twitter), and retrieves the most recent article. 

As this application is simple markdown and JavaScript, no application server is required. You can open index.html locally in a browser and it will work just the same as if deployed to a hosted endpoint. 
