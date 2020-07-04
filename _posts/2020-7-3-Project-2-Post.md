---
layout: post
title: Project 2 Post
---

As far as difficulty, this project went much better for me than the 1st project did. Like the 1st project, I did run into some technical difficulties. However, there were fewer, so I will count this as a win. 

There were some things about the data that I didn't understand and still don't entirely get. The LDA variables seem like they came from a different analysis and analyzing text is not something I've ever done before, so understanding how someone could measure things like "positive words" or subjectivity were difficult for me. I took the route of turning the problem into binary classification and selected a Logistic Regression model along with a Random Forest for my 2 models. At first, I thought that this would make predictions easier because we are essentially getting rid of the need to have an exact prediction for number of shares. Additionally, it makes more sense to me to say "this article had a high volume of shares" as opposed to "This article had 10,000 ish shares". However, I believe the threshold wasn't set all that well. 1400 was the cutoff value mentioned in the prompt for the project (which I think is the median number of shares). The data as a whole was **Very** concentrated around that value and I think that made prediction a nightmare for these models (though I could have picked my models poorly). I think that if you had a near infinite amount of computation power, I'd like to pick the cutoff value that determines high and low volume (by cross validation or something else). However, I am in no way set up to do that, so I didn't. 


On the topic of computation, I ran into a pretty big issue when I utilized the MASS package's function stepAIC and selected "backward" as the direction. I couldn't really figure out why that was, but it would take nearly 20 minutes to find the model with lowest AIC. However, when I reversed the direction, the computation was much faster. With my luck, I likely arrived at the worst model because of this, but I couldn't figure out how to speed it up with parallel computing. 

I only ran into the issue of not really understanding how GitHub organizes files during this project. I had a funny problem where one of my analysis files for one day of the week was getting capitalized somewhere and I couldn't figure out how to trace where the issue was (files weren't linking correctly because of this).

All in all, the project was pretty fun. I'm loving how I can push changes to GitHub from R Studio, but I wish I could figure out how to see old versions of files a little more easily. I still don't quite understand the difference between forking, commiting, pushing, pulling, etc. just yet. I suppose it's in due time. 

My project can be found [here](https://rwest-ncsu.github.io/558-Project-2/) with subsequent links to the analysis for each day. 
















