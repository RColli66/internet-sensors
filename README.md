internet-sensors projects
README.md
May 19, 2014 (revised twitter streaming project)

A web version of this document (with pictures) can be found at: http://zerokidz.com/ideas/?p=5859

NOTE!!! - This project is undergoing active revision 5/2014 - The projects are being re-tested and moved to separate folders. Because things have gotten out of hand. 

---
overview:

This is a series of projects that demonstrate ways to use Internet API's for interactive media projects.

Projects have been tested on Mac OS 10.7 (Lion). All but one of the projects use Max/MSP 6.1.0 from: http://cycling74.com. The other project uses Pure Data 0.42.5 (extended) from: http://puredata.info. Other required programs are listed in the documentation for individual projects.

---
downloads:

The links for the projects below include operating instructions. All the patches, source code, and data can be downloaded from the github repository:

 https://github.com/tkzic/internet-sensors

---
authorization:

Some of the projects require you to get passwords and API-keys from providers. For example, you'll need a Twitter account, to run the 'Twitter streaming API in Max' project. For projects which need authorization you'll need to modify the patches/source code with your user information - as directed - or they just won't work.

---
help:

The API's used in the projects change fairly often. So there's no guarantee they'll work. If you find problems or have ideas - please post to them to the github repository. Or email me at tkzic@megalink.net with "Internet sensor projects" somewhere in the subject heading.

---
Projects: For up to date list and links see: http://zerokidz.com/ideas/?p=5859

---

Twitter streaming API in Max
Sending tweets from Max using curl
Sending tweets from Max using ruby*
Sending tweets from Max using speech 
A conversation with a robot in Max 
Playing bird calls in Max 
Soundcloud API in Max 
Real time train map using Max and node.js 
Playing stock market music with Max ([Note] This project is currently not part of the github archive.)
Using wind forecast data to drive wind sounds in Pure Data 
Using ping times to control oscillators in Max
Echo Nest segment analysis player 
Flying a Quad-copter AR_Drone with Max
Adding Markers to Google Maps in Max
Max data recorder
Web Audio Google domain ping machine

*Use a Fisher Price Little Tikes piano


---

[note 5/17/2014]: 
1) Added Google Maps
2) Added Little Tikes piano
3) Added data recorder
4) Added web audio domain ping machine

---

[note 5/13/2014]: 
1) Added quadcopter AR_drone project

---

[note 5/1/2014]: 
1) Fixed ‘blocking’ in google speech and chatbot apps when togging voice record
2) added missing file autorecord-buffer2.maxpat
3) NOTE: still need to update documentation for the auto record / chatbot projects


---

[note 3/26/2014]: 
1) Complete revision of chatbot conversation project - cleaned up UI, added auto record feature
2) Fixed minor bugs in streaming Max twitter php code
3) updated google text to speech api program (also does auto record)
4) NOTE: still need to update documentation for the auto record / chatbot projects


---

[note 2/2/2014]: 
1) Complete revision of streaming Max Twitter project.
2) Added new project: segment analysis player that sonifies echonest audio analysis data.

---

[note 9/8/2013]: 
Yet another change for Twitter. In the Max patch which sends Tweets using a ruby server, you no longer need to use xively.com and zapier.com but you do need to set up a Twitter app to get the oauth authentication strings for the ruby program. Instructions are at: http://zerokidz.com/ideas/?p=7013 - I think this is useful because its faster, more direct, and free!

---

[note 9/2/2013]: Surprise! Any of the projects which used Twitter were now broken in June 2013, due to requirement for Oauth and some changes to the Twitter API version 1.1, and changes to cosm.com (now xively.com) - I have fixed the programs and revised documentation. 9/2/2013. For sending Tweets you'll need to adjust your xively.com triggers using zapier.com. For streaming Tweets there is new php code and you'll need to set up a Twitter App under your account - but this is all in the revised documentation at the link above.


---

[note]: the wind forecast API from http://cordc.ucsd.edu appears to be broken. There's no data. As a 
workaround, I have written a new pd patch and ruby script to use data from http://openweathermap.org (OWM) -
So... until I get a chance to write up documentation, please make the following substitutions when
running the 'wind' project:

wind-open-forecast.rb replaces: wind-forecast.rb

wind-open-machine.pd replaces: wind-machine.pd

The API's are different - OWM gives a 7 day forecast with fewer data points, but it has worldwide data,
more weather params, and after some tweaks... Actually the gust data sounds cool. And it defaults to 
Rumford, Maine when you start the server. 



