## PREFACE

- What Makes a Pragmatic Programmer?
  - Early adopter/fast adapter: instinct for technologies, love trying things out
  - Inquisitive: be a pack rat for little facts
  - Critical thinker: rarely take things as given without first getting the facts
  - Realistic: understand the underlying nature of each problem you face
  - Jack of all trades: try hard to be familiar with a board range of technologies and environments

`We’re challenging you to THINK about WHAT you’re DOING WHILE you’re DOING`

## Chaper 1: A Pragmatic Philosophy
`The Cat Ate My Source Code`
One of the cornerstones of the pragmatic philosophy is the idea of taking respnsibility for yourself and your actions.

### Take Responsibility
You have the right NOT to take on a responsibility for an impossible situation, or one in which the risks are too great. When you DO accept the responsibility for an outcome, you should expect to be held accountable for it.

Make a mistake or an error in judgment -> admit it honestly and try to offer options. Don’t BLAME, or make up an excuse. Provide solutions.

If the disk crashes-taking all of your code with it-and you don’t have a backup, it’s YOUR FAULT.

“The cat ate my source code”, won’t cut it. Before tell anyone why something can’t be done, stop and listen to yourself first. Does it reasonable? or stupid?

Before you go and tell them the bad news, is there anything else you can try? Instead of excuses, provide options.

Don’t say it can’t be done; explain what can be done to salvage the situation. How to prevent it from happening again?

### Software Entropy
Don’t live with Broken Windows. Fix each one as soon as it is discovered.

Take some action to prevent further damage and to show that you’re on top of the situation.

### Good-Enough Software
You can discipline yourself to write software that’s good enough-good enough for yours users, for future maintainers, for your own peace of mind.

### Know when to stop
Dont’ spoil a perfectly good program by overrembellishment and overrefinement. Move on, and let your code stand in its own right for a while.

### Your Knowledge Porfolio
Your knowledge and experience are your most important professional assets.

Unfortunately, they’re expiring assets. Your knowledge becomes out of date as new techniques, languages, and evironments are developed.

### Goals
- Learn at least one new language every year
- Read a technical book each quater
- Read nontechnical books, too
- Take classes
- Participate in local user groups
- Experiment with different environments
- Stay current
- Get wired
- Critical thinking
- Think critically about what you read and hear

### Communicate
We have to communicate on many levels. We spend hours in meetings, listening and talking. A large part of oour day is spent communicating, so we need to do it well.

### Know what you want to say
Plan what you want to say. Write an outline. Then ask yourself, “Does it get acroos whatever I’m trying to say?”. Refine it until it does.

### Know your audience
You need to understand the needs, interests, and capabilities of your audien.

### Choose your momment
As part of understand what your audience needs to hear, you need to work out what their priorities are. Make what you’re saying relevent in time, as well as in content.

Sometimes all it takes is a simple question: “Is this a good time to talk about…?”

### Choose a style
Adjust the style of your delivery to suit your audience: briefing, wide-ranging chat, reports, documents… If in doubt, ask

### Make it look good
Your ideas are importent. They deserve a good-looking vehicle to convey them to your audience

### Involve your audience
If possible, involve your readers with early drafts of your document

### Be a listener
If you want people to listen to you, listen to them.

### Get back to people
Always respond to e-mails and voice mails, even if the response is simply

## Chapter 2: A Pragmatic Approach

### The evils of duplication
As programmers, we collect, organize, maintain, harness knowledge. Unfortunately, knowledge isn’t stable. It changes-often rapidly. It means we spend a large part of time in maintenance mode. Programmers are constantly in maintenance mode day by day.

DRY: Eeach piece of knowledge must have a single, umambiguous, authoritative representation within a system

*How does duplication arise?*
Imposed duplication: Developers feel they have no choice-the enviroments seems to require duplication
Inadvertent duplication: Developers don’t realize that they are duplicating information
Impatient duplication: Developers get lazy and duplicate because it seems easire
Interdevelop duplication: Many peole on a team(or orther teams) duplicate a peace of information
Orthogonality
Two or more things are orthogonal if changes in one do not effect any of the others.

*Eliminate effects between unreleated things*

- Gain productivity
- Changes are localized
- Promotes reuse
- Gain productivity when you combine orthogonal components

*Reduce risk*

- Diseased sections are isolated
- The resulting system is less fragile
- Be better tested
- Tighly tied to a particular vendor
- Coding
- Everytime you write code you run the risk of reducing the orthogonality of your application

*Maintain orthogonality*

- Kepp your code decoupled
- Avoid global data
- Avoid similar functions


## Chapter 3: The Basic Tools

Every craftsman starts his or her journey with a basic set of good-quality tools Each tool will have its own personality and quirks, and will need its own special handling. Each must be sharpened in a unique way or held just so.

Many programmers make the mistake of adopting a single power tool, such as a particular integrated development environment, and never leave its cozy interface. This really is a mistake.

