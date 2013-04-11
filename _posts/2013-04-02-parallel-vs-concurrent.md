---
layout: post
title: Parallel vs Concurrent
tags: parallelism concurrency algorithms opinions
year: 2013
month: 4
day: 2
published: true
---

Well a lot of people are taking a stab at the parallel vs concurrent
definitions and here is mine. 

Parallel is easier to define. When you have independent tasks which needs
no coordination among them they fall into the category of parallel.
Parallel is in my opinion a subset of concurrent. There is a strict
condition in parallel processing that when things if they  can be run at the same
time they should be. There are different aspect of parallelism as task
parallelism or data parallelism which we will not go into this time. 

We fall into the category concurrent when we start talking about
coordination. Parallel starts with or eventually leads to concurrency at some point of
time for communication and coordination of parallel processors.
Concurrent programming has another aspect which is weaker than parallel
is concurrent is defined as tasks don't have dependency on order of
execution. They could run together, or one after another or in reverse
order and all have the same effect. So concurrent doesn't really make
any promises on how things run just that no dependency.

Well those are my opinion. What are yours?
