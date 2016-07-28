# pogo-notifier

First install following apps on the phone (ios or android)

    Traccar Client https://www.traccar.org/client/
    Slack https://slack.com/

Then you need a linux server to run Pokemongo-Map from

    https://github.com/AHAAAAAAA/PokemonGo-Map

Then you need to:

    Install webserver with PHP (google it)
    Change port of the webserver to 5055
    Point Traccar Client to IP of your server with port 5055
    Place index.php file from my git so it will answer on 10.10.10.10:5055/ (usually root of the server).
    Edit index.php with corrent Slack webhook (google it) and IP to the Pokemongo-Map server
* Edit $server with IP to your server
* Add slack webhook
* Run composer update

Enjoy! :)
