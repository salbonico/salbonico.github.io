---
layout: post
title:      "Hey, it's BeerBuddy! "
date:       2019-01-26 18:00:07 +0000
permalink:  hey_its_beerbuddy
---


Hello! I'm Steve and I'm currently learning Web dev with FlatIron. Now you might ask what are my main goals in life at the moment, and well. Coding, Drinking, and Traveling. So I figured with my first portfolio project, I'd code something that helps me with all three!

So here's the deal. Me, the wife, and the doggo have this plan, we're going to save up, trade in a car and buy a fifth wheel and truck and travel around the states in it while she makes money doing amazing photography and I pick up a job doing remote work. We did this a couple years ago and it ruled! Except there was an issue.

# Which beer to drink when in a new location?
If only I had some sort of buddy who always knew the best brews in a new location?

Well then, with my knowledge of Ruby, it's time to make that beer buddy in a convienient CLI form.

BeerBuddy took the better part of two full days, most of which was spent figuring out how to scrape beers from the very very fine folks' work over at TapHunter.com. They don't actually know I'm pulling from their stuff, but I'm sure if they did, a few beers and we'd have the whole thing figured out. 

So, how does it work?

When you wake up BeerBuddy, he asks for your location. Whats cool is that taphunter.com has a great URL that essentually lets you just build location in plain text and then fill in that you just want beers to come back.

https://www.taphunter.com/search/?type=beers&near=94553

See that type= part? That lets me make sure the return is always beers, so my future scrapes are always confident in what they'll get back. Then the near= thing is great, you could type in anything and it will bring back results from eaither a zip, a town, a state, or even random words like poo (Brings back a place in Canada that I now need to go drink in.)

Cool, so a few list scrapes later and I'm now pulling in their awesome lists of good beers on tap nearby. Take those bad boys and convert them into objects, then display away.

But now, just barfing a list of like 40 beers and all of their stats is simply not refined enough for the modern craft beer leyperson. So I decided to only bring back the top ten and then drop an index number on them for easy selection. So at first, you get just the name and type, and then you can select a beer and get all the good stuff like description, IBUs, brewer, and even the ever important ABV! (How toasty it'll get ya.)

So the funny thing at the end was trying to find someplace, anyplace that would have no beers so I could test my error checking. This was super hard! Even "poo" brought back a spot in Canada that had some good beers! But luckily for me, i did find it, a beer desert, in the poor poor zip code of 92222. A mysteriouse place known only as Bard, CA. These poor people with no good beer anywhere near them. I must see this place for myself. 

Anyways check out BeerBuddy for yourself at https://github.com/salbonico/BeerBuddy-CLI !

I've allready used it to try a few new beers out here in Oakland.

-Steve


