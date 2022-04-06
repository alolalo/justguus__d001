---
title: "WIP: BOUM"
date: 2022-04-06T07:31:06.850Z
author: Guus "mr Bot" Hoeve
summary: >+
  Documenting my thoughts and work on writing out the naming convention by hand
  first, not in code first. The key to making a naming convention is to make
  it's narrative, that has to have some functional aspects to it's semantics so
  it can be applied from a sense of applied narrative.

tags:
  - post
---
This is why you will see far less code examples than you might think, because that's the whole point about .: B.O.U.~M :. , it's a semantical and fractal pattern that you should be able to "just speak about". Not like code at all, because that's how code works; it's a computer science narrative.

# A skeletal & semantical design system for design tokens.

BOUM is the successor to a naming-convention I dropped a year ago called Base Plus Minus, just before lock-down, at React Conference in AMS 2020. It was/is a love-project: a side-project that doesn’t let go.

It changed how I looked at using CSS-variables in conjunction with **accessibility** for developers. A forgotten part of DX, to check our own six on that matter and to make our own work accessible for peers too.

The talk I gave got lots of positive reception, people really like the fact design tokens could solve the accessibility issue of color upfront. At that time I thought that's why they liked the concept, because it fixed accessibility.

But it could only do that; do colors and it was intended to be applied universally to all kinds of things. Using a relative token syntax that is just a simple concept of going up or down an elevator with floors, it means people narrative.

The implementation however is one 

