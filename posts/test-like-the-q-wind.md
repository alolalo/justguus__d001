---
title: Test like the Q-wind!
date: 2022-04-08T10:33:53.481Z
author: Guus "mr Bot" Hoeve
summary: A single responsibility test-utility, using only ONE css variable; var(--q);
metaDescription: "Q-wind is an experimental approach to testing using one single
  variable to test everything. "
tags:
  - CSS
  - DS
  - DX
---
## Time to lock, load & ship some DS

Hi there! I'm making my first ever "dutch design system" called Q-wind. 

It uses only **ONE** CSS variable; `var(--q)`

It only has one purpose; **testing in pre-production.** Although I found it very handy to learn more on how layouts are actually stacked in the browser.

My writing-style is very direct, so here we go; some key terminology, the full code, then the break-down

# Revolver-DS

Revolver-DS has a simple premise;

Simply *lock* in all your design tokens, *Load* in your layers & utilities, and *Ship* away your custom classes. 

It's a methodology that I created to explain how I think and work in **non-destructive** layering, and give each layer a specific purpose to separate concerns upfront. 

I hope to show you how I applied that to Q-wind, and to not confuse it with any form of atomic design or IT-CSS. I do not need to borrow anyone else's concept to explain a simple concept of threes (+1).

## Qwind.css

## Lock.css

## Load.css

## Ship.css

# Goodbye, and Hello Guus!

Hi, I'm justgu.us and this is my attempt at shaking up and waking up some designers & developers, *especially* copywriters too, to practice some "new CSS" because... 

I'm writing my blogposts in reverse-ordering; I first show you all the goodies, what you came for, and than talk for ages on my "why's", what I came for; writing.

This part of the blogpost is therefor mostly for me, as a viewer experience of myself. And others can read it too as a bonus.

##### In defense of Programming as a Designer

CSS itself is just awesome as a **prototyping & testing** tool for your design to final code steps! That to me sounds a lot like... programming!

Especially if you're new to CSS, a testing-library to see where all things are placed (or even working!) is quite nice! That's a program, not a stylesheet imo.

So instead of breaking things in production-ready libraries, I decided to break away from that idea and just isolate a single purpose; testing

It seperates two things gracefully; the fact I can ruin development assets that they want to protect so preciously per repository, and the fact I can test those artifacts by the facts they don't meet their own standards.

Not in post production; **preproduction** testing, when you're setting things up so you don't have to check them after the fact; you know because you tested it first!

And so Q-Wind was born in a way of simplicity-first; one form, one function, one fiction of purpose. To test designs before the fact they need to be tested in the front-end.

It's always far less expensive to test and prevent things upfront, ask your local fire department. 

So that goes too in code, where designers now face a layer of code they normally don't WANT to see. But as you can see they can easily layer their work around their developers work.

It's a missed opportunity if we want to see designers code, because what you ask of them is to code like you. Ask HOW would designers code, and you will see they have a different approach from the surface.

##### Press SPACE, designers

See most people probably don't get the origin of `code;` it's a language, not a production-ready standard to comply with from the start. Most developers don't get this too.

Testing is production too, it's very easy and therefor also very hard to forget, and it doesn't just happen in the front-end. And I don't understand why you should treat your test-colors any differently than your brand-colors, especially if you're using the same technology & language.

That's literally re-inventing the wheel of purpose, by a simple dumb word; brand colors, not just colors. They instantly get some halo-effect because they belong to "the brand", but your system doesn't care. It's just another color, and it can be treated as any other first-class citizen.

Testing sounds much like insurance, like it's a good thing to always be testing. It is, but why is testing not done manually and always thought of in the end? 

And if you do only test design at the end, you did it too late imo and most likely you are not a designer. You need to ask why designers don't test their designs and think it's a front-end job, and most likely they will say "because only you can do that"!

An illusion of mind, created by framing & naming testing environments. Like if you don't do it in an "environment", all hell brakes lose and we need bullet-proof glass to protect us from a css-file written badly.

##### Designers don't need to code, they need to work

