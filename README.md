# pogo-notifier
Live real-time GPS based notification system about nearby Pokemons in Pokemon Go. You get notifications in real world as you move.

Proof of concept
https://www.youtube.com/watch?v=ri6d2Ol6WIs

First install following apps on the phone (ios or android)

    Traccar Client https://www.traccar.org/client/
    Slack https://slack.com/

Then you need a linux server to run Pokemongo-Map from

    https://github.com/AHAAAAAAA/PokemonGo-Map

Run it using:

python runserver.py -H 10.10.10.10 -P 2020 -u googleuser@gmail.com -p googlepassword -a google -l "59.0 10."7 -st 3

Then you need to:

    Install webserver with PHP and composer (google it)
    Change port of the webserver to 5055
    Point Traccar Client to IP of your server with port 5055
    Place index.php file from my git so it will answer on 10.10.10.10:5055/ (usually root of the server).
    Edit index.php with corrent Slack webhook (google it) and IP to the Pokemongo-Map server
* Edit $server with IP to your server
* Add slack webhook
* Run composer update

Enjoy! :)
