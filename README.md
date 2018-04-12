# One Reader App

##APIs Used:
* Twilio
* Hacker News
* Forismatic Random Quote API
* The Verge (RSS/.xml)

This is a simple reader app that pulls the latest top stories from both the HACKER NEWS API and THE VERGE RSS (.xml).

We also added a random quote generator using an API for good measure.

Hackers News and The Verge are my two favorite news sources, so I thought it'd be fun to build a little reader putting all of their latest headlines in one place.

I also added a simple Twilio integration that sends an SMS to my phone number with the top story from The Verge so that I can read it later.

The Hacker News API was interesting to deal with because it actually requires two API calls to get the information in the app. First, we have to call the IDs of the top stories, and then once we have the IDs, we can use those to find the actual title and link for the associated posts.

Learning to parse an .xml file was also a challenge, and while the concept is similar to working with JSON from APIs, it required different code and (after much StackOverflowing) use of the from_xml method. Something I learned throughout this was the capabilities already built into Ruby. I should've just started with the documentation instead of Googling for an answer.

Anyway, I use an RSS reader regularly (Feedly), but don't really like it, so it'd actually be a fun project to build out my own RSS reader now that I know how to parse .xml data into a hash and make it useable in Ruby.

There are a lot of ways I envision building out the functionality of this more so that it's actually a "homepage" I'd use on a regular basis.
