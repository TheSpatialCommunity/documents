# Introduction to Bots

There are a couple of special bots present in the Spatial Community that are worth knowing about. This is a short guide to using them.

## Call Admin

If you want to send a message to the admin team, use this command. It will let them know what channel you have sent it from, along with a message why we should be looking at things.

Invoke it using `/call_admin {message}`. The admins will see something like `user: {your handle}, channel: {channel sent from}, message: {message}`.

Usually we will drop in on the channel and see what is going on. Depending on the situation, it will then be discussed between us and a decision as to what needs to happen will be made between the admin team.

### Example of Use
`/call_admin Please can you write a guide to bots?` which will send the admin team a message as follows: `user: joe_blow, channel: #random, message: Please can you write a guide to bots?`.

## PointsBot

This bot awards extremely valuable internet points to people. There is no real criteria as to what a valid reason for giving points is, but they are usually used to thank people for giving advice.

Valid calls to this are the following:
`/points {@username} (user to give points to) {points} (points to give, -100 to +100) {reason} (optional)`
`/points me` (your score)
`/points top_5` (top 5 on the scoreboard)
`/points low_5` (low 5 on the scoreboard)
`/points givers` (top 5 givers scoreboard)
`/points takers` (top 5 takers scoreboard)

Awarding points to yourself is not allowed. Totals in excess of +-100 will be capped at +-100.

### Example of Use

`/points @mtb-za 100 Brilliant guide to bots! Thanks!`

## Glob

If you want to search through all the channel names for something, this is what you want to use. The syntax for the search query should be the same as the standard `*nix` tool `glob`. A summary can be found on [https://en.m.wikipedia.org/wiki/Glob_(programming)#Syntax](Wikipedia). Please let the admin team know if you are trying something that does not actually work as expected.

The command is invoked using `/glob {search pattern} {number}`.

### Examples of Use

`/glob loc-* all` will list all the channels starting with `loc-`. A more complex alternative is `/glob loc-[a-z]*`, but the output is the same (in this case because the channels do not have numbers in them).

    Top 25 matching channels:
    #loc-canada (74 members)
    #loc-aotearoa (56 members)
    #loc-pac-nw (55 members)
    #loc-norcal (46 members)
    #loc-australia (44 members)
    [20 more]

`/glob gis 5` will list the first five channels that have `gis` somewhere in the channel name, sorted by number of users who have joined it.

    Top 5 matching channels:
    #arcgis – ArcGIS stack related chat (519 members)
    #arcgis-web –  (373 members)
    #qgis – To discuss specific tasks in QGIS, a free and open-source Geographic Information System. (373 members)
    #postgis – PostGIS discussion, news, tips, tricks (260 members)
    #arcgis-desktop –  (247 members)

## Poll

If you need a poll for some reason, this will allow you to create one. YOu can also make the poll anonymous, which will not show who has voted for which option.

Invoke it using `/poll "{question}" "{option a}" "{option b}" "{so on}"`.

### Example of Use

`/poll "Is this bot guide useful" "Yes" "Of course!"`

`/poll "Is this bot guide useful" "Yes" "No" anonymous` will prevent one from knowing who has voted no, and then hunting them down....

## Memes

There are a series of commands that take little interaction. Most of them simply post a meme and/or gif of some kind, and do not take any additional input. You simply use the command on the left, and it will display the link on the right.

Command | Link
-------| -------------------------------------------------------
`/wtf` | http://media1.giphy.com/media/aZ3LDBs1ExsE8/giphy.gif
`/thisisfine` | http://gph.is/1IPoO7R
`/sick_burn` | https://en.wikipedia.org/wiki/List_of_burn_centers_in_the_United_States
`/neat` | https://i.imgur.com/iYOXpB3.gif
`/badgers` | https://www.youtube.com/watch?v=gx6TBrfCW54&feature=youtu.be&t=16s
`/believe` | https://youtu.be/YLO7tCdBVrA?t=2s
`/iwritecode` | http://resguru.com/wp-content/uploads/2011/05/angry-keyboard-user.gif (currently broken)
`/thumbsup` | https://imgur.com/uKL8tJg.gif
`/trap` | https://img.memecdn.com/its-a-trap_o_491986.jpg
`/deepthoughts` | Posts a random deep thought by Jack Handey. According to Wikipedia: "He is best known for his "Deep Thoughts by Jack Handey", a large body of surrealistic one-liner jokes, as well as his "Fuzzy Memories" and "My Big Thick Novel" shorts, and for his deadpan delivery."
