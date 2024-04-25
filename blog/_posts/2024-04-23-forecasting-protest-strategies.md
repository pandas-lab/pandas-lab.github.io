---
layout: post
title: "Forecasting Police Strategies During Mass Protest Events"
featured-img: cherry-blossoms-01.jpeg
authors: [bradford]
tags: [machine learning,protest]
---

In a working paper presented to UNC Charlotte's School of Data Science, Dr. Radford evaluates the predictive power of prior protest events to forecast subsequent policing actions. Below are videos of predicted probabilities.

## The Poster

![SDS Poster 2024](/assets/img/posts/SDS_2024_poster_small.png)

<a href="/assets/img/posts/SDS_2024_poster_small.png"> Full size image.</a>

## Police Presence Predictions

<center>
<video muted controls style='border: 1px solid #000;'>
    <source src="/assets/sds_police_2km_2hr.mp4" type="video/mp4">
</video>
</center>

* Upper left: actual observations of police presence.
* Upper right: predictions made with only structural predictors.
* Lower left: predictions made with structural predictors, weather conditions, and time.
* Lower right: predictions made with structural predictors, weather conditions, time, and prior protest-related events.

## Police Vehicle Predictions

<center>
<video muted controls style='border: 1px solid #000;'>
    <source src="/assets/sds_emergency_car_2km_2hr.mp4" type="video/mp4">
</video>
</center>

* Upper left: actual observations of police vehicles.
* Upper right: predictions made with only structural predictors.
* Lower left: predictions made with structural predictors, weather conditions, and time.
* Lower right: predictions made with structural predictors, weather conditions, time, and prior protest-related events.