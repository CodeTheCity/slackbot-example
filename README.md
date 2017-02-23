# jazzbot

This is a Jazz Bot which runs in Slack and which will answer questions about my jazz album collection.

It responds to a range of commands: 

* album, 
* count,
* artist
* wildcard album,
* wildcard artist
* help. 

The latter prompts the user to use valid entry.

![screenshot](https://github.com/watty62/jazzbot/blob/master/Screenshot%202017-02-05%2013.27.19.png)

I've now got it connected to a SQLite 3 database containing two tables - Artists and Albums - which it queries and uses to answer commands.

It is highly inspired by my friend [Andrew Sage](http://twitter.com/symboticaandrew)'s [Slackbot](https://github.com/andrewsage/slackbot) but is not done in an Object Oriented way. We were both inspired by Matt Makai's [Slack Starterbot](https://github.com/mattmakai/slack-starterbot/)

My intention was to create somthing that I can query from afar and it will tell me if I have a particular album.

Now it is working quite reliably.

If you are want to copy this for yourself follow the set-up instructions on Matt Makai's blog above.  

I don't run my version in Virtualenv (although I should!), so I sore my credentials in a secrets.py file and import that, rather than exporting environment variables.

Also, you'll need a couple of modules which can be installed using "sudo pip install" - sqlite3 and SlackCLient.

Have fun!
