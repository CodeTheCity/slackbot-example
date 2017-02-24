# Example Slack Bot Written in Python

This is an example of a slack bot which has been written in Python 2.7. 

Ideally, is should be created in a virtual environment - see the tutorial link on Matt Makai's [Slack Starterbot](https://github.com/mattmakai/slack-starterbot/)page. My example is not done like that and I keep with authentication tokens in secrets.py file which I then import. NOt best practice, I know. 

It has mport two dependencies: sqlite3 and slackclient. Both of these can be installed via "sudo pip install"

# What does Jazzbot do?

It responds to a range of commands: 

* album, 
* count,
* artist
* wildcard album,
* wildcard artist
* help. 

The latter prompts the user to use valid entry.

![screenshot](https://github.com/watty62/jazzbot/blob/master/Screenshot%202017-02-05%2013.27.19.png)

It connecta to a SQLite 3 database containing two tables - Artists and Albums - which it queries and uses to answer commands.

My intention was to create somthing that I can query from afar and it will tell me if I have a particular album.

Now it is working quite reliably.


Have fun!