See, I just think the whole idiom of designers who "need to code" is a FAD of self-invented luxury. Like they have the choice to not code.

The "Big Devide" or "Big Gap" that people are talking about is nothing more to me than the inability of people caught up in their own idea of what is "technology".

Designers don't think visually, they just see the surface. That's why they think visually! Because they only see that surface as design. It's a bit of a mindfuck, but words frame the mind here.

I pit designers and developers against each other here, like I'm on either side. It's the framing that makes people think designers can't code, or that developers can't do visual design or sales. 

Titles in that sense always create more confusion than clarity on which side you or I am on. So lets ditch that for a second in our assumptions so we can clearly look for intent & impact.

If everyone would see code, would they than magically transform everyone into developers? No, they would just do the work they need to do. Mostly defined by their title, so what's the point to coding if your work doesn't adapt to that?

Some just don't want to code, they want to drag & drop code on a canvas... Like that's some form of programming they are entitled to, and others should fix it for them.

Again, they see the surface because that's the only thing they can see. By choice or by force, your memories make you and your thoughts around a certain context.

If I would be the designer on your team, or even a corporate, I would opt for 100% user generated design-ops. Like how Little Big Planet and Super Mario Maker let you do anything with it, and test it too.

That makes me sound more like a design engineer, that drives UX to a degree of DX, on par with devs. But the truth is that it is totally possible if you would see OS as a standard company practice.

If you can do drag & drop professionally, so can they right? The interface doesn't care if there is a noob or a pro in control, it just works. So too should our design language just work for everyone aboard. Or at least as much as possible.

Let the user fix the UI & UX for themselves with some blocks that do it all! That sounds far fetched but that was the original idea of a design system; to let the end-user be in control. 

## Dinosaurs never Die

Look at Blender for that matter, an open-source tool that has survived and thrived for 25+ years on the community alone. But it wasn't until their UI went fully towards "Everything Nodes" that it took off.

I'm not saying any should follow their footsteps, but look at some companies standards that have changed the game of the industry and you will see they did it with simplicity in UX. 

Apple, Google, Amazon, all of them. You can probably say in less than three words what they are best at or known for. These dinosaurs tend to stick around not only for their size, but for their continuos effort for more simplicity as things get increasingly complex.

Well I say CSS is at that stage right now, where the simplicity in UX is finally surfacing after all those years, and the complexity just doubled with @layers while it became far more clear to me as a concept too.

It's maturing to a state where you feel it's reborn, and you can now finally see the end of the tunnel before you actually go into the tunnel. If you ever wanted to program as a designer, start with CSS *now.*

And I'm fully betting on the UX they do right; **the semantical language & non-destructive layering**

See, the only times you see that kind of change for your kind of work is once in a lifetime, or we would have settled on best practices by now and CSS-in-JS would have died. 

And CSS has been there since the beginning, just like Blender.

And for more than half a century, a text-editor has always been good enough to create those awesome coded things you and I interact with everyday. 

Now, the language is what matters and what makes or breaks people from actually speaking your coded language to begin with.

CSS is a legacy, yes, but one that will stay for a long, long time since language is the main driver behind the web's technology. 

## Signing off

Any questions? Just askgu.us
See more? Just followgu.us
Who are you? justgu.us

You see, how can any job title compete with that?! Even if you think I'm a unicorn (des+dev), that would make me sound boring by just being myself. A golden standard nobody can beat; just be yourself.

You would simply lose value by giving me a title! But I would love to get in touch with you to do work for you too. I win, you win, game over... No more job titles, just professional people being equal!

Naming things is that important to me, and if you've made your own name a brand identity that in the literal sense represents you as a professional, you better back it up or your name didn't mean anything to no one; not even yourself.

I had the highest of highest education, but I never needed to waiver a paper to make a point. The point is that language is a technology itself, and I was born to write.

Titles don't show people's ambition or competence, only their supposed responsibility & authority. But they are static and not dynamic declarations of power, or they wouldn't be asking for the pay-raise to begin with.

