---
layout: post
title: Some notes on Agile Development
date: '2015-11-19 15:02:00'
---

<p>Agile development is a Cult to some, a Fad or just plain old weird to others. I'm a fan of this type of development. I've seen teams do great work by adopting Agile and a framework to execute it. Agile isn't magic bullet however. Some Agile projects fail. I do find it the best way to iterate and communicate, so it really works for me personally. I'd like to go over the <a href="http://www.agilemanifesto.org">Agile Manifesto</a> and add in my own notes.</p>

<p>But first, some definitions for those new to Agile and to make sure I'm clear on any of my own jargon.</p>

<ul>
<li><p><a href="http://www.webopedia.com/TERM/A/agile_software_development.html">Agile development</a> is a phrase used in software development to describe methodologies for incremental software development. Agile development is an alternative to traditional project management where emphasis is placed on empowering people to collaborate and make team decisions in addition to continuous planning, continuous testing and continuous integration.  </p></li>
<li><p>Product Owner: The person responsible for the Project. He or She works closely with the client, other stakeholders and the development team.</p></li>
<li><p>Scrum Master: The Person responsible for communicating from and within the team to the Product Owner. Akin to a Producer or Project Manager. He/She helps manage the production of the team and in some cases the personnel of the team. This is what I currently do.</p></li>
<li><p>Sprint: A chunk of time, usually 2 weeks, that a team dedicates to work on the software. The team commits to working on specific things in a Sprint. Those commitments would only be changed in extreme circumstances.</p></li>
<li><p>Backlog: The list of things that need to get done. Prioritized by the Product Owner. </p></li>
<li><p>User Story: The items in the Backlog that become tasks for the team. Usually written in the voice of the software users. For example: "As a user I need to be able to log into the website."</p></li>
<li><p>Epic: A User Story complex enough to warrant being broken down into other tasks.</p></li>
<li><p>Task: A unit of work needed to be delivered to fulfill a User Story.</p></li>
<li><p>Sprint Planning: A meeting that kicks off the Sprint. In this meeting the Product Owner and/or Scum Master go over the prioritized Backlog. The team then generates the tasks and estimates how complex (Story Points) and how long (Ideal Days) they'll take to get done.</p></li>
<li><p>Sprint Recap: Review the latest build of the software to check progress. Everyone is present from the team. Sometimes the Client is present as well.</p></li>
<li><p>Sprint Retrospective: The development team and Scrum Master get together to talk about the previous Sprint and determine what about the process/team can be made more effective.</p></li>
</ul>

<p>That's a good enough intro to get us running. On to the Manifesto itself. It reads:</p>

<ul>
<li>Individuals and Interaction > Process and Tools</li>
<li>Working Software > Comprehensive Documentation</li>
<li>Customer Collaboration > Contract Negotiation</li>
<li>Responding to Change > Following  a Plan</li>
</ul>

<p>The stuff on the right is important, but it's not as important as the stuff on the left. Hence my use of the Greater Than symbol. That last bit about responding to change applies to the Agile Development process itself. In Agile, the team is supposed to evaluate the process they're using and adapt to change. Teams that don't change  have a greater risk of failed projects. Change can be hard, but the process requires you to do so, which can only lead to growth, imho.</p>

<p>The 12 principles of the Agile Manifesto:</p>

