---
layout: post
title: Big progress on the flashcard app.
---

Since the beginning of January I've been working on a flashcard app to help myself study computer science and programming concepts. Today feels like a major milestone in its developement. First, how I got here!

## Some Background

I wanted to build a full-stack app on my own that would also help me solidify everything I am learning. I also wanted to learn some new technologies that I wasn't exposed to on my bootcamp that I kept seeing in jop posts. As I've been building it, I've also been applying for jobs, doing practice problems, and reinforcing my javascript fundamentals, so progress has been slow, but consistent.

I chose the PERN stack - PostgreSQL, Express, React, and Node. Prior to this I had the barest of exposure to everything but Express, to which I had none, so before I got started I followed some of a tutorial to learn the basics of React, and a quick PERN stack tutorial to get the gist of how all the parts fit together.

The PERN stack tutorial was about 1.5 hours long, but it took me a week! It was a couple years old so I had to debug some version incompatibilites, and I learned a lot about CORS as I struggled through CORS errors on my local environment. Frustrating, but worth the work.

I started by building the back end, which went pretty well! I actually love SQL so working in PostgreSQL just meant I had to learn the quirks of the syntax, but setting up the database went smoothly. After that I built my routes, which proved complicated because I was using two related tables, versus just the one that was used in the tutorial I watched.

When I started building the front end, I had to go learn more about React before I was ready, so I did another tutorial and studyied the docs a bit, which took a while. Learning React has been it's own journey, and I'm still at the beginning of it - it probably deserves its own blog post.

## Recent Success

The step I was most scared of came last week, when it was time to connect the front and back ends. After a whole lot of trial and error and a lot of studying how to use the `fetch()` method, I finally got the question topic and question text rendered. I stopped to celebrate!

Today, it was time to make the buttons work. I had to figure out how to implement `fetch` on a button click. The challenge wasn't the button click, it was WHERE to put the fetch method.

A common experience I've had when solving code problems or trying too build something is that the actual solution is a lot more simple than I expected. The same was true here! Once I figured how how to make the buttons display the right thing, there were actually a lot of pieces I had put into place that I didn't need anymore, so my code become significantly cleaner once I figured it out.

This felt SO good.

<video width="640" height="420" controls>
  <source src="../images/flashcard_app-basic.mp4" type="video/mp4">
</video>

And now there is SO much more to do!
