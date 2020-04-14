# Heroku Deployment

This guide will go over deploying your site to Heroku and setting up a MongoLab database for your site. We'll be using the commad line to run our commands.

## Installation

Start by installing Heroku Toolbelt:

`brew install heroku-toolbelt` or `sudo apt-get install heroku-toolbelt`

Sign up for an account on [Heroku.com](https://www.heroku.com/).

## Login

Use `heroku login` to login into heroku.

In case you are alredy logged in, use `heroku auth:whoami`b to reveal who you are logged in as.

## Create a heroku app

`heroku create <appname>`

`git push heroku master`

The heroku deployment is done at this point. Open your favorite browser and point it to the heroku url.

My favorite way to open my new heroku app is using ```heroku open``

## Set-up database with MongoLab

Back on the command line:

`heroku addons:add mongolab` Will ask for verification.

`heroku config` Displays mongo.uri. We have to st this to the mongoURI

`heroku config:set MONGO_URL=<mongo uri>`

`heroku config:set STATIC_DIR="/dist"`

Sign up for a free-tier sandbox account at [mongolab.com](https://mongolab.com/).

Add a remote connection, set name to your databse name and add your MongoURI.

