---
layout: post
title: "A/B Testing in action : Trivago Case Study"
date: 2016-11-12
excerpt: "An introduction to A/B Testing with a focus on real case study on trivago.co.uk website"
tags: [A/B Testing, KPI, Optimization, Web Analytics, Business Intelligence, Trivago]
feature: http://i.imgur.com/BT6dSKb.png
comments: true
---

# WHAT IS A/B TESTING?

It's a testing technique known also as Split or Bucket Testing and based on comparing the performance of the original version of a webpage or app (version A) against its modified or optimized version (version B). These two versions are shown at random to the users, those who interact with version A are the control group and the others form the experiment group. The performance evaluation is made through statistical analysis and measured by metrics known as Key Performance Indicators (KPI) which line up with the company conversion goal.   

> Measuring the performance of a variation (A or B) means measuring the rate at which it converts visitors to goal achievers.

The Conversion goal depends on the business model of the company and the business problem being tackled by A/B Testing. For instance, an e-commerce website wants visitors converting from just visitors to product buyers. Another example would be the case of online services like Spotify for music and LinkedIn as a job board,  these companies would aim to convert free trial users into premium (payant) ones. Measuring the performance of a variation (A or B) means measuring the rate at which it converts visitors to goal achievers.

> We can test for example a webpage layout by changing colors, headlines

A/B Testing can be used with anything related to the user behavior. We can test for example a webpage layout by changing colors, headlines, Call to Action items, Images, etc. Advanced tests can cover also free trial period length or navigation and UX experiences, free or paid delivery, and much more testable items.

To get a deeper understanding of the A/B Testing, I highly recommand the online free course (MOOC) provided by Google on Udacity platform which cover the design and analysis of A/B tests. It covers also how to choose and characterize metrics to evaluate your experiments, how to design an experiment with enough statistical power, how to analyze the results and draw valid conclusions, and how to ensure that the the participants of your experiments are adequately protected.

 <i class="fa fa-graduation-cap" aria-hidden="true">&nbsp;&nbsp;<a href="https://www.udacity.com/course/ab-testing--ud257" target="_blank">A/B Testing by Google on Udacity</a></i>

# Trivago Case Study

Trivago is in fact the company behind one of the most extensive hotel meta search for travellers. There are three sides to trivago: objective hotel price comparison, helpful independent user reviews and interaction in a vibrant travel community. Recently, I read that they're constantly conducting A/B tests on their websites. As a way to observe the A/B testing in action, I tried to find ongoing tests on sites like Trivago.co.uk and think of some tailored KPIs that can go along with their Web Analytics experiments. 

## Find and analyze A/B-tests on our website

The goal behind Trivago's metasearch engine and price comparison website is to monetize the coming organic traffic by increasing the conversion of visits into hotel deals click-outs. While navigating through “trivago.co.uk” using different browsers, I managed to identify the two following A/B tests. 

<b>1-</b> The first test is mainly an aesthetic modification of the hotels’ cells shown as a result of a search. As presented in the figure below, the font color of the highest booking price found for the corresponding hotel has changed from black to red while maintaining the lowest booking price green. A description of the attractive perks provided by the hotel is also added at the bottom.  

<figure>
	<img src="http://i.imgur.com/TwHZMEq.png">
</figure>

The visual modifications in the “B” version are meant to check if the website visitor will be more tempted to click and discover the offer if the highest booking price available in market is not only crossed but also highlighted in red (sign of loss and danger), and if he sees a description of the attractive perks like the sauna for instance. Will these changes push the visitor to notice the lowest booking price found by Trivago engine (added value) which is colored in green as a sign of reliability/positivity? I believe the click-through rate would be a suitable conversion metric for this test while considering positive any click within the hotel cell. 

<b>2-</b> The second test is about a new feature in the website called “Express Booking By Trivago” which I identified by discovering different deals and trying to continue with the booking process. By clicking on the booking site link highlighted in the figure below, on one browser I get the “Express Booking” page and on the other I get redirected immediately to “Amoma.com” which is the source of the deal.

<figure>
	<img src="http://i.imgur.com/Jbfr0Lj.png">
</figure>

<figure>
	<img src="http://i.imgur.com/lB4XVPt.png">
</figure>

 This test’s main objective is to evaluate the impact of “Express Booking” feature on the user in-product booking experience. In the control experience, the visitor gets redirected to the booking site deal where he will find the exact deal he picked on Trivago with the criteria he specified (dates, room type, etc.). He will then decide to proceed with booking or not. In the variation experience, the visitor will continue in the same theme, same user experience thanks to “Express Booking”. The visitor won’t need to get familiar with the booking website to finish the transaction. He will get an exhaustive description of the hotel with photos, possibly change the dates or the number of rooms/travelers, and then pick the room type he wants. Next, he will be able to fill the contact and payment details all without leaving Trivago website. The conversion metric in this case will be the ratio of the number of confirmed bookings generated by the control/variation experience over the total number of visits of the given page. 

## KPIs for analyzing A/B-tests

In addition to the standard KPIs like Bounce Rate and Session Duration, I believe it would be wise to consider the following meaningful and tailored KPIs when conducting A/B tests and evaluating/optimizing the performance of Trivago website:

* __Average Search To Booking Time (ASTBT)__ 

This metric will be used to assess the average duration and the smoothness of the process that starts with the keyword search for hotels/deals and ends with the booking conformation. It’s crucial to take in consideration Trivago metasearch engine speed and usability. It’s also important to see how fluid and intuitive the deal customization and the checkout steps especially with the integration of the “Express Booking” feature. Without this feature, we can average the duration between the search and click-out (getting redirected to the hotel or booking website) instead (Average Search To Click-out Time).

* __Search Abandonment Rate (SAR)__

I insist again on the evaluation of the metasearch engine capabilities, hotel ranking algorithm efficiency and the output layout. The SAR metric will help in tracking the variation of the number of cases where the visitor concludes the search experience without selecting any deal or hotel. A high SAR would be a sign of inappropriate/insufficient search results, bad results ranking strategy, or maybe a weak visual call-to-action.

* __New users’ bookings versus returning users’ bookings__ 

It’s important for Trivago to keep track of the number bookings coming from new visitors as a result of its marketing and potentially traffic acquisition campaigns. This number should be compared to the number of bookings coming from returning users’.  The second number will reflect the performance of Trivago customer loyalty and user retention strategies.  