### The power of plain text
As programmers, our base material isn’t woord or iron, it’s knowledge. And we believe the best format for storing knowledge is plain text.

*What is plain text?*
Plain text is made up of printable characters in a format that can be read and understood directly by people. You can do everything with plain text that you could do with some binary format, including versioning. Plain text tend to be higher level than a straight binary encoding, which usually derived directly from implementation.

*Drawbacks*
There are 2 major drawbacks to using plain text:

- It may take more space to store than a compressed binary format
- It may be computatioanlly more expensive to interpret and process a plain text file

- The power of text
- Insurance againts obsolesence
- Leverage
- Easier testing
- Shell game
- GUI interfaces are wonderful. But if you do all your work using GUI, you are missing out on the capabilities of your environment. You won’t be able to automate common tasks, or use the full power of the tools available to you.

A benifit of the GUI is WYSIWYG-What you see is what you get. The disadvantage of the GUI is WYSIAYG-What you see is all you get.

The shell is your friend.

## Debugging
*SELECT isn’t broken*

It is a painful thing. To look at your own trouble and know that you yourself and no one else has made it.

*Psychology of debugging*
Embrace the fact that debugging is just a problem solving, and attack it as such.

It doesn’t master whatever the bug is your fault or someone else’s. It is still your problem.

Fix the problem, not the blame.

## A debugging mindset
The first rule of the debugging: Don’t Panic

Before starting debugging, turn off many of the defenses you use each day to protect your ego, turn out any project pressures you maybe under, and get yourself comfortable

If your first reaction on witness a bug or seeing a report is “that’s impossible”, you are plainly wrong. Don’t waste a single neuron on the train of thought that begins with “but that can’t happen” because quite clearly it can and has.

*Where to start*
Make sure you are working on code that compiled cleanly - without warnings. Set compiler warning level as high as possible. It doesn’t make sense to waste time trying to find the problem that compiler could find. We need to concentrate on the harder problem at hand.

Unfortunately, bug reporting isn’t an exact science. It’s easy to be misled by coincidences, and you can’t affort to waste time debugging coincidences. First, need to be accurate in your observations.

*Debugging strategies*
Once you think you know what is going on, it’s time to find out what the program thinks is going on.

- Visualize your data: get a good look at the data it is operation on
- Tracing: watch the state of the program over time.
- Rubber ducking: explain it to someone else
- Process of elimination: SELECT isn’t broken

## Chapter 4: Pragmatic paranoia
You can’t write perfect software

The analogy with coding is pretty obvious. So we are taught to code defensively. If there are any doubt, we validate all information we’re given.

## Chapter 5: Bend, or Break
Life doesn’t stand still. In order keep up with today’s near-frantic pace of change, we need to write code that as loose - ass flexible - as posible. Otherwise, we may findout code quickly becoming outdated.

### Decoupling and the Law of the Demeter
`Minimizie coupling`
Need to be carefule how many other modules you interact with, and more importantly, how you came to interact with them.

### Metaprogramming
Everytime we have to go in and change the code to accommodate some change in business logic, we run the risk of breaking the system - of introducing a new bug.

So we say “out of the details”, get them out of the code. While we’re at it, we can make our code highly configurable and “soft”-that is easily adaptable to changes.

### Dynamic configuration
We want to make our systems highly configutable. Not just things such as texts, colors, but deeply ingranted items such as algorithms, database products, middleware technology,…

Configure, don’t integrate

Use metadata to describe configuration options.

### Metadata-Driven Application
Our goal is to think declaratively, and create highly dynamic and adaptable programs. We do this by adopting a general rule: program for the general cases, and put the specific somewhere else - outside the compiled code base

Put abstractions in code, details in metadata

Define most details untils the last moment, and leave the details as soft as posible.

## Chapter 6: While you are coding
Avoid programming by coincidence-replying on luck and accidental successes-in favor of programming deliberately

### Program by Coincidence
Doesn’t know why the code is failing because didn’t know why it worked in the first place.

### Accidents of Implementation
It’s easy to be fooled by this line of thought: “It works now, better leave well enough alone…”

### Implicit Assumptions
It’s easy to assume that X causes Y. DON’T ASSUME it, prove it.

### How to Program Deliberately
- Always be aware of what you are doing
- Proceed from a plan, whether that plan is in your head, on the back of the cocktail napkin, or on a wall-sized
- Rely on reliable things
- Dont be a salve to history
- Algorithm Speed: there is a kind of estimating that programmers use almost daily -> estimating the resources that algorithms use - time, processor, memory, and so on.

It’s a good idea to make sure an algorithm really is a bottleneck before investing your precious time trying to improve it.

### Refactoring
Change and decay in all around I see

As a program evolves, it will become neceessary to rethink earlier decisions and rework portions of the code. The progress is perfectly natural.

### Evil Wizards
Don’t use wizard code you don’t understand
