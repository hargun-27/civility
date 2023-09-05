# Getting Started
### Visit Hosted Site:
https://civility.vercel.app/

### Video Demo:
https://youtu.be/pNMQyDe-3F8

### Run locally:

Run in terminal window to start backend server which allows the API connection
```
npm start
```
Open another terminal and run this to start the front-end
```
npm run dev
```

# Inspiration
We took inspiration from the countless controversial social media posts that often appear online, many infamously posted by famous figures (I'm sure you can think of some). In order to prevent the spread of such heavy negativity throughout the internet and to preserve the ideal images of the celebrities we all love, we thought of a straightforward solution to help social media users keep themselves in check.

# What it does
Civility is a web application that analyzes text and provides metrics based on the social repercussions that a user may incur from posting online. Main factors include age warning, political group alignment, and toxicity level. All three indicators will give a message encouraging the user to do the suggested activities such as not posting or posting with caution. Some indicators will also give a percentage to show the confidence percentage of the suggestion. For example, a percent indicates which side of conservative vs liberal viewpoints the text is favouring.

# How we built it
We built Civility using Next.js, React, Material-UI, Express.js, and of course, the Cohere API. We used Figma for the early mockups of the design, CSP (somewhat scuffed replacement to Adobe Illustrator) for the logo, and Git for version control and collaboration. We were able to 'train' models in Cohere using external datasets we found online: one which classifies Twitter tweets as toxic or not, and one that labels political Reddit posts with a particular political alignment. More specifically, we were able to perform text classification using the classify endpoint and semantic search with the nearest neighbour search algorithm. Both methods produce a certain percentage of being 'correct' in regards to how accurate the label they attach to the example/input might be, which is also a statistic we show. For example - and you can try this for yourself - 'bruh' is 79% likely to be used in an offensive manner online (obviously).

# Challenges we ran into
While most of us have some decent experience in frontend and even a little backend development, we had pretty much none in machine learning, NLP, or anything of the sort. Approaching the task was quite daunting at first because we had no idea where to begin. However, as always, documentation soon became our saviour. In fact, it was instrumental in our progress; the tutorials provided got us through most of what we needed to do. Besides that, we also strangely (or perhaps, expectedly) struggled with certain CSS operations. Material-UI having some very oddly documented components certainly did not alleviate any of the pain.

# Accomplishments that we're proud of
We are incredibly proud of our group's accomplishments mainly because we completed most of the goals and features that we wanted to accomplish in a timely manner. We haven't worked together in a LONG time, so working together, first of all, felt very fun. Coming together to work on this and having a live demo to play with made us feel amazing after. We also feel that we were much more prepared to go into this hackathon since this was our third hackathon. We brainstormed before (which then led to catching up and chilling in a call), but we thought of ideas and felt much more excited especially since HTN was in person this year! In the end, we were very proud with our final product since we actually were able to deploy the backend for the first time in a project :)

# What we learned
We learned a lot about Next.js, Express, the Cohere API, and even more about NLP! It was our first exposure to these concepts so working with them and coming out with a product was very exciting. We also learned it's sometimes better to get at least some sleep, rather than none. Also, we got reminded of how annoying CSS can be...

# What's next for Civility
What's next for Civility you may ask? Although most of the tests that we ran have given out somewhat accurate results, we're not done yet. We would love more time to train our models so that results can be even MORE accurate. We also want to provide our users with a personal experience with responses that are more enriching, and also that provides more valuable information that they can't get anywhere else. For instance, more indicators such as race/cultural alignment and text suggestions. Oh yeah, we also want to add a dark mode ;) and expand into the metaverse.
