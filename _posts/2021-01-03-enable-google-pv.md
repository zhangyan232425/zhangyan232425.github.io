---
title: Enable Google Page Views
author: Dinesh Prasanth Moluguwan Krishnamoorthy
date: 2021-01-03 18:32:00 -0500
categories: [Blogging, Tutorial]
tags: [google analytics, pageviews]
---


This post is to enable Page Views on the [**Chirpy**][chirpy-homepage] theme based blog that you just built. This requires technical knowledge and it's recommended to keep the `google_analytics.pv.*` empty unless you have a good reason. If your website has low traffic, the page views count would discourage you to write more blogs. With that said, let's start with the setup.

## Set up Google Analytics

### Create GA account and property

First, you need to setup your account on Google analytics. While your create your account, you must create your first **Property** as well.

1. Head to <https://analytics.google.com/> and click on **Start Measuring**
2. Enter your desired _Account Name_ and choose the desired checkboxes
3. Enter your desired _Property Name_. This is the name of the tracker project that appears on your Google Analytics dashboard
4. Enter the required information _About your business_
5. Hit _Create_ and accept any license popup to setup your Google Analytics account and create your property


    If the `site.baseurl` is specified, change the first filtering rule to `ga:pagePath=~^/BASE_URL/posts/.*/$`, where `BASE_URL` is the value of `site.baseurl`.

After <kbd>Run Query</kbd>, copy the generated contents of **API Query URI** at the bottom of the page, and fill in the **Encoded URI for the query** of SuperProxy on GAE.


