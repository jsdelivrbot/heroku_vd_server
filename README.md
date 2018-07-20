# Instant Games Server Demo

This demo contains code that demonstrates common scenarios in a backend service that supports an Instant Game client: a game bot and a storage service.

## Pre-requisites
1. npm ([Install npm](https://docs.npmjs.com/cli/install))
1. Postgresql([Install Postgresql](https://www.postgresql.org/download/))


## Install Dependencies
```bash
$ npm install
```

## Configure environment variables
You can rename the file `template.env` into just `.env` and input test values of the variables below. This file will be used for local testing. When you host your code in the cloud, you'll need to reconfigure these variables to their production values.

1. `BOT_VERIFY_TOKEN`: create a memorable word. You'll use that to validate webhooks with your Messenger Bot
1. `APP_SECRET`: paste your App Secret. This can be found in your App's settings page. c1fb975db01e9e1623a66b30972a1197
1. `USE_SECURE_COMMUNICATION`: 1
1. `PAGE_ACCESS_TOKEN`: leave blank for now. EAAFXQaBuTiABACWt2dmoG20FZANeFQfaFBqZCjbuRPCNvgBURXA8unUZBpBPyQSRrgtkZAJjmhgjFI8zLYAcaGBnNVjuqX4oxNTbT1OSLXW0pCJ0AITx42E7rZBJHSvTZC4xiputmgQ98uZAGRon87zWf2o7ZBvM1rgxbi8QihL5ERlDfNx6RCSRFYKQD9pyrpnNJCF5rPHdbwZDZD 
1. `DATABASE_URL`: connection string to your Postgres installation https://thawing-shelf-75043.herokuapp.com/ , https://git.heroku.com/thawing-shelf-75043.git

Virtual Dice
App ID: 377414352784928

## Create a Facebook page that will host your bot

1. Follow the instructions on the [Game Bot setup guide](https://developers.facebook.com/docs/games/instant-games/getting-started/bot-setup) to setup a Facebook page that will host your game bot
1. When associating the Webhooks, under the **Verify Token** field, input the memorable word you created for `BOT_VERIFY_TOKEN` above
1. Once webhooks are configured, copy your Page's access token into the `PAGE_ACCESS_TOKEN` environment variable of your hosted app.

All done! Your Backend service is configured!
You can run your code with

```bash
$ node index
```

## Running the client-side code
Follow the instructions in the README.md of the client-side counterpart of this demo:

https://github.com/edgarjcfn/fbinstant-communication


/////
Creating app... done, ⬢ thawing-shelf-75043

https://thawing-shelf-75043.herokuapp.com/ | https://git.heroku.com/thawing-shelf-75043.git


Creating app... done, ⬢ fathomless-tor-94719
https://fathomless-tor-94719.herokuapp.com/ | git@heroku.com:fathomless-tor-94719.git


https://heroku.com/deploy?template=https://github.com/heroku/thawing-shelf-75043/tree/master