MasterBot
=========

Uncrashable Python IRC bot

This is a pet project I've been working on for fun, so there's a number of "hack" solutions to problems, given that the problems arise due to specifics with IRC networks. It's designed to fit around the standards implemented for IRC, specifically the freenode network. 

When first downloaded, moving into the main folder and running BotShell.py will initialize the user data.

Then, you should open up UserData/Data.txt, and add the necessary data following the commas so that you can connect to the IRC server with the name you'd like. After that, simply run BotShell.py to start the bot up.

All commands are stored in Commands.txt, using a code specified in the Mem class of cmds.py. 

Known bugs: Ogame highscore functionality does not properly deal with connection hangs. The entire script will go down due to the signal method currently in place, which I am unhappy about. Therefore I've simply disabled the Highscore functionality, which shouldn't be a problem unless you really want ogame data. Also, I need to implement something which ensures that cmds doesn't return a string too long to be sent. Currently, the help text will be truncated because of this. License has not been selected as my licensing experience is nil and I haven't had a reason to license yet as this is just a pet project. 
