# dashboardAuth-hbs
### Dashboard with user authentication - built with Express and Handlebars
********************************
[ ![Codeship Status for sethbergman/dashboardAuth-hbs](https://codeship.com/projects/3a8c3820-15cc-0134-a125-667ff3898a5e/status?branch=master)](https://codeship.com/projects/158178)
Clone
```
git clone https://github.com/sethbergman/dashboardAuth-hbs.git && cd dashboardAuth-hbs
```
Install dependencies:
```
npm install
```
Setup configuration scripts:
* Create a file in the `config` folder called `auth.js`.
* It should have something like the following in the file:
```
module.exports = {

    'facebookAuth' : {
        'clientID'        : '1112223334445557777777',
        'clientSecret'    : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'     : 'http://dash3.stackriot.com/auth/facebook/callback'
    },

    'twitterAuth' : {
        'consumerKey'        : '1112223334445557777777',
        'consumerSecret'     : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'        : 'http://dash3.stackriot.com/auth/twitter/callback'
    },

    'googleAuth' : {
        'clientID'         : '123-1112223334445557777777.apps.googleusercontent.com',
        'clientSecret'     : '111abc222def333ghi444jkl555mnopqr7777777',
        'callbackURL'      : 'http://dash3.stackriot.com/auth/google/callback'
    }

};
```

Create a file in the `config` folder called `database.js`.
* It should have something like the following in the file:
```
module.exports = {

    'url' : 'mongodb://mongouser:mongopass@ds03162.mlab.com:03162/mongoname'

};
```
Start the app!
```
npm start
```
Visit [http://0.0.0.0:5000](http://0.0.0.0:5000) in your browser.
