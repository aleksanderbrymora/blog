---
title: New form of web-browsing.
description: Dev plans for near future
date: 2020-08-25
tags:
  - browser
  - gopher
  - beaker browser
layout: layouts/post.njk
---
## Intro

I read [this article](https://macwright.com/2020/08/22/clean-starts-for-the-web.html) today and it got me thinking about how we consume some parts of the internet. I think I came up with a pretty cool project for myself, but before I get into why this new approach is important, I wanted to mention that one of my favorite dev-things to do is creating software that abstracts hard parts from the user or even dev. And I know it seams off-topic but bear with me.

## Why do you need to hear about my preferences

I'm more of a convention over configuration guy and strongly believe that most of the time we don't need much power over our projects - we simply expect them to work. This is why, when I finally decided to make this blog, I created this page with 11ty, because I knew it would be the fastest one to get into. I chose this framework even though I do enjoy working with Gatsby, or I know i could get the sweet syntax of Svelte. I love the abstraction of getting into projects straight away and the tools being there to help us instead of creating them. That's why I have such a sentiment to rails probably. So where does this come to play when talking about new form of browsing? I feel that we have a good idea about how to create document-like websites (more on that in the article i linked above), but we do it in a unnecessarily complicated way. The way we create the documents physically is nice, don't get me wrong - medium post creation, markdown to html conversion in 11ty or gatsby or plain old post on Facebook. This is a well constructed abstraction. I think there is a step there that is unnecessary - converting to html.

## Why html might not be the best

Before you get the impression that I advocate HTML-bad-dont-use-pls etc, I want to emphasize that I do not think this way. I strongly believe html by itself is great for many reasons:

- it's semantic
- it structures the content into logical parts with (mostly) good names, like `main` or `nav`
- has a top-down flow of information
- it's accessible, at least mostly, by default
- and most importantly it implements links which are the core foundation of the web

The crux though lies in the fact that, I believe, we abandoned some of that these days. Sometimes it's rightly so - we've never had so much power on the web as we do right now. All those applications that run on the web are amazing and I hope they never stop! But there are other parts to the internet, that are more text based - like this post, whole wikipedia, documentation for everything - all of these things are written in overcomplicated technologies, rarely accessible to those who can't program and contribute to some kind of gate-keeping. I get the feeling that we dug a whole so deep that we forgot the true reality and began to create tools to better our situation in that whole,instead of climbing out.

## So what do you suggest..?

I'm just a small human but I believe solutions are already out there and we need to mold them into one cohesive creation to achieve the vision. I believe we need new kind of browser for serving document oriented files, thats focused only on that instead of being a jack of all trades. I also think that the website structure needs to be rethought. We don't need to use html anymore - lets use normal text document that spits out markdown. CSS? We don't need anything custom anymore - provide few styles for different themes with simple selectors (reminiscent of [water.css](https://watercss.kognise.dev/)). It doesn't even have to be normal css - it can be some new clever way of doing this, either through earlier mentioned editor or new language. The beautiful part is that the main selling point of learning languages, which is an ability to go full granular on small behaviors, goes away as all of the structure can be made so simple that there is no point to look at the code. And all of that is just text with predictable, cachable, compressable structure.

## What have you done to make this happen?

Nothing yet sadly. I only got inspired to do it today. I did and will continue to do research on the topic to discover what might be the best way to go about this approach, in the meantime here are my findings

## Inspirations

### [Beaker browser](https://beakerbrowser.com/)

What a wonderful idea this is! I really would like to build this project on top of this browser, but I'm not certain its flexible enough. In any case I would love to implement similar protocol that lets you host your website on your own so I will be definitely keeping a close eye on this project

### [Gopher protocol](https://en.wikipedia.org/wiki/Gopher_%28protocol%29)

A internet protocol that didn't really make it because HTTP became so much more popular, but had a great idea - all of its content was text based. And while now we clearly know this wouldn't be a sustainable way to deliver all of the internet content, as there is more than text that needs to happen, we know for sure that some of the internet could benefit from that. Gopher is a big inspiration and will continue to be one as this project is being modelled after it.