<ol>
<li><p><strong>The Highest Priority is to satisfy the customer through early and continuous delivery of valuable software.</strong> Iterate, iterate and iterate some more. Agile wants transparency with the client at all times. A working version of the software, even without all the features is the thing to evaluate at a given time. This helps you learn, collaborate and pivot.  </p></li>
<li><p><strong>Welcome changing requirements, even late in development. Agile processes harness change for the customers competitive advantage.</strong> The time you know the least about what you're building is at the beginning (planning). If you close off the opportunity to change, you can wind up building the wrong thing, or the thing that no one wants to use. But you can't run around changing everything everyday, madness that way lies. So you generally protect the Sprint commitments as much as possible, and plan on evaluating and changing priorities for next Sprint. </p></li>
<li><p><strong>Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale.</strong>  Make something quickly, evaluate it, adjust. Pivoting is key in software development, short cycles help you know what you don't know.</p></li>
<li><p><strong>Business people and developers must work together daily throughout the project.</strong>    The Product Owner fills this role most often. That person must know business and development well. Their knowledge doesn't have to be deep on either end, they have to be great in that gray area in the middle.  Although Scrum Masters and Developers should be versed in this too, or at least know enough about the customers business to be able to anticipate challenges, and generate ideas.    </p></li>
<li><p><strong>Build Projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done.</strong>  On a personal level this one rings so true to me. It's not about "just getting out of the way", although sometimes that's the best thing to do. It's about setting clear goals and a cadence and supporting the developers. That can be rendered in a million different ways. This is the work I enjoy most.</p></li>
<li><p><strong>The most efficient and effective method of conveying information to and within a development team is face-to-face conversation.</strong> Working with remote team members is wonderful. It allows a company to not be constrained geographically when looking for and keeping talent. That said, it's a challenge to stay in touch if everyone isn't in the same space. Talk to each other face-to-face if you can. Video chat if you can't. Have a Slack/HipChat/whatever too. Talk to each other. </p></li>
<li><p><strong>Working software is the primary measure of progress.</strong> This sounds so simple, and it is. How's the project doing? Look at the latest build. We're good at building all kinds of metrics and data-driven evaluations. Those can be great supporting metrics. The latest build is the best. It informs you of what you know, and what you don't know, at that point in time.</p></li>
<li><p><strong>Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely.</strong> A lot of people new to Agile don't really grok this. There are processes to measure the development teams <em>Velocity</em>. Which is simply how much the team can get done in a time period. Velocity is best measured in a system that takes into account Complexity, not Hours. This system lets you know how much you'll be able to get done in the Sprint. And when things change, as they always do, you'll be able to adjust. <br />
There's so much to this, as it's a weird metric for some people. The short story is to find a task that everyone agrees is 'not complex'. Use that as a base-line to measure the others tasks against. Categorize everything in a complexity system comprised of Story Points, or T-shirt sizes, whichever works for your team. Then measure how many of these points you can get done in a Sprint. That's your Velocity. You'll need several Sprints and some discussions to understand the average and to make sure your categorization is correct. It's so worth it. Once you have this information, you can tell each other, the client or anyone else what you'll be able to do in a Sprint right from quick discussion about the Backlog.    </p></li>
<li><p><strong>Continuous attention to technical excellence and good design enhances agility.</strong> Humans want to do the best job they can. It's just in our nature. After all, "We are here to make a dent in the universe". A Scrum Master who builds the right information, space and time into the team lets everyone trust each other. A team that trusts each other will do the best work they can, and support each other while doing so.   </p></li>
<li><p><strong>Simplicity -- the art of maximizing the amount of work <em>not done</em> -- is essential.</strong>  The best way to simplify is to reduce. Cut features. A dropped feature is better than a broken or incomplete one. A Scrum Master can look to reduce the amount of waste as a way to simplify. Importance should be measured by the frequency the user needs to do something, how big things are on the page, etc. Cut it down to the essential. Build that. Learn from it. Expand it. Deliver working things, and iterate.</p></li>
<li><p><strong>The best architectures, requirements and designs emerge from self-organizing teams.</strong> The team wants to be awesome. They'll self organize to maximize each other. Management can guide this, and help the team figure out who's best at what types of work. But Management should resist dictating the who's doing what. Let each member of the team grow, when appropriate. People want to be awesome, guide them and let them.</p></li>
<li><p><strong>At regular intervals, the team reflects on how to become more effective, the tunes and adjusts its behavior accordingly.</strong> There are a couple of ways to evaluate the teams effectiveness. First is on a one-on-one basis, of course. The Scrum Master should be meeting regularly with each team member individually to discuss their progress, goals, growth and interests. <br />
The Sprint Retrospective is the place to collectively discuss the effectiveness of the team. When a team first comes together, these meetings can be too quiet. If there isn't enough trust yet, no one will want to speak up. As the Scrum Master, start with yourself. You're  a part of the team after all. As a Scrum Master, I like being a <a href="http://www.benhallbenhall.com/2013/03/scrum-meeting-pigs-chickens/">Pig</a>.  Tell the team this is what you think you can do better or differently. Start there. Build the trust.</p></li>
</ol>

<p>Agile works for me as I'm a fan of simplicity, <a href="http://blog.codinghorror.com/boyds-law-of-iteration/">Boyd's Law of Iteration</a> and working with teams. The team builds great momentum from constantly shipping software. Yes it's frequent shipping of small pieces, but those pieces add up quickly and great trust and collaboration is built. </p>

<p>Want to talk more about this? Find me on <a href="http://www.twitter.com/@chad_g_moore">twitter</a>.</p>