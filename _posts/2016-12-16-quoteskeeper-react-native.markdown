---
layout: post
title:  "Quotes Keeper - react native thoughts"
date:   2016-12-16 12:00:00 +0000
tags: [startup, quoteskeeper, quotes, tech, react]
author: Marek
---

As You already know we’re building one of our OneMonthProject apps using Facebook [React Native](https://facebook.github.io/react-native/) framework. After more than 2 weeks of development, I wanted to share our thoughts about it.

## First, the good parts.
React Native is really easy and straightforward to start with. You can set the project up and start coding in about 5 minutes. Everything is taken care of - XCode project setup, JS environment and templates, simulator, etc. You just run built-in project generator and most of the stuff is done for you.

Second - if you have [React](https://facebook.github.io/react/) experience you’ll feel right at home. Everything is familiar and works almost the same way. Most of the knowledge you have about components, lifecycle, state, props, mixins, etc. can be used in your React Native project. You can use Flux or Redux to manage application state and EventEmitter to notify UI about changes. Just like you would do in regular React app.

There are plenty of libraries ready to be used by your project if any native component is missing. Also calling native code is super-easy. It’s so easy, that in many cases it was faster for me to write simple Objective-C function and call it from JS instead of searching for some library that had it ready.

Now the absolute killer feature - code-test-code cycle. React Native is the best programming environment you can get when building mobile UIs. You can open iPhone simulator next to your code editor and see changes constantly being applied while you edit files. It’s really a pleasure to work with. Every time I need to change native code and re-run the whole app I feel like I’m traveling back to ’90s. Even if you don’t have “hot reload” enabled and need to hit Cmd+R sometimes, it’s still freakin’ great!

There are more nice things about it: performance is great compared to “Hybrid” solutions, building UI that’s compatible with iPad is easy, styling with flex is really nice. But there are also some…

## Parts we didn’t like.
React Native is still young and you can see it in many places. Some properties are missing, even in core components. Documentation is lacking and you often have to dig into framework code to see how something works. Many external libraries still need much work and have nasty bugs. Of course, this is something to be expected from open source project in this early phase, but you need to take it into consideration if your project is large and critical for your company.

Second issue we’ve had is with the performance. Don’t get me wrong. The app is very responsive and probably you won’t have any issues if you’re not displaying very long lists or processing large amounts of data. But if you do, you’re in trouble. JS performance is nowhere near Objective-C code. We started having performance issues with around 2000 objects in the list that we needed to process end filter. Moving it to native code fixed everything. Also built-in React Native list component starts to work slowly when you have so many elements. You really need to test things out if you plan to work on large datasets.
 
## Summary
To sum things up - would I use React Native in my next project? The answer is probably yes. It’s really good and fast. Developer experience is great and what you’re building is a real app, with native look and feel. You’ll have a chance to test it yourselves in [Quotes Keeper](http://quoteskeeper.com).


