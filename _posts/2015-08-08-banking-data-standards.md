---
layout: post
title:  "Why banking needs data standards for regulation to work"
date:   2015-08-08 12:00:00
categories: [data standards, banking]
---

It is clear the banking system needs technological innovation and recent history has demonstrated the incredible power of collaborative open-source projects to spark that innovation. I will start by highlighting an example from - and arguably less sophisticated - sector to get all the pessimists out of the room.

### A standard success
One of my favorite stories of data standards is that of General Transit Feed Spec ([GTFS][gtfs]) which in a few short years went from someone's holiday dream to a global reality. The full story is [here][gtfs-story]. In a nutshell, a visionary public servant combined with a civic minded technology company to create the standard to publish transit data in a useful format for developers. They started out small (sorry Portland) and ended up changing the world with very little investment or marketing budget. Moreover, the project is open source and growing organically. Basically, perfect execution for implementing a global data standard and further proof that visionary innovation does not come from the big players.

In my opinion, there are a few key things that stand out which drove the success of the project:

1. **Simple**: The standard is very simple to understand so everyone from the largest transit agency to the smallest can adopt it easily. Five minutes browsing the above link and you will be able to describe it to your friend. Hand in hand with simplicity is the idea of shrink-ability. Application developers always talk about scaling up, but being scalable down is what really makes a standard universal. The resources required to deploy, manage, update and publish data should scale with the size of the organization. A small town has very few buses and even fewer changes to their schedules/routes, but London has loads.
2. **Non-Competitive**: While it took some convincing, eventually the transit authorities realised that having a proprietary data exchange format was not a competitive advantage (it is the content of the message). This is obvious in hindsight but is something that all standards from HTML to flight data have in common.  
3. **Clear Purpose**: It hits at the core purpose of what a transit agency does for the customer. Why is this standard necessary and what will it be used for? As a passenger I want to know which bus, where to get it and when is it coming. I do not care about the bus make, vehicle registration, driver name, last service date etc. which are all valid data points from a transit authority point of view but not necessarily from a customer point of view. So a clear purpose is mandatory to limit and define the scope of a standard.
4. **Optional**: Optional standards mean they can be adopted if and only if they are good. If there was a multi-million dollar government program to harmonize and create a proprietary transit standard it undoubtedly would not have been as successful.
5. **Friendly**: Machines and humans can ingest reports/data easily which removes any entry barrier. It is also published online with tons of documentation, examples and a free, open forum for the community. 

But before we start with our data schema, lets understand a little bit more about the banking industry today.

### A standard failure

The banking industry has tried implementing underlying data standards like FpML, FIX etc. but while they have succeeded in some niche areas, you cannot show up to any bank and say "send me a portfolio of X" and know what to expect. Even saying please "send X in FpML format" will not be perfect as every institution *extends* the XML and adapts it to their needs. The primary reason for the standards failure is simple yet subtle.

> Data standards improve efficiency and foster collaboration where there is no incentive to compete on the raw data (differentiation happens at the application, user-experience or customer service layer), but data standards fail in highly competitive raw data environments. 

Banking products, when looked at as an economic good, are close to being perfect substitutes. This puts the banks themselves in a market with near [perfect competition][perfect-comp]. Banking products (consider a payment) are designed to be best when invisible, ideally never catching the attention of the customer. Without any opportunity to improve upon an instant, accurate and invisible customer service, banks are operating with prices very close to marginal costs.<sup>1</sup>
<aside><num>1</num> Whether or not those costs can be reduced is another debate, and one that retail consumer focused FinTech companies are actively challenging in the lending and payments space.</aside> 
Operating under these conditions, banks have looked inward to differentiate themselves by building or buying bespoke systems - each with the 'optimal data schema' for that particular system. The end result of decades of working like this and constant swapping of staff between banks is a collection of hundreds of separately optimal systems each serving a specific customer or product vertical.<sup>2</sup>
<aside><num>2</num>In other words, high-performance, reliable and inflexible legacy systems.</aside>
Until regulation required, these systems and the people that built them never had to spend much time talking to each other given the silo-ed business lines within banks. Moreover, these systems didn't need to be opened up and modified because the customer requirements never changed. Until a new customer came to town...

### A new customer

Following the financial crisis, regulatory requirements have skyrocketed. The 'regulator' has suddenly emerged as a new kind of customer. A customer that is demanding, detailed and frequent in its data needs and asking banks to present themselves in a way comparable to other banks - those same competitors banks are desperately trying to differentiate themselves from. To top it off, not only does this customer not pay for the services it requires, but it in fact *asks banks to finance its operations* as well.

Banks have approached this new customer in the same way they would have approached any other new customer segment. Create a new department, set aside a budget and build or buy new systems for that department. Unfortunately, this approach has failed and will continue to fail until banks stop treating the regulator as just another customer. They need to realize that there is no competitive advantage to serve an unprofitable customer. Luckily, many banks we have spoken to have realized this and are keen for innovation in this space.

In order to serve this new customer, banks need to embrace a common, collaborative, standards-based system which has core banking data at its heart. The first step in this process is therefore the establishment of a standardised data schema for core banking products.

> There is no incentive to compete in regards to regulation, and therefore it is an area where data standards can succeed.


[gtfs]:			https://developers.google.com/transit/gtfs/?hl=en
[gtfs-story]: 	http://beyondtransparency.org/chapters/part-2/pioneering-open-data-standards-the-gtfs-story/
[perfect-comp]:	https://en.wikipedia.org/wiki/Perfect_competition 