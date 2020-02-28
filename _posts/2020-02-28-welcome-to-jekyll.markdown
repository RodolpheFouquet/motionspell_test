---
layout: post
title:  "The secret about hidden software costs"
date:   2020-02-05 17:36:56 +0100
categories: blog
author: Romain Bouqueau
---
*An essay on how to keep your development projects under control*

# Introduction
**I’d like to share a secret with you**: there is nothing like a custom software suited to \*your\* need.

At first it may seem a paradox considering our company licenses its software. Moreover we have heavily pushed toward the use of frameworks such as [Signals](https://www.gpac-licensing.com/signals) or [Filters](https://github.com/gpac/gpac/wiki/Filters). Frameworks are marketed as the paragon of reusable components. I will show you why it is not and where to draw the line.

# The acceptance and use of third-party software
**Using third-party closed software to perform your core business is not ok.** It is never ok to let the control your business value be in external hands. What happens when your provider raises prices? Wouldn’t it be a threat if this third-party knew your market and users better than you do? On the other hand **using third-party software to execute tasks that are out of your added value is perfectly fine.**

**The main technical issue with third-parties is maintenance.** Either 1) you don’t have access to the source code or 2) you don’t have and don’t want to have the knowledge (the reason why you decided to use a third-party). But when it comes to supporting your customers you should always have the control over the product you ship. At GPAC Licensing we provide both the source code and some professional support to put chances on the right side.

This lack of control over third party software leads to under-optimal decisions such as: refusing third-parties, being too dependent to the external parties, developing a clone of the third-party, … We will see how this vision harms in the long term.

# Re-using code
**Business-wise it perfectly makes sense to reuse resources.** However code duplication is seen as an engineering failure. The reality is more mixed.

There is no code that can cover all the use-cases and stay clean. Let’s take an example: my customer wants to stream MPEG-DASH. The good news is that in GPAC we have a MPEG-DASH streamer. While digging into the customer’s use-case we discover that we need to introduce custom modification to our code. We have to choose between increased complexity versus code duplication (we could mix both).

What is the right granularity for code duplication? According to [leading experts](http://www.pathsensitive.com/), duplication of code is ok but duplication of final user problem solving is not.

# The myth of the universal framework
**The harm comes from the belief in a single solution for all problems.** For example (as of 2019) [React](https://en.wikipedia.org/wiki/React_(web_framework)) strives for writing UIs on both Web and Mobiles platforms. Some developers know React and think React. When a problem cannot be solved using React, they will hack React to meet their ends. These developers need to think out of the box. Building [your own React is not hard ](https://pomb.us/build-your-own-react/) but it requires some curiosity to get there.

Developers need to use the right tools. Hard problems often involve a deep understanding of that problem. There is a phase of mastery. At GPAC Licensing we have a team of experts who master the media tech field.

# Drawing the acceptability line for external dependencies
A framework like [Signals](https://www.gpac-licensing.com/signals) doesn’t address your business challenges. In fact it doesn’t address any of the media challenges. [Signals](https://www.gpac-licensing.com/signals) addresses structural issues of multimedia programs (e.g. concurrency, memory control, metadata transmission, …) but none of your business logic.

In fact the force of [Signals](https://www.gpac-licensing.com/signals) is to let you assemble our bricks and your bricks, with your logic, inside an application. [Signals](https://www.gpac-licensing.com/signals) addresses 90% of our customers’ business cases but sometimes it doesn’t: [Signals](https://www.gpac-licensing.com/signals) is not a religion and we sometimes rewrite code from scratch.

# Solution
**Every use-case is different.** Focus on your customer needs.

First of all, always work with providers or contractors who are open and agile in their methodologies. You want them to deliver early and redeliver fast. In our opinion [Test-Driven Development](https://en.wikipedia.org/wiki/Test-driven_development) (TDD) is a game changer.

Don’t save on using a software architect for your need. Invest in key people who will [understand your business need](https://blog.pragmaticengineer.com/the-product-minded-engineer/).

The acceptance for external code must be driven by the business. If you want to make an experiment in your code, or if you are a small business and want to stay focus, it is perfectly acceptable to rely on a third-party code. If you plan to build your whole product and team around a bootstrapped project, invest in an architect and a product owner, and ask for a solution suited to your need.

In any case our team is here to help and accommodate with your needs. Just contact us as many companies already did.

*The GPAC Licensing team*