And the only job-title I have is to just be me and do what I'm good at; creating co-operative systems of dynamic & fluid design for the armies of one, and the many.

As a (game) designer I write design rules in the CSS programming language based on my design system's layered architecture & naming; Lock, Load & Ship!

Today I don't use the cascade anymore to explain how it works, or specificity; I think of it already like Photoshop now, with layers of "watering down" the rendering.

I talk in a more kinetical way of how things move inside the system, and how we relate to them on the metaphorical plane. 

The analogy of a river has always resonated with programmers, trees too. Natural language is key then.

CSS uses @layers now that will make you feel right at home coming from any graphical application, except this is how a developer layers their artwork; using a CS language because it needs to be automated. 

### Language as a system

I intentionally mentioned I'm a game designer here, as games are closed systems of feed-forward and feed-back to not only the player-space (UX) but also the maker-space (DX). 

They apply the right kind of restrictions to allow the movement and freedom within the space. You think you can do anything in a modern game, but it's the opposite actually; it's how far the makers got to creating the illusion of it.

How it's made is not how it's sold...

##### A word about CSS

And that is what this post is actually about; what if **the word CSS** was invented to refer to "Closed System Strategy", in which the purpose is to create a closed system of design. Much like a videogame.

Yes, it's a horrible name new abbreviation for CSS. Yes, it doesn't sound sexy. Yes, it will even create a bigger feeling of nerdy disgust to say " Why are you using Closed System Strategy and not React+Emotion?"

Comparing CSS with React to begin with is comparing apples & pears these days, not because they are neither good or bad, or that they are a programming language (they are standards); of a strongly typed, closed system strategy.

It's because everyone still sees CSS as a "cascading style sheet", and those words never seem to bother anyone as a "source of evil" on why CSS is frowned and looked down upon...

To me CSS a functional design language, that **I LOVE** learning how to program! So yes, you can use it as a programming language, just like how you can use JS to print "hello world" and call it "programming".

I'm fond of CSS layering and watering down my design choices and rules to specific details, like how video-games have their player-spacerestrictions, so the browser can know what to do when it's players and content shift context & states. 

It's the only programming language specifically driven by design, for design. It is also the only programming language that is becoming more semantical & technical at the same time rather than more complex.

 Meaning simply; it's getting far easier to do CSS today than ever before. That's not just the language doing that, that's mostly done by all the support it's getting from awesome developers.

In my humble opinion, the true value of a good programming language is simply that you can read it, without knowing about it. A native language if you will.

```css
  body {
    line-height: 1.6ex;
    -webkit-font-smoothing: antialiased;
    text-rendering: geometricPrecision;
  }

  p:not(.text-hidden){
    font-size: 21px;
}
```

CSS is very beginner-friendly in its reading experience, even if you've never seen it. 

And for your ease of comfort, or not; I'm just beginning to learn the "new way" that is literally a few days old historically speaking. 

Luckily computers don't care if you're bad at it, they just execute it and if it works; congrats, you are now a "software engineer" because you made your program work.

The new CSS syntax is not more complex than Excel these days, and mostly it doesn't take more than three lines of CSS to create something effective & simple.

My point is simply this; if we only say CSS is for styling, and not for programming our own closed system of styling things with the browser, I don't think people will actually get to know the new CSS to begin with.

##### functional programming vs functional language

CSS as a functional programming language that enables you to program design as a rule-based system that uses the browser to solve the problem.

It's not just made to make pretty things in the browser, and focused on production-first. It's framed too much the old way, and the naming doesn't help much either.

So what am I saying? Well, we need to *relanguage CSS* a bit, because it still sounds "dusty, dirty & nerdy" to the many. Because of how it's *named & framed* and sounds somewhat of a shame to love & use by some.

I'm not the only one making a point about this; Ahmad Shadeed wrote about the contextual shift that we can undergo too to see CSS differently, and my take here is *testing in the browser,* and it can do that too.

It will never be production-ready because that's not what it was meant for; it was meant to make your stuff production-ready faster by seeing what is happening with --Q.

I hope you've enjoyed this read, me too!