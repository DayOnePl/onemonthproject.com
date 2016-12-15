---
layout: post
title:  "Life Left - why native?"
date:   2016-12-15 12:00:00 +0000
tags: [startup, lifeleft]
author: Bartek
---

Hi there, 

we haven’t written for quite long - we’re just working hard on our apps. By now, you should know that we’re creating [Quotes Keeper](http://quoteskeeper.com) using [React Native](http://www.onemonthproject.com/2016/12/07/quoteskeeper-react-native.html). I hope you remember that we are also creating micro journaling app - [Life Left](http://www.onemonthproject.com/2016/12/02/lifeleft.html).  We decided that Life Left is going to be created natively for iOS. Why have we chosen two different approaches to developing mobile apps?

Firstly, we decided to create Life Left only for iOS for now. At the beginning, we didn’t want to develop this app for Android. Thus, a native solution is a quite straightforward decision. The biggest promise of React Native is the ability to enable web developers easily step into mobile development, but also create a solution for both iOS and Android with minimal difference. 

Secondly, we want to have the possibility to compare both approaches of development. Since we are implementing multiple apps simultaneously, we can observe how both approaches differ. Even without real life experience, we can see many differences - starting with language and tooling. Still, the biggest difference is the philosophy of creating UI. We want to analyze that in real projects, not just “hello world” examples.

Of course, we’ve selected to use Swift for native iOS development and we’ll be using version 3. We’re going to support iOS 9 and 10. As measured by App Store in 27.11.2016, 63% of users is running iOS 10 and 29% is using iOS 9. That’s why we decided not to support remaining 8% of users. Naturally, that’s much better situation compared to Android version defragmentation, so that choice was quite easy. 

Eat broccoli & workout,

Bartek
