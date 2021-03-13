---
title: Hurricane Track Prediction
excerpt: This project focuses on the problem of predicting the track of hurricanes using satellite imagery data accessed via AWS. I implement a Tensorflow multi-input, mixed type model (imagery plus numeric data) using the tf.data API to do automated feature engineering on the data pipeline.
permalink: /hurricanes/
image: hurricanes.jpg
background-image: hurricanes.jpg
---

<hr />

2/28/2021 Update: I have recently returned to this project to make use of NOAA's Big Data Project's offerings on both AWS and GCP, which weren't available when I started the series. Please check out the "2021 update" folder and included code / notebooks, located [here](https://github.com/M00NSH0T/Hurricanes/tree/master/2021%20update). This is probably the best place to look if you're trying to get a quick sense of how I work, but for a more extended view into the way I break broblems down and go about solving them, you should check out my YouTube series and the associated code. Much of this predates my big switch over to using Jupyter Lab / PyCharm, but there's also a lot I go into here regarding the work we all have to do before we every write a line of code, such as doing research into data, what others are currently doing to solve the problem, brainstorming of new approaches, and planning of what experiemental prototypes to spend our time building. This previous work also goes into building a SQL Database, encoding massive datasets with a multidimensional autoencoder, and uses a couple very different model types types to solve the problem in different ways, such as an LSTM and a GAN.

Far too many tutorials on using Machine Learning (ML) out there make it seem like your whole job is just taking a nice pre-processed dataset that you were simply given and running it through the latest algorithm of the week, like you find on Kaggle. And the job title "Data Scientist" has been used to label pretty much anyone working with Machine Learning or even basic statistics these days. Many don't realize that building a system, testing its performance, making tweaks to it and retesting is in fact a closer description of the core engineering design process than the scientific method. Applying research to design new systems that meet a specific set of requirements is engineering, not science. However, people with the title "Machine Learning Engineer" are rarely the ones designing the neural network or even the feature engineering. Companies continue to label the architects of prototype solutions "Data Scientists," which I sort of see as a misnomer, leading to confusion in terms of how to go about solving these sorts of problems, and ultimately part of the reason why I think so many "AI" initiatives fail. People with expertise in tensorflow are often hired on as either "Data Scientists" and given vague goals with fuzzy timelines, or brought on as "Machine Learning Engineers" to take the random successful projects of those Data Scientists and scale them up. There are taught to follow very basic steps to apply ML to problems, such as "clean the data, test these different approaches, etc." There's far too little focus on how to think about the problem at a more abstract level and find new datasets, or perform rigorous feature engineering (such as feature crosses) to handle non-linearities better. If more companies viewed Machine Learning as a tool that could be used to achieve a set of specific objectives, and then hired engineers to come in and apply that tool to that objective while meeting a set of clearly defined requirements, there would be a lot more success. 


{% include post_picwrap.html pos="left" src="/images/Slide9.JPG" %}

This series attempts to teach you how to do some of that, at least as much as something as short as a YouTube series ultimately can. I use the "core engineering design process" to tackle a problem using Machine Learning and raw, uncleaned data. This process is used effectively by all disciplines of engineering, from mechanical and chemical to electrical and computer. Following this is how we figure out what precise problem needs to be solved, define our design requirements, research existing solutions to figure out what's been done and how we might be able to improve it or apply it in a different way, and then design a solution that will actually solve the problem. Randomly grabbing a dataset and trying a million things with it might get you a usable solution as well (and on the surface sounds like it fits the old "fail fast and fail often" philosophy of Silicon Valley startups), but following the engineering design process will ensure that you maintain a bigger picture strategy that will likely bring you to a more creative and interesting solution that works far better in the end. And ultimately, this is what many of those tech startups are actually doing, at least the successful ones. There's a lot of work that has to get done to set up the design/build phase, but once that happens, we build prototype after prototype... iterating and honing in on the a final design until our performance metrics reach the desired levels. This process more than anything else is the reason why our technology has seen such a drastic increase in the rate of improvement over the past hundred years.



So that's what this series is all about... applying the engineering design process to solve big problems with the coolest new tools. And we're starting off with hurricanes. If you're interested in getting your hands dirty with me as we apply this process to the problem of forecasting hurricanes using machine learning, strap in and subscribe. 

The series will follow the steps of the engineering design process. The result will likely be that some episodes will be longer than others, but I think this approach as a whole will convey the intent of the series better. Below are quick links to each video in the series, but to get notified of new episodes, you'll need to subscribe via YouTube. Also, be sure to checkout the associated GitHub site: https://github.com/M00NSH0T/Hurricanes

## Episode 1: Introduction
{% include post_youtube.html id="GDVal32IUxk" %}

## Episode 2: Problem Definition
{% include post_youtube.html id="jcNjHr140I4" %}

## Episode 3: Concept Generation
{% include post_youtube.html id="BdIfuKNIyFk" %}

## Episode 4: Selecting Our Best Idea (1/2)
{% include post_youtube.html id="qhQqmGt_Z7E" %}

## Episode 5: Selecting Our Best Idea (2/2)
{% include post_youtube.html id="d9SurPxW2u8" %}

## Episode 6: Preliminary Design
{% include post_youtube.html id="xE7zi2oLnek" %}
