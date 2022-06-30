---
layout: post
title: #100DaysOfCode Round 2
---

#### I DID IT! I REVERSED A LINKED LIST ON MY OWN WITHOUT LOOKING UP SOLUTIONS!

I made so many mistakes and it took a long time, but the struggle to do it myself was worth the dopamine reward.

During this round of #100DaysOfCode, I've been balancing my time between learning Data Structures and Algorithms and building a personal library app. Recently, I solved a couple of easy leetcode questions about linked lists, but I had do ultimately look up solutions before I got them working. I think this is okay - the general advice I've seen when you're getting started with leetcode is to study solutions until you understand how to do it, and keep doing problems until you recognize the patterns before you need to look up solutions.

That said, I got to one about reversing a linked list and decided I was gonna figure it out on my own using just my notes from the youtube lectures. I'm not worried about optimizing for efficiency (yet), I just want to be able to do it, and I want to figure it out myself.

I ended up doing it in O(n^2) time by removing the last node of the input list and adding it to the end of a new list. I'm sure there's a way to reverse the list in place, but I'll deal with that later. 
 
Some unrelated thoughts:
- At first, the lists I made were circular for some reason - my `addLast` method was aggregating the nodes rather than just adding a new one to the end. 
- I dealt with many iterations of "cannot read property 'next' of null" trying to make my loops work.
- It was good practice writing classes and methods because I don't do that often in my side projects and it's a fundamental concept of OOP and Javascript. 
- I could call this "test driven development" because I wrote my tests first and let those guide my mistakes.
- I got to the point where I could reverse a list with 2 nodes but not 3... turns out I needed to reset the `current` pointer to the head after the first node was removed.
- My implementation doesn't actually solve the leetcode version of the problem because I defined my own `Node` and `LinkedList` classes, but I can probably adapt my solution to solve the leetcode version.

I am proud of learning how to do this and challenging myself to solve it on my own. I'm glad I took the time to celebrate my success because I've been pretty frustrated with some other things and this is a nice win for me, but of course now there's so much more to do. It's time to jump back into my book app!
