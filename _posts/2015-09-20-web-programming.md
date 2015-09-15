---
layout: post
date: 2015-09-20 12:00:00
title: "Web programming sucks"
categories: programming
---


I don't like to write about programming because there is so much already written on the web by people much more qualified and knowledgeable than myself. However, I do think web programming is especially ugly and needs to be re-thought. While it is great that you can write some code that can be essentially deployed to any device seamlessly, that is more of an adoption of standards rather than a fundamental aspect of HTML/CSS/Javascript. 

Programming concepts are not well understood by "programmers" and so 90% of what you find online are practical solutions to "I have problem X and need to get Y." While it is great that almost any problem you have has been solved before, this is a bit like cheating ie. getting the right answer without understanding why. This is of course typical of most educational systems - where students are taught how to pass the test rather than the fundamental concepts - so I was not surprised that this method of learning had become the norm for programming as well. Coupled with the millenial notion of *instant satisfaction* and the whole lean development philosophy, it is easy to see why most people would rather just hack together bits of other people's code than create something from scratch.

<aside>
<num>1.</num> I found using sites like Weebly and Wordpress extremely frustrating as any attempt at customization ended in disaster with multiple CSS overrides and conflicting instructions to the DOM. 
</aside>
> I am not a fan of jumping to the answer without thoroughly understanding how to get there. So copy and pasting someone else's code doesn't sit well<sup>1</sup> and, in my opinion, can lead to massive amounts of [technical debt][tech-debt] that you will regret later.


### Getting started
When I made my first webpage in 1995, there was only HTML so it is very hard for me to imagine what else it could have been so let us take it as a starting point. And I assume that is what most people did because what followed was just a selection of small shortcuts up to what we have now which is a bit of a mess in my opinion.

When I decided to take another serious look at web programming I started like I had before, writing pure HTML in notepad. After getting some basic content on the page, I started to turn to formatting which is when I realized that I could do a heck of a lot more than the basic <h/p/a> formatting I knew. After writing style="" 100 times for each div, I thought hmm, maybe I can define a variable somehow for this. Voila CSS, clearly the brainchild of someone else who spent 1 week writing HTML and got sick of copy and pasting formats into each DOM element. Ok, this was better, but still not very intuitive. You basically had to look up every term and see what variables it would accept. CSS would useless without the online reference dictionary. It was also quite static. How can I do an animation, or change a color when I click?

That is when I entered the chaos of Sass/Less, Javascript, PHP, Ajax, JQuery, charting libraries, Bootstrap, Font-Awesome etc. Soon, I had so many different things I was importing and referencing, my codebase was basically 95% written by someone else, or worse, by 1000's of other people. There was no consistency in approach or design. It became impossible even for me to understand what was going on, but when you loaded the page... it worked. 

That is when I realized that I had become *one of thos people*. I had resorted to copying and pasting instead of finding my own answers. But how had that happened? Because it was easy and because I had no choice.

> All of these web manipulation tools did essentially the same thing, but none of them were designed in an intuitive manner. Yes, they gave commands to the computer, but you had to memorize all the commands, you couldn't learn a few and use those to make up the rest. It is the linguistic equivalent of a second-rate language - one where you have to memorize all 10,000 words instead of just the letter of the alphabet and the pronounciation rules. 

There was no way for me to intuitively come up with terms like "addEventListener" or "getElementsByTagName" from fundamental concepts or defintions. So the only solution was to resort to searching the web and finding a solution to a similar problem online.

### D3
Then I stumbled across [D3][d3]. It was a shining light of DOM manipulation at the most fundamental level. It had a few basic components, a few concepts to understand and everything else you could generate yourself. It felt so *intuitive*. I felt *in control*. 

Web programming sucks. But it doesn't have to.



[tech-debt]:	https://en.wikipedia.org/wiki/Technical_debt
[d3]:			http://d3js.org