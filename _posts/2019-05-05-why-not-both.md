---
layout: post
title:  "Why not both!"
date:   2019-05-05 21:06:00 +0530
categories: thoughts
---

Well, programming languages are super awesome. Yes, there are lots of them and many alternatives to do the same task. But usually, there are only a few that stands up.

Most of the prominent programming languages are imperative. For example Java, C++, C# and python (I know, this is double edge). Recently, functional programming is gaining traction and becoming a trend. But in my opinion, the logic of functional programming is not natural.

In imperative style, we define step by step instructions until we get what we what. But this approach has some unpleasant side effects such as state and mutable variables. Functional programming in the other hand does the exact inverse of this. We first define the last thing we want to do and in order to do that we get it's dependencies next. This goes until all the required steps are done. In order to implement some logic in functional programming we have to think in an unnatural way. But of cause, this style has some shiny things such as not needing to worry about keeping the state, support for immutable variables and higher order functions.

So there's something that we have to sacrifice if we chose one of the sides. But what if we don't. What about the best of both worlds. Is it possible? Well, I think yes. I guess you may have seen the observable pattern, the pattern used in ReactiveX libraries. There we create a pipe which have source which we transform by sending it through a set of operators(functions) until we get the desired output, just like a pipeline. In this pattern, we define operators in imperative style. We don't have to worry about the state between operators by ourselves, doesn't have a limitation immutability and since operators are just higher-order functions we have the shiny stuff of functional programming style too.

Recently I have become more and more interested in this approach and I find it very enjoyable to design and write code this way. If your interested, here is the link to [ReactiveX](http://reactivex.io/).