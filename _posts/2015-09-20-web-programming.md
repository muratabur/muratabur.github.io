---
layout: post
date: 2015-09-20 12:00:00
title: "Web programming sucks"
type: 
image:
categories: programming
---


I don't like to write about programming theory because there is so much already written on the web by people much more qualified and knowledgeable than myself. However, I do think web programming is especially ugly and needs to be re-thought. While it is great that you can write some code that can be essentially deployed to any device running a broswer, that is more of an adoption of standards rather than a fundamental aspect of HTML/CSS/Javascript. 

Programming concepts are not always well understood by people who code, because most programmers are not CS graduates but people who have learned on the job. It is a bit like cooking. Hence, most advice you find online are practical solutions to "I have problem X and need to get Y." While it is great that almost any problem you have has been solved before, this is a bit like cheating ie. getting the right answer without understanding why. This is not surprising given that the educational system favors learning how to pass the test rather than the fundamental underlying concepts.

> I am not a fan of jumping to the answer without thoroughly understanding how to get there. So copy and pasting someone else's code doesn't sit well and, in my opinion, can lead to massive amounts of [technical debt][tech-debt] that you will regret later.<sup>1.</sup>

<aside><num>1.</num> I found using sites like Weebly and Wordpress extremely frustrating as any attempt at customization or personalisation ending in disaster.</aside>

### But it works
When I made my first webpage in 1995, there was only HTML so it is very hard for me to imagine what else it could have been so let us take it as a starting point. And I assume that is what most people did because what seems to have followed is just a selection of small shortcuts up to what we have now which is a bit of a mess, in my opinion.

When I decided to take another serious look at web programming a few years ago, I started like I had before, writing pure HTML in notepad. After getting some basic content on the page, I started to turn to formatting which is when I realized that I could do a heck of a lot more than the basic <h/p/a> formatting I knew. After writing style="" 100 times for each div, I thought hmm, maybe I can define a variable somehow for this. Voila CSS, clearly the brainchild of someone else who spent 1 week writing HTML and got sick of copy and pasting formats into each DOM element. Ok, this was better, but still not very intuitive. You basically had to look up every term and see what variables it would accept. CSS would useless without the online reference dictionary. It was also quite static. How can I do an animation, or change a color when I click?

That is when I entered the chaos of Sass/Less, Javascript, PHP, Ajax, JQuery, charting libraries, Bootstrap, Font-Awesome etc. Soon, I had so many different things I was importing and referencing, my codebase was basically 95% written by someone else, or worse, by 1,000's of other people. There was no consistency in approach or design. It became impossible even for me to understand what was going on, but when you loaded the page... it worked. 

### Learning from experience
That is when I realized that I had become *one of those people*. I had resorted to copying and pasting instead of finding my own answers. But how had that happened? Because it was easy and because I had no choice.

> All of these web manipulation tools did essentially the same thing, but none of them were designed in an intuitive manner. Yes, they gave commands to the computer, but you had to memorize all the commands, you couldn't learn a few and use those to make up the rest. It is the linguistic equivalent of a second-rate language - one where you have to memorize all 10,000 words instead of just the alphabet. 

There was no way for me to intuitively come up with terms like "addEventListener" or "getElementsByTagName" from fundamental concepts or defintions. So the only solution was to resort to searching the web and finding a solution to a similar problem online. Some say this trial-and-error development method forces you to be agile and test quickly, but really it is a waste of time and huge source of inefficiency and errors.<sup>2</sup> 
<aside><num>2.</num>Just swap Angular for Ember and time how long it takes you to get back to square one.</aside>

This gives most Javascript developers an experience-based learning curve. The only problem is that with frameworks and libraries being re-written and going out of favor every couple years, everyone is constantly starting from scratch. Eventually one library will be *adopted*, not due to its elegance, but due to critical mass.

### D3
Then I stumbled across [D3][d3]. It was a shining light of DOM manipulation at the most fundamental level. It had a few basic components, a few concepts to understand and everything else you could generate yourself intuitively. It felt *intuitive*. I felt *in control*. Moreover, existing code is easy to digest, even for the most complex visualisations. I haven't counted but there are probably more graphing libraries built on top of D3 than all other Javascript libraries combined. I think D3 is here to stay because it is good. Not because it has critical mass. Styling in D3 is also mostly handled through the script rather than the style. Programmatic manipulation of style is much more intuitive and powerful than loading an endless CSS framework and then adding to it with over-writes. This is particularly true as you start making your style more dynamic and conditional on mouse movements and interactions.

### Overcoming.js
There are hundreds of sites dedicated to hating on JS, but I think [JSFuck][jsfck] is my favorite. For myself, the most bothersome aspect is the notion of callbacks. It can take a simple program into an endless series of mind loops, requiring the programmer to keep multiple levels of [Inception][inception]-style nested logic. And just like the inception limit of inceptions within inceptions in the movie Inception, good javascript needs an enforced limit of callbacks. The same way good programs limit the number of nested for loops. Javascript has it's origins at Netscape, being developed under pressure by a corporation to compete with Microsoft so it is probably safe to assume it was underfunded, rushed and never expected to outlive its immediate purpose by 20 years. As a new language, the corporate objective for adoption needed it to compete with VB, feel welcoming to C developers but sound like Java. Unfortunately, javascript doesn't seem to be going away anytime soon. <sup>3.</sup> 
<aside><num>3.</num>You can probably say the same things for VBA.</aside>  

So suck it up. Accept that web programming sucks. But know deep inside that it doesn't have to.


[tech-debt]:	https://en.wikipedia.org/wiki/Technical_debt
[d3]:			http://d3js.org
[jsfck]:		http://www.jsfuck.com/
[inception]:	http://
[dart]:			http://www.dartlang.org