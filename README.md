# Selenium-Twitterbot-Starter


## About

Makes a request to twitter.com/login and saves cookies to a .json file.\
If cookies exist upon startup, uses the cookies to log in instead.


### Prerequisites

Have a recent copy of node installed on your machine.\
Have a webdriver on your system path.

### Installing

1. Download the source code
2. Unzip the files
3. Navigate to pw.envEXAMPLE
4. Enter your credentials
```
TWITTER_PHONE is used to handle 'Unusual Login Activity' error.
In case of error, the application will log in with phone number instead.
If this doesn't work, try replacing with your username.
```
```
TWITTER_EMAIL = ""
TWITTER_PASSWORD = ""
TWITTER_PHONE = ""
```
Remove EXAMPLE from the end of the filename.\
You should be left with __pw.env__

5. Open a terminal window and cd into the folder
6. Install the dependencies:
```
npm i
```


## Usage <a name = "usage"></a>

Run the application:
```
node src/app.js
```

The bot will:
1. Open a browser window
2. Check for existing cookies
3. If cookies exist, navigate to twitter.com/home with cookies
4. Else, navigate to twitter.com/login and enter the credentails found in the pw.env file
5. Once logged in with credentials, save the cookies to a json file for use upon next run