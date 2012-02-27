Tweetflux
=========

This is a quick ruby script to save live twitter data to JSON files.

Setup
-----

1. Clone this repository

		git clone https://linenoise@github.com/linenoise/tweetfllux.git
		cd tweetflux

2. Setup dependencies

If you have and prefer to use [RVM](http://beginrescueend.com):

		rvm gemset create tweetflux
		gem install bundler
		bundle install

If you don't have or prefer not to use RVM:

		sudo gem install bundler
		sudo bundle install

3. Give it a twitter username / password combination:

		cp authentication.yml.sample authentication.yml
		chmod go-rwx authentication.yaml
		vi authentication.yml

Running
-------

Searching by tag:

		./tweetflux ows oo opdx

This will produce a runtime logfile in `tags_ows_oo_opdx.log` and save off JSON files in the `fluxes/tags_ows_oo_opdx` directory.

TODO
----

* Searching by user
* Playback (mock the API)

