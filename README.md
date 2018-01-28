# About-a-route
Unfinished game based on the GGJ2018 "transmission" theme, where you route messages via Pigeon post and packages via courier riders and horse carts in a medieval packet-switching trade route network pestered with robbers and all...

It can (when finished) be played as a multiplayer board game or digital (web based) or a hybrid/mix.

## Inspiration / background
Some internet "RFC" specifications specify how to transport internet packages using Pigeon mail. Yes, birds! See:
- https://en.wikipedia.org/wiki/IP_over_Avian_Carriers - including live tests.
- https://tools.ietf.org/html/rfc1149 (1 April 1990)
- https://tools.ietf.org/html/rfc2549 (1 April 1999)
- https://tools.ietf.org/html/rfc6214 (1 April 2011)

Do the cooperating and simultaneously competing network carriers of today really significantly differ from their medieval colleagues in this game? Do some routing strategies perform better than others? (Hints from what modern internet routers do, see:  https://en.wikipedia.org/wiki/Routing)


## Data

Game-data like unit speed, costs, distances etc is in the Google sheet: https://docs.google.com/spreadsheets/d/1Hdv2bzW4Izl0eYmpvZojKtlYjOsgi-PUenAtSnbTU8k/edit?usp=sharing

## Digital version
Currently being too slowly hacked away at https://ide.c9.io/eriksundvall/about-a-route (more of that code will move to the https://github.com/lophtix/About-a-route/ github repo later). By cut & paste of a region from the above described google spreadsheet into the conversion service at http://www.csvjson.com/csv2json different JSON-snippts can be generated for the digital version (currently imported via the file game-data.js). 

The digital verion is on the serverside based on https://nodejs.org and a lightweight NeDB database https://github.com/louischatriot/nedb. HTML5+Javascript (including a bit of simple Angular and bootstrap) is used on the client side. Communication between server and client is mainly done via websocket messages, so future alternative clients coud be huilt using other technologies than HTML/web.

## Hybrid?  
Clients can be set to view the game from a specific town's perspective and could be viewed on e.g. separate phones/computers at different locations in a building or room where you'd have to walk to change perspecrive...

