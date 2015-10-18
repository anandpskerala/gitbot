# Jannes' GitBot
#### A Python Telegram bot that notifies you via Telegram if there is a push event in one of your repositories

It uses the Flask microframework and the [python-telegram-bot](https://github.com/leandrotoledo/python-telegram-bot) library. It's based on this [example](https://github.com/sooyhwang/Simple-Echo-Telegram-Bot).

The file is prepared to be run by anyone by filling out the blanks in the configuration.

## Required
* Python 3.4 (may work with earlier versions, untested)
* [python-telegram-bot](https://github.com/leandrotoledo/python-telegram-bot) module (tested with version 2.8.7)
* [Flask](http://flask.pocoo.org/) microframework (tested with version 0.10.1)

## How to use
* Install the script
* Edit BOTNAME, TOKEN, BASE_URL, HOST and PORT in bot.py
* If you want to handle SSL with Flask, also fill out the CERT and CERT_KEY fields and check the section about SSL.
* Visit https://BASE_URL/set_webhook on your web browser to set up webhook.
* Follow Bot instructions

## SSL
You can start the server without an SSL context, if this is handled by another programm, like Apache or haproxy. You can leave out the SSL Information in the header and select the second run-line at the end of the file 

Please note that you need a valid ssl certificate or a self-signed one. Please refer to [this gist](https://gist.github.com/leandrotoledo/4e9362acdc5db33ae16c) for an example with self-signed certs.
