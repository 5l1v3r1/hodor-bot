hodor-bot
=========

Hodor meets IRC.

This program implements a funny little chatbot which says, under
certain conditions, "Hodor."  It serves as a simple example of an IRC
bot in python:

* It joins channels when invited
* It replies to private messages
* It (intermittently) speaks in channels when others are speaking
* It also conveniently presents protocol information on stdout.

Requires the irc package, but uses the API of an old version.  To run this
program, I recommend the following:

    git clone http://github.com/clintonc/hodor-bot
    virtualenv hodor-bot
    cd hodor-bot
    source bin/activate
    pip install -r requirements.txt

Usage
-----

    usage: hodor-bot.py [-h] [--server SERVER] [--port PORT] [--nick NICK]
                        [--probability PROBABILITY] [--verbose] [--debug]

    Hodor meets IRC.

    optional arguments:
      -h, --help            show this help message and exit
      --server SERVER       Server to connect to (defaults to localhost)
      --port PORT           Port to connect to
      --nick NICK           Nickname to connect with
      --probability PROBABILITY
                            Probability to reply in channel per message
      --verbose             Print to stdout all events
      --debug               Debug messages

