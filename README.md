# ACMSCryptocurrencyPriceTracker_Pragya
Data is fetched from a third party API -cryptocompare.com with least granularity/margon of 30 minutes.
Since there is no limit for the number of accceses a user can have,daily and monthly data is fetched on the fly so as to give user updated data upto our granularity.
the fetched data is currently stored in json file-each cryptocurrency has its own json(improvement needed-backend database)
Graph is generated by pygal library which finally renders a SVG image in static/image which can be passed on to user side as it is to give user an interacive image.
currently hosted on localhost
localhost:portno/PerHalfHour - parameters: SourceCurrency,ConvertToCurrency,Numberofrecords,Aggregatetime
localhost:portno/LineGraph - creates a svg file as per the records generated 