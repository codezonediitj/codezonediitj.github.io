---
layout: post
title:  "Inception Bar: A new type of phishing attack."
date:   2019-05-26
author: "Anukriti Jha"
excerpt: "Developer James Fischer recently documented a possible phishing attack which works by masking the URL bar of the Chrome for mobile and show a fake URL instead. This new fake bar has been dubbed as the ‘inception bar’."
image: "/images/pishing.png"
---

Developer James Fischer recently documented a possible phishing attack which works by masking the URL bar of the Chrome for mobile and show a fake URL instead. This new fake bar has been dubbed as the ‘inception bar’.

While scrolling down, Chrome for mobile hides the URL bar to increase the shown content by the webpage. This is the very vulnerability utilized by malicious users who then use a doctored URL bar in it’s place. This fake bar has a padlock and the number of tabs, just like what is present in the real bar.

Making it worse, the fake static URL bar can be made to appear as a dynamic bar with interactive content.

Normally when the user scrolls up, the real bar reappears. But even this can be overcome by making a “scroll jail”. Once Chrome hides the URL bar, one can move the entire contents of the page into the new element with overflow : scroll.

But it gets even worse! Even with the above “scroll jail”, the user should be able to scroll to the top of the jail, at which point Chrome will re-display the URL bar. But one can disable this behavior, too! One insert a very tall padding element at the top of the scroll jail. Then, if the user tries to scroll into the padding, the users would be scrolled back to the start of the content. It looks like a page refresh.

#### The name inception?

“The user thinks they’re scrolling up in the page, but in fact they’re only scrolling up in the scroll jail! Like a dream in Inception, the user believes they’re in their own browser, but they’re actually in a browser within their browser.” - Fischer

#### Is it a real security threat?

Showing the authentic URL of a website, the fake website may prompt users to enter sensitive data like the login credentials and this might lead to a potential phishing act.

Well, even I, as the creator of the inception bar, found myself accidentally using it! So I can imagine this technique fooling users who are less aware of it, and who are less technically literate”, Fisher wrote.

#### Steps to identify the inception bar

So far, there have been no reports of malicious parties exploiting the hack to deal damage. But there are a few measures one can take to protect themselves from the “inception bar' hack:

The only time the user has to verify the true URL of the page is during load time, after that there is not much escape.

While browsing a webpage on Chrome for mobile, lock the screen and then unlock it. Doing so will automatically show the real URL bar that was hidden while scrolling through a webpage. In case the inception bar trickery is at work, users will see two URL bars simultaneously – the real one at the top and the doctored one below it.

Inception bars often display an incorrect number of tabs, so if one keep a check on the number of webpages one has opened in different tabs, the anomaly can be spotted.

One security feature that Chrome can add would be not to completely remove the URL bar by scrolling down, it can display a shadow of the nearly hidden scroll bar.
