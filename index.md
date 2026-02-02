---
layout: default
title: Blog
---

# MY OUTREACHY BLOG

Welcome! This is my personal outreachy blog that documents my journey with Outreachy and Mozilla Firefox.

## Introduce Yourself {#introduce-yourself}

*December 07, 2024*

> Hi, I'm Anannya (pronounced uh-NUN-yah).

### WHO I AM

What drives me:
- Working on **real impactful products**
- The intersection where **tech and art meet**
- Thinking about **UX, feelings, and tiny details** while understanding **how everything is wired underneath**

That mix pulled me towards FOSS, [Outreachy](https://www.outreachy.org/), and Firefox.

### WHY OUTREACHY

Reading about [Outreachy's](https://www.outreachy.org/) program description gave me that **"you belong here"** feeling. That was enough to show up, apply, and keep going through all the stages. 

During the contribution period, I got hands-on with Swift and UI Kit while making contributions. My mentors were available, patient, and genuinely helpful. In an environment like that, it's easy to see yourself contributing long term without burning out.

### WHY FIREFOX

I was already experimenting with mobile dev before Outreachy. Firefox felt like a perfect match. Through this internship with [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/), I'm hoping to:
- Learn how impactful apps are designed and shipped
- Find a community of like-minded people 

**What I'll be working on:**

My project focuses on Firefox's native error pages. When I explored the codebase, I found there's a "no internet connection" error page with a cute fox illustration that was disabled. I enabled it and tested it locally. Other errors still fall back to older HTML-based pages with technical wording that can be confusing.

My task is to expand those native error pages to cover common error types. I'll be collaborating with UX and PM teams on clearer designs and their implementation.

**What I've been preparing before the official start:**

- Swift, UIKit and Redux-style state management
- The native error page codebase
- How the existing "no internet" implementation works
- How other browsers (Safari, Chrome, Brave) handle their error pages



### THIS BLOG

This blog is where I'll share short, focused updates about the journey and my progress over time

---

## Learnings Till Now {#learnings-till-now}

*December 22, 2024*

It’s been a really good couple of weeks so far. I’ve been easing into iOS development and trying to properly understand how Redux style state management works like unidirectional data flow, actions, reducers, and why predictable state actually makes a difference once a codebase grows. Along the way, I’ve been getting more familiar with Swift too, especially things like optionals, structs versus classes, and how the iOS lifecycle and data flow fit together. Seeing my changes show up in the Local Fennec build felt really nice, and I’m slowly getting more comfortable finding my way around both the iOS and Firefox codebases. The learning has been genuinely enjoyable, and it feels like something I’d be happy to keep doing


---

## Think About Your Audience {#think-about-your-audience}

*January 05, 2026*

I've been thinking about who I'm actually writing this blog for. At first, I assumed it was "for everyone," but that makes it hard to write anything at all. So I'm picking a few specific audiences and writing with them in my mind:

### Future Me

The version of me a few months from now who probably won't remember the messy parts about:
- how long I overthought about a failed build because of a dependency on another file which was a part of the future PR
- how confusing it felt to juggle multiple PRs that depended on each other
- how I went back and forth between files just to understand one action's flow

I'm writing this so I don't only remember the "merged" state, but also the messy middle like the build order notes, the scratch diagrams, the "what triggers what" scenarios.

### New Contributors / Outreachy Applicants

People who are at that new stage where I was when I started out and want to know my experience and what I'm learning on my way.
- The work isn't just writing code. It's also understanding which PR unblocks which, when to split work, and how to not trap yourself in a dependency loop (still learning).
- Overthinking usually just freezes you. Taking a breath, jotting down the chain of actions, and asking questions works better.
- It's normal to feel like you're "bothering" mentors, but trust me you're not. I got stuck in a PR dependency loop, and my mentor handled it like a solvable problem. That moment shrunk the whole thing down to size.

If you're reading this while trying to send your first patch or open your first PR: the panic when things don't line up in our mind is common. I've been there too.

### Firefox iOS Contributors && Reviewers 

This is me documenting how I'm learning the patterns here.
- how to think in terms of actions, middleware, state, view instead of just a view controller
- how to respect existing patterns and principles and learning about clean code practices
- how build order and PR dependencies affect what is safe to land when

I'm also learning that review isn't just about correctness, it's about keeping the codebase consistent. I'm trying to treat reviews as chances to learn the patterns, not just fix individual lines which might take longer than usual but teaches me a lot.

---

## Mid-Point Progress {#mid-point-progress}

*January 19, 2026*

Halfway through, I’m noticing something that feels like progress in a very specific way... I’m not getting lost as easily anymore.

### What I've been working on

Most of my work has been on the native error page flow, especially certificate-related errors. It's been Redux and UI; making it look right, but also making it behave correctly and predictably.

- Redux integration for error page actions: where actions are dispatched, how middleware handles them, and how to change things without breaking other flows.
- Certificate exception / proceed flow: wiring up the "Proceed (Risky)" action so it works correctly for the current tab.
- Certificate details UI: reusing the existing certificate viewer and making the link open reliably.
- UI polish and consistency: layout in UX, typography via FXFontStyles, colors via theme tokens while keeping the Figma intent

### Stuck to Unstuck moments (and what helped)

Debugging things that looked correct in code but behaved wrong in the app (for example a link not opening or content not scrolling) were confusing. What helped was thinking in terms of system: What input we have? What state we expect? What URLs are being generated? What does the UI need from that state? That moved me to targeted fixes.

### Before & after: certificate error UI

I recorded a short video showing the certificate error flow before and after the changes. It should give a clearer sense of what changed.

<div class="blog-video-wrapper">
 <video class="blog-video" controls>
   <source src="{{ site.baseurl }}/assets/video/before.mov" type="video/quicktime">
   Your browser does not support the video tag.
 </video>
</div>

---

## Career Opportunities {#career-opportunities}

*February 02, 2026*

This section will be updated on *February 02, 2026*

---

## Final Progress {#final-progress}

*March 02, 2026*

This section will be updated on *March 02, 2026*
