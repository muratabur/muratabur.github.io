---
layout: post
title:  "Banking Data Standards"
date:   2015-08-08 12:00:00
categories: data standards, startups
---

# A standard success story
One of my favorite stories of data standards is that of General Transit Feed Spec ([GTFS][1]) which in a few short years went from a holiday dream to a reality. The full story is [here][2]. In a nutshell, a visionary public servant combined with a civic minded technology company to create the standard to publish transit data in a useful format for developers. They started out small (sorry Portland) and ended up changing the world with very little investment or marketing budget. Moreover, the project is open source and growing organically. Basically, perfect execution for implementing a global data standard and further proof that visionary innovation does not come from the big players.

In my opinion, there are a few key things that stand out which drove the success of the project:

1. **Simple**: The standard is very simple to understand so everyone from the largest transit agency to the smallest can adopt it easily. Five minutes browsing the above link and you will be able to describe it to your friend.
2. **Shrinkable**: Being scalable down is what makes a standard universal. The resources required to deploy, manage, update and publish should scale with the size of the organization. A small town probably has very few buses and even fewer changes to their schedules/routes, but London has loads.
3. **Fundamental**: It hits at the core of what a transit agency does for the customer. As a passenger I want to know which bus, where to get it and when is it coming. I do not care about the bus make, vehicle registration, driver name, last service date etc. which are all valid data points from a transit authority point of view but not necessary reporting for a customer point of view.
4. **Optional**: Optional standards mean they can be adopted if and only if they are good. If there was a multi-million dollar government program to harmonize and create a proprietary transit standard it undoubtably would not have been as successful.
5. **Friendly**: Machines and humans can injest reports/data easily which removes any entry barrier. It is also published online with tons of documentation, examples and a free, open forum for the community. 

# A standard failure

But one might try and argue that banking has a data standard already, XBRL. While this works well for documents and reports, XBRL and other XML-based data formats (like FpML) have not been anywhere near optimal. If the financial crisis was not evidence ennough that the format is broken, we can see that XBRL has failed all five of the key tenants above of what a successful standard should embody. 

1. It is so complicated that there are entire businesses built around converting an excel file to XBRL. 
2. The resource burden placed on smaller banks to produce and populate these files is too large to do internally and hence they are forced to waste resources on poor, manual 3rd party vendor solutions. 
3. XBRL is often described as XML on steroids which is an apt description of the level of unnecessary detail it contains.
4. The format was imposed on banks rather than being adopted due to its utility.
5. The inherent structure of XBRL creates unnatural hierarchies and sparsely populated documents rather than a data format for injestion.

---

Before we go further, we need to accept that 

# Problems with banking data
- The data is living. A financial product's core fields change during its lifetime. Moreover, these changes are unpredictable in terms of time (when they will occur) and quantity (how much affect they will have).

- The fields are inter-linked. A change in one field can have quantitative and/or qualitative effects on other fields or other products. A change in *interest rate* will change *monthly payment*

- ds




[1]:	http://...
[2]: 	http://beyondtransparency.org/chapters/part-2/pioneering-open-data-standards-the-gtfs-story/