If anyone remembers my talk in Base Plus Minus, Hello again! My name is [Gu.us](http://gu.us) if you remember, and if you have any questions about what you're about to read; just askgu.us. 

I'm a chef, a designer, a serious gamer, a developer, a poly-skilled individual who loves to ruin problems by design. I like to keep design as salient, accessible and do-able as possible. Minimal fluff.

The problem I’m going to ruin in my very first dev-ops oriented article, is actually a very common one: creating a naming convention that scales uniformly, semantically & systematically.

Creating your own naming-convention makes you really humble. It's like you need to create the 5th cascade, the one that goes outside of the scope and into the mind of the development experience. Because before any product reaches any customer, your peers are your customers. UX == DX.

# Thinking is perception

I hope my learnings on perception & linguistics will make a difference for the better of creating a universal token convention, without the overhead. Language is a technology of your perception, and naming things in a system is allocating a place for it by giving it a relative "word of image".

A narrative, a very powerful one too.

By giving you the placeholder character in the middle, BOU and the base can adapt to anything you throw at it and using a simple rule: **1st-letter replacement**. This rule is also a class in CSS, which makes it also applicable to itself should you choose to document BOU in your DS automagically.

I opt not to, for good reasons; BOU is made to memorize. Start on Monday, master on Friday.

So lets say I have --brand-primary, I can choose to use **p**rimary as replacement and ramp tokens on primary, and under primary. The BASE is always a word, the tokens on or under use **1st letter** abbreviation as a replacement of '**base**' in the middle;

```css
--brand-op3: hsl(120, 50%, 85%),
--brand-op2: hsl(120, 50%, 75%),
--brand-op1: hsl(120, 50%, 65%),
--brand-primary: hsl(120, 50%, 50%),
--brand-up1: hsl(120, 50%, 40%),
--brand-up2: hsl(120, 50%, 30%),
--brand-up3: hsl(120, 50%, 20%),
```

I really like to write it out as such: the semantical parent in the middle as the silent base, siblings nicely surrounding it with the 1st letter as reference. Very legiable and memorable to abbreviate still using the on and under naming like it was never out of place. It's also a good test-pattern post.

You might technically be forced to write out brand-primary-base (generated). That is easy to fix with BOU: just use base as an appending replacement that you can apply one Sass-function to all your globals such as colors to generate a ramp, and write automated test that look for specific tokens.

```css
--brand-primary-ob3: hsl(120, 50%, 85%),
--brand-primary-ob2: hsl(120, 50%, 75%),
--brand-primary-ob1: hsl(120, 50%, 65%),
--brand-primary-base: hsl(120, 50%, 50%),
--brand-primary-ub1: hsl(120, 50%, 40%),
--brand-primary-ub2: hsl(120, 50%, 30%),
--brand-primary-ub3: hsl(120, 50%, 20%),
```

BOU can cover those stories for you, weather you are just starting out with an IDE and writing your first assignments for school, or if you need to implement this into serious build and testing tools. Shouldn't matter and that's what makes it shine and scale based on your needs right now.

A **skeletal design system** is my answer, perfect for customization by standardization of structure, NOT surface; that's just one simple variable that you can tweak to your heart's desire with just on css-variable to change the hue for example;

```css
--h: 120,
--brand-primary-ob3: hsl(var(--h), 50%, 85%),
--brand-primary-ob2: hsl(var(--h), 50%, 75%),
--brand-primary-ob1: hsl(var(--h), 50%, 65%),
--brand-primary-base: hsl(var(--h), 50%, 50%),
--brand-primary-ub1: hsl(var(--h), 50%, 40%),
--brand-primary-ub2: hsl(var(--h), 50%, 30%),
--brand-primary-ub3: hsl(var(--h), 50%, 20%),
```

DRY-ing out your design tokens is really showing progressive enhancement of your system, graceful decay as a result with zero friction. It shouldn't feel like adoption, it should feel like liberation of a voice you didn't have before; the one to name your tokens with.

You might also go a bit more dynamic on what primary actually is using internally. Some great write-ups have already been made on what you can do with variables with clamp(), calc() and minmax(), and BOU is perfect for those use-cases imo. I say give it a try, too hard for me right now. 

BOU works for pretty much anything you would throw at it; your color-scale, typographic-scale, spacing-scale, grid-scale, media-scale, fluid-scale, minmax-scale, clamp-scale... Pretty much any ramp imo, but that is not the real issue of creating a convention: 

I love keeping things basic and BOU will live and die by that simple standard. Refactoring feels like Botox, another filler that makes things look good for some, and leaves many behind by killing all the options for you. I hope you see BOU is an open standard, a skeletal design system. No face or colonial fiction of the perfect system. Just the perfect structure to support that.

Making things very simple and basic feels like I got a voice back to now communicate my design decisions in a systematical and semantical correct way, without learning. No docs needed, no npm-install, no repo to fork. Just case-studies and write-ups to read about IRL-cases I need to research.

## All your contrast belongs to A11Y

One of the little details of the new color-contrast() I don't like for that fact; it has the same wonky AAA-accessibility checks with rigid values to check for contrast. No way they let you set your own variables and values for each, we must follow the hurd of A11Y and use their values! Why?!?

People always have to look up those values, they only check technical color-contrast and not IRL perceptual color-contrast where a font's weight will render characters much lighter, yet your test will say "PASS" because it just check colors. 

Really depressing to see the most prestigious people praise A11Y but never really question it's obsolete practices and technical excellence. I'm not here to judge that, I'm here to destroy that incredibly inaccessible development experience they create, and the wake of tools that support it.

I really don't like those handicaps in my DX cause by other people's choices, and in the end your UX will suffer for accessibility-tooling NOT being made accessible for engineers tbs. We really need that first or we can't pass it down the line properly. The hito-zukuri is more important than the mono-zukuri of the making of things. Language is technology, remember? People first.

Leading Industry standardization & colonial unification in search of one language to rule us all is the problem. And I'm here to say no to that, partially. Indies always know best, you know that. They just break the glass ceiling and show you can't manage to get people three variables to control since they don't control them themselves properly;

AA: ratio of 4.5:1
AA-Large: ratio 7:1
AAA: 7:1
AAA-Large: 4.5:1... 😷

# The Three Scales and the Five Planes

We want in instant-noodle design systems these days and just add hot water themes, but forget to know how to make that ourselves or to know where the resources of our design-food came from.

The eco-system is out of sight, the label and the language took over the conversation. Speed is a deadly weapon to silence a majority, and mean and fragile we have become to become self-learning and reliant again on our own strengths of system masters, the new web-masters.

Naming conventions in design systems have quite some legacy syntax to define scales, like t-shirt sizing, relative sizing like clamp or min-max, numerical ones like you see in Tailwind and Material Design, and use quite some cosmetics to describe the same thing; objects on a ramp of relationships.

To my knowledge there are currently only three adopted conventions for ramping tokens, and these concepts are universal through any system design you find in real life (clothing, screws, metric units, etc..). I'm not going to re-invent that, a new metric unit. No I'm pointing to how we refer to such things with those units since we don't know any other units to describe the relationship;

- font-weight-**300** //numerical order
- font-weight-**thin** //semantical order
- font-weight-**xl** // sizing order

But I would like to **introduce a new form** that I see more and more these days; skeletal scales and tokens that are agnostic in presentation (cosmetics) but clear in application and relationship;

- font-weight-**base** // skeletal order

It's a this exact kind of definiton to describe the purpose of BOUW too; it's a skeletal naming convention to give structure and meaning to the surface-naming of your convention to begin with, especially if you're into using calc(), clamp() for more parametric & dynamic styling of your content.

## Meta, Micro, Maxi, Macro

BOUW has such a simple premise that the entire convention has a few principles to restrict it from ever getting in the hands of BS, and making a few statements on some core principles;

1. **No docs, Strictly Principles (***meta -zukuri***)**. BOU will only have case-study write-ups using it, keeping it as relevant as the last case treated with the convention. Submission are wellcome to the repo AwesomeBOUWwerk which collects all known articles & systems using BOUW.
2. **One Form, Function & Fiction (***mono-zukuri***)**. BOU keeps things simple and *anti-fragile*; the symmetrical sibling of minimal that is about first principles that are simple unbreakable by design. **B**ase **O**n, **U**nder, **W**ith is the only documentation of the syntax. Comments are key!
3. **S.A.D. Principle (***hito-zukuri***)**. "Keep it Salient, Accessible & Do-able", where salient means instinctively clear like a door-handle. BOUW is instantly clear and do-able for peers & people who wish to "bouw" a system themselves and need a skeletal design system to support them.
4. The Meerloo Principle (meso-zukuri). **Logic can be met with Logic, while illogic cannot.** While we all tend to practice what we preach, it is mere words that make up BOUW. Therefor the language that it speaks must be logical, something we practice, proof and preach, so it can be translated logically if it's illogical tbw. That's "Rape of the Mind" to begin with.

## System Design vs Design System

We often don’t realize how much effort went into actually naming some properties that are specced into our everyday lives, but in tech we have not found a system of it’s own nature to name things. We do not have a design system for naming things in design systems.

The technical perception of system rules your thinking here, not your first-person perception, because it defines the structure. Yet even if it looks technical perfect, practically it is far from since we constantly need to explain people what all of it actually does and means. 

They can’t “see the system” or read the language, and what they want is restricted by inception. And we all adapt to technology so easily, our thumbs are the proof. Is that by design system, or system design? Did we evolve or did we devolve because of the system adoption?

Do you study medicine or healthcare? Because design systems are the medicine we often prescribe to our patients, making them reliant by the system design of how they are perceived. A kind of paradox leadership without a head that sees what you see. They just invent your role.

We don’t rethink our tech and see that language is a technology we must all use to project our ideas consistently without restrictions. And that’s why thinking in systems is really hard, especially new kinds of words of image. 

And guess what, our docu-fallacy makes us create docs for things that don't explain themselves. Every design system has a documentation site on what it has under the hood, some code examples, but mostly lots of words explaining complex abbreviated terminology only coders can read.

I'm also the type that says if you bitch about it, then just fork it and fix it.

So as a good samaritan, I'm using an IRL design system as a use-case: Feo.css by Kevin Pennekamp, a (as decribed) front-end lover and coder who I chat with on Twitter, and has an issue naming and explaining his design system naming-convention, or the choices behind them.

A very normal, regular thing to encounter; a naming-convention that needs a doc and a person to explain what it means. That's not your fault, that's legacy fallacy of Mary's Room; we literally see our system in code, but we write a doc? We need docs right? ...... WRONG! 

## Mary’s Macro Mania

Design systems are in a state of Mary’s Room, and most of us are seeing it’s colors for the first time. We need more open systems that need less control, more autonomy and user generated content.

Tailwind is often under a lot of backlash, wrongfully imo, for creating a design system framework that enforces their way of working on “pure developers”, but the reality of the matter that the conflict comes from a social aspect yet they blame it on the framework’s adoption and methodology not akin to theirs.

The social aspect I see is actually very simple: it doesn’t give you a framework, it gives you a naming-convention standard you have to adopt as the utility-first JIT build-tools demand it since that's what it was designed for.

But that’s mostly it; I imagine a beautiful can-do-it-all system yet in reality I created more of a ‘npm design’ function and just dumped all kinds of cool tricks in my CSS codebase, and need not to worry about them: comes with a JIT cleaning-service for the 1000’s I don’t use.

Base Plus Minus, and BOU too, are therefor thoroughly de-languaged from my subjective viewpoints on “best industry practices”. It is not a design system framework, it is a skeletal design system for when you are creating your own custom design system framework and need a S.O.L.I.D. language.

As a "state of design systems" we simply are trying to take a black-hole picture every year of what it really should look like, a by the confirmation-bias and social bubbles we see other peers & pros their “flagship system”. 

Lots of sailors on deck, huge shiny guns, everyone happy and raving that someone made a google-doc that is strictly kept private for the sake of "governance & consistency". One system to rule all.

Mostly fueled by large corporations, these kind of practices are not akin to my natural bold transparency and clear "Dutch hospitality" in communication. I have a sense for psychology and bullshit, and when people hide behind flash-bang politics and big names, the bigger the bubble.

## Docufalacy, Legacy Fallacy, Innovation Paradox

The ironic truth of life happens often when we focus on creating a "design system"; focus less on your design system and your system design becomes clear. The real technology is language or this industry wouldn’t be called IT; information technology, and language IS A TECHNOLOGY.

Seriously, BOUW could very well be the best design system I (n)ever made, since it only lives in **no-code**, not in a doc, so it always has living documentation, and living people using and writing about it. It keeps the pencils sharp, and the use-cases creative, the proof consistent and relevant.

In hindsight, the design of BOUW as little as it seems at first, showed me how incredibly delicate the difference is of having a uniform system taking things over. Overtaking your natural language to express logical cause and effect. What’s the point to that, speaking French al of a sudden, if it just makes us feel smarter? That's conceptual colonialism of supremacy, we know that doesn't work.

Why? Because a systemic change on that level cascades down all departments, including it’s problems you don’t see. Shit in, shit out. And I really check my perceptions from a lot of angles.

I monitor that kind of things with myself by no means of methodology or practice: I just kinda feel there is something out of balance, especially when people can’t put it in words yet feel the frustration. Most likely you're hitting the same glass sealing Elon is trying to solve; logical language.

Can I be an artist here, please? That’s forgotten, the lost art of developing the answers for our creative language. TLA’s , KPI’s, OKR’s have replaced our naming convention of quality, speed the new sanity. I take it very, very slow because I see that goes at light-speed the second it clicks.

We all see things our own way so I say your naming convention should definitely support that; communication of perceptual application; a no-brainer that doesn’t need documentation, OK!?.