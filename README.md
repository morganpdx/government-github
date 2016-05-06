# Government-GitHub API Scraper

To set up and run:
	Requires python, virtualenv

	virtualenv env   # create virtual environment
	. env/bin/activate 	 # activate virtual environment
	pip install -r requirements.txt   # install dependencies
	python create_db.py   # initialize database
	python gov/scraper.py   # scrape github api to populate database - this will take a while.  A really long while.
	datafreeze freezefile.yaml   # query database to generate org level connections
	python gov/networks.py   # generate gephi network files of org connections

