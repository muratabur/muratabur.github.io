---
layout: post
title:  "Full-Stack FinTech"
date:   2015-09-14 12:00:00
cover: /images/pancake-stack.png
categories: [fintech, enterprise software]
---

Starting out as a new company, you need some core services just to run things together. Somewhere to store your files, emails, office space, accounting, recruitment, invoicing, legal, mailing lists, advertising etc. Naturally, you outsource these functions at the cheapest possible price and ideally for free because they do not differentiate your business. As your company grows, you may start to bring these functions in-house like hiring a general counsel, CFO, HR manager and so on because how you do your accounting or recruiting could become a differentiating factor. This is obvious outsourcing.


### Outsourcing in your product
Now, as a technology company, it becomes really easy to start outsourcing non-core bits of your product as well by incorporating software services from other companies as components in your own product. Consider using Twilio's API to send text messages, Mailchimp to send emails, Stripe for payments, chatbots for customer service, Readme for documentation or any of Amazon's Web Services. Undoubtedly, the "tech revolution" of the past decade has been the emergence of all of these software services which have made new software development quick, cheap and highly scalable. All of this *outsourcing* boils down to essentially using the cloud and connecting to APIs. Fundamentally, for these APIs to serve your purposes, they require you to send your data to someone you don't know and somewhere out of your control.But what if you are a bank and your infosec policy doesn't allow for data to venture outside the firewall?

> The last decade of "tech revolution" is completely inaccessible to a bank. 


### On-premise software
This is why legacy systems survive and banks are still running slow batch processes and moving large files around filled with unvalidated data. No one is developing on-premise software anymore! It is not "cool" to build and maintain a database model and FTP connections for every customer. Would Paul Graham advise you to re-configure your product to every possible permutation of Oracle, IBM, SAS and SAP license a customer may or may not have? Maybe, I don't know. But the point is that on-premise software is classically unscalable. It takes too long to build (because you have to build your own version of every API you would ever want to use) and takes too long to sell (because you have to go through procurement, penetration testing and/or wait for other vendor licenses to expire). Moreover, until you have all the IT and business features, requirements and integrations developed, your technology is simply unusable. Got a great trading platform? Make sure you can deploy it on WebSphere and you've already paid, integrated and tested the market data connection with multiple failover server. Let's be clear, this is not an attractive proposition to any young startup with limited resources. Getting your first few clients and finding a minimum-viable-product that is usable can be an insurmountable challenge. Then how can Oracle be so ridiculously profitable?

> But what no one tells you, is that once you overcome that initial hurdle, you become unstoppable. There is no competition at the top.

One of the few companies to see this opportunity recently is Palantir who has quietly become a [multi-horned unicorn][palantir] with very little public explanation of what it is they actually offer. This is often the nature of complex enterprise solutions - if you are not a potential customer, then there is no point to try and explain the solution. There are probably a few hundred companies that Palantir could sell to. Contrast that with Uber's billions of target customers. But Palantir (at least from what they say) is sitting at the top of their market with very little competition whereas Uber's ride-sharing market is crowded with hundreds of competitors offering essentially the same thing.


### The full-stack approach
The full-stack approach is about owning a product or service end-to-end. Full-stack products not only replace your current product, they also replace other people that used to be in the chain. With the iPod/iTunes combo, Apple not only replaced your discman, but they also cut out the record store, the radio,headphones, batteries, cd-burners... The iPhone had a similar impact. Sonos, Nest, when IoT companies go full-stack works, it can work particularly well. Tesla is now doing the same thing with cars - no dealership, no mechanics etc. With a full-stack product, Tesla collects not just the upfront sales, but all future revenue because they can control the quality of every single component in the supply chain.

For FinTech companies dealing with the on-premise problem, and by FinTech here I mean *companies selling software to financial institutions*, going full-stack is absolutely a must for two reasons: 

1. The first reason is so that you only have to change your software *only when your software changes*. This is important because nothing is ever backward compatible on-premise. In fact, large vendors make very good money consulting and fixing these compatibility issues. 
2. Regardless of what you are doing, the "problem" you have identified and want to solve will only be the tip of the iceberg of *the problem you actually need to solve*. Systems inside banks are so interconnected that if you replace one component, five other components fall over. Whats worse, those five components will not be the same at each bank. Imagine that trading platform you built. You will now need to also build the internal reports that the old system used to generate. You will also have to provide reconciliation reports and issue trackers. And maybe that trading platform was also their CRM or settlement tool. If you do not own your whole stack, you will not be able to accommodate for the host of secondary objectives you software will need to fulfill to pass acceptance.

Owning your full stack might take longer and cost more, but it will pay dividends many times over further down the line.


[palantir]:	http://techcrunch.com/2015/12/23/palantir-has-raised-880-million-at-a-20-billion-valuation/