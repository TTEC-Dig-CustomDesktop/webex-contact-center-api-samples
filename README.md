# Webex Contact Center API Samples

This basic set of samples helps a developer understand the all new Webex Contact Center APIs available today on the **[Webex Contact Center Developer Portal](https://developer.webex-cx.com/)**

## Getting Started

To get started, created an App on the Developer Portal:

- Sign into developer.webex-cx.com with a valid Webex Control Hub Account.
- Create an Application Integration by going to your Profile > Manage My Apps.
- Creating an Application Integration will give you a set of Client ID and Client Secret that you will need for this sample.
- Note: While entering the Redirect URI, ensure it has http://localhost:5000/auth/webex/callback for example.

## Using the API Samples

#### Pre-Requisites:

- Node JS and NPM
- An IDE like VS Code or similar.

```
$ node -v
v14.16.1
$ npm -v
6.14.12
```

#### Steps:

- Ensure you have installed NodeJS and NPM
- Clone this Repository / Download it.
- Create a .env file in each of the folders with the settings of the environment variables required to initialize the environment variables. Your server.js will pick it up from the local .env file in the root folder.

`$ cat .env`

```
PORT=5000
CLIENT_ID=<your-client-id>
CLIENT_SECRET=<your-client-secret>
REDIRECT_URI=<your-redirect uri - ex: http://localhost:5000/auth/webex/callback>
ORG_ID=<your-org-id>
```

- Run `$ npm install`

- Run the App

`$ nodemon` OR `$ npm start`

- Go to http://localhost:5000 to fetch an access token
- Go to http://localhost:5000/tasks or http://localhost:5000/users to see the basic GET Tasks and GET Users examples.

Expand / extend the sample app(s) as required.
