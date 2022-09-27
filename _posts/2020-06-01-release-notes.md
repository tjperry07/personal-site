---
layout: post
title:  "Thinking about release notes"
permalink: /thinking-about-release-notes
image: "assets/images/release.png"
description: Describes release notes, what to consider when creating release notes and release notes design."
categories: [ Technical Writing ]
tags: [ Release Notes, Changelog ]
comments: false
---

Release notes, changelog whatever you want to call them, is a critical way to communicate with customers. I'll attempt to define what release notes are, the content and who should write them. 

## What are release notes?

Release notes or changelog is a way to inform your users of changes to your product. The product changes can include changes to the API, updates to the documentation, bug fixes, UI (User Interface) changes, anything that has changed with the product. 

## Formating release notes

* Keep them short but informative.
* Include date and version number (if applicable).
* Break them up into sections with headings to make them easier to browse.
* Add links to direct readers to any supporting content.

## Release notes content

What should your release notes contain? A good guideline to follow is:

* **Enhancements** - Changes or updates to features that already exist and improve the user experience. Try to detail how it will help them.
* **Bug Fixes** - Problems with the platform that were fixed. Mention the issue and the fix. 
* **New Features** - Anything new added to the product. Provide some details to help drive engagement. Remember, the release notes should be short and informative; this is an excellent place to link to a blog post about the new feature. 

![Slack Windows Release Notes](assets/images/release_notes_slack.png "Slack Windows Release Notes https://slack.com/release-notes/windows")

## Release notes design

Designing your release notes might be the hardest part. They need to be apart of the product, but what else can you add to make the experience better?

* **Filters** - Filters can let users narrow down the release notes to the information they need. 
* **Tags** - Tags are a great way to let users know what's in this release. For example, adding tags for API or product name makes it easier to scan the page. 
* **Pinned posts** - Pin a release note if it's something they need to know. Urgent bug fixes and product deprecation is an excellent place for this information. 
* **Subscriptions** - Readers should be able to opt-in and out of receiving release notes notifications. If you are not going to send an email digest, using a simple subscription to alert that release notes are available is another way to go. 
<br>

![Shopify Developer Release Notes](assets/images/release-notes-shopify.png "Shopify Developer Release Notes https://shopify.dev/changelog")

## Multi-channel releases

Appcues ([https://www.appcues.com/blog/release-notes-examples](https://www.appcues.com/blog/release-notes-examples)) has a great article where they detail the places your release notes should live. 

> * **Email**—re-engage users and encourage them to log back in to check out what's new
> * **App Store**—this is your elevator pitch to entice new users and get existing users excited about new features
> * **Blog posts**—more real estate for releases that deserve more copy or explanation
> * **Social media**—great way to spotlight single features and built hype
> * **In-app messaging**—timely, contextual, and can be targeted to specific users

While I agree with the list, it details more on how you should release features and not the notes themselves. A multi-channel release can be great if it's a new feature is released, and it needs a lot of marketing behind it, or there was a significant bug that was fixed. All of these work together with the release notes to announce changes. I'll go into detail on a few of these. 

### Email

Email is a common way to complement release notes. They usually have an abridged version of the most significant changes with a link that directs back to the full set of notes. If you are a company that has frequent releases, it may make more sense to package them and send them on a regular schedule. 

### In-app

Notifying your users directly of changes in the app is another way to make sure the release notes get seen. 

To refine the in-app releases further, you can split your release notes into two categories; in-app and technical. 
In-app releases will detail changes that directly impact the UI. They don't mention changes to the codebase or API. Include a link that directs them to the technical release notes to see everything. Technical release notes include all modifications to the product. It should detail UI and API changes. Using in-app allows you to provide information that is directly relevant to their experience without adding information they might not want to know. 


## Questions to ask

Before creating your release notes, you should think about the following questions:

* Who is my audience?
* Are they more technical, or do they prefer less technical jargon?
* Where do we usually communicate with customers?
    * Research your page views and email opens. Where does it make sense to announce product changes? Would they work better as an in-product notification?
* How many products need release notes?
    * Does it make sense to have them all on one page with a filter or each product have their release page?
* What should accompany the release notes?
    * Does the release need a blog post or in-app notification?
* How much should I include in the release notes?
    * Does every single change need a release note or should I filter out the less significant information?   

## Resources

* [https://www.appcues.com/blog/release-notes-examples](https://www.appcues.com/blog/release-notes-examples)
* [https://uxdesign.cc/the-art-of-writing-great-release-notes-6607e22efae1?gi=48efdf31d336](https://uxdesign.cc/the-art-of-writing-great-release-notes-6607e22efae1?gi=48efdf31d336)

Todays cover by: Icons made by <a href="https://www.flaticon.com/authors/smashicons" title="Smashicons">Smashicons</a> from <a href="https://www.flaticon.com/" title="Flaticon"> www.flaticon.com</a>