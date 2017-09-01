# dashboardAuth-hbs
### Dashboard with user authentication - built with Express and Handlebars

[![Greenkeeper badge](https://badges.greenkeeper.io/sethbergman/dashboardAuth-hbs.svg)](https://greenkeeper.io/)
********************************
[ ![Codeship Status for sethbergman/dashboardAuth-hbs](https://codeship.com/projects/66047110-1a59-0134-0759-3217b0339886/status?branch=master)](https://codeship.com/projects/159315)

### Clone
```
git clone https://github.com/sethbergman/dashboardAuth-hbs.git && cd dashboardAuth-hbs
```
### Install dependencies:
```
npm install
```
### Setup configuration scripts:
* Create a file in the `config` folder called `auth.js`.
* It should have something like the following in the file:
```
module.exports = {

    'facebookAuth' : {
        'clientID'        : '1112223334445557777777',
        'clientSecret'    : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'     : '//dashboard-hbs.stackriot.com/auth/facebook/callback'
    },

    'twitterAuth' : {
        'consumerKey'        : '1112223334445557777777',
        'consumerSecret'     : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'        : '//dashboard-hbs.stackriot.com/auth/twitter/callback'
    },

    'googleAuth' : {
        'clientID'         : '123-1112223334445557777777.apps.googleusercontent.com',
        'clientSecret'     : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'      : '//dashboard-hbs.stackriot.com/auth/google/callback'
    },

    'githubAuth' : {
        'clientID'        : '1112223334445557777777',
        'clientSecret'    : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'     : '//dashboard-hbs.stackriot.com/auth/github/callback'
    },

};
```

Create a file in the `config` folder called `database.js`.
* It should have something like the following in the file:
```
module.exports = {

    'url' : 'mongodb://mongouser:mongopass@ds03162.mlab.com:03162/mongoname'

};
```
### Start the app!
```
npm start
```
### Visit [//0.0.0.0:5000](//0.0.0.0:5000) in your browser.
