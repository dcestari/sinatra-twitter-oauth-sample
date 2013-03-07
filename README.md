Sinatra Twitter OAuth Sample
============================

This is a sample Sinatra application that shows how to use Twitter's OAuth
authentication and authorisation mechanism

It needs "bundler" to work properly.


Usage
-----

First, install dependencies:

    bundle

Inside `server.rb`, replace `CONSUMER_KEY` and `CONSUMER_SECRET` with the real ones from your Twitter application.
Also, make sure to use the real `CALLBACK_URL` with your hostname and port.

    CONSUMER_KEY="consumer-key-from-twitter"
    CONSUMER_SECRET="consumer-secret-from-twitter"
    CALLBACK_URL="http://your-server-name.com/oauth/callback"

Then, run the server:

    ruby server.rb

And finally, go to [http://localhost:4567/oauth/request_token](http://localhost:4567/oauth/request_token)
(replace "localhost" with your actual hostname), copy & go to the displayed Twitter's URL.

The user's *screen_name* and *access_token* will be displayed after authorising your application.

