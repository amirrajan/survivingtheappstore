# Get Started with Game Dev When You Don't Know How to Code

**tl;dr;**

It can be paralyzing when you look at how to get started. What
language do you learn? What framework should you use? What editor
should you use? What network/server stack should you use? How much will
all this cost?

Well, here's the answer: Use JavaScript, jQuery, HTML, CSS, and
Canvas (Pixi.js) for your front end. Use Sublime Text 2 for your
editor. Use NodeJS for your back end. Use Heroku for your host (it's
free).

The emphasis with this development stack is on an incredibly fast
feedback loop. JavaScript deemphasizes type theory, performance, and
memory management. For your first game, you really don't have to worry
about this stuff. With these advanced concepts deemphasized, you can
concentrate on just getting familiar with programming and getting your
ideas on a page that you can show off.

**inb4**

>Just use [Unity](https://unity3d.com), it's easy.

>Just use [Unreal Engine](https://www.unrealengine.com/blog), it's easy.

Two things:

1) You can make wonderful things with
[insert awesome framework, widely advertised platform]. But, at the
end of the day, these are all complex beasts with their own unique
takes on how to approach game development (using their Integrated
Development Environments, language, and programming constructs). When
you're just starting with game development, it is incredibly
overwhelming to navigate these IDE's. So, for now, hold off on these
platforms. It's just too much to take in when making your first game.

2) Brick walls are rampant in these framework. You end up watching a 5
minute tutorial video and see how you can "Create this awesome 3D FPS
by just dragging and dropping stuff and 5 lines of code!". You follow
the video, and get their sample up and running... but then what? A lot
of the demo videos out there go for "wow factor" as opposed to
teaching fundamentals.

To elaborate on this: A friend of mine went into the digital arts. The
first things he was told to do by his professor was to draw a perfect
circle and straight line by hand. Can you imagine how boring that
would be to practice? My friend saw all the glam and glory with being
godlike with Photoshop, he gets to class bright eyed and bushy
tailed, and is told to bring out a piece of paper and a pencil to
draw rudimentary shapes. Every craft is like this. You have to have a
good grasp of fundamentals before you can start using tools to augment
that solid foundation. Large frameworks with "batteries included"
don't teach you these fundamentals (they teach you how to use _their_
product).

>Your recommendation of JavaScript (jQuery), HTML, CSS, Canvas, etc
>is terrible. No real games use these frameworks.

You can get pretty damn far using this tech stack. Here is a Dive Kick
clone I made in about a week:
[Gameplay Gif](https://gfycat.com/SingleJauntyAmazonparrot),
[Source Code](http://github.com/amirrajan/nodekic).

Look, I'll be the first to say that JavaScript is a _terrible_ language. It
was built in 10 days, by a guy in a basement, after he broke up with his
girlfriend. It has the most ridiculous value coercion issues I've ever
seen in a language (among other things). [This lighting talk by Gary
Bernhardt titled Wat
enumerates the sheer insanity of JavaScript](https://www.destroyallsoftware.com/talks/wat). But,
this stack that I'm recommending will give you an extremely fast
feedback loop. It'll let you get a grasp of some programming
_fundamentals_, and then provide you a bridge to a "real" game
development stack.

>You don't need learn to code to build a game. I just used th-

Yes. You do.

>No really, you can get pretty far without knowing how to program if you
>j-

No. Stop. You need to have a good grasp of fundamentals. You can't
short cut this process (if you try you'll hit that wonderful brick wall).

##Words of Warning

**Coding Isn't Easy**

You have got to work at it. I started dabbling with computers when I
was in 8th grade (1997-98). I had to learn how to code using Turbo
C++, Visual Basic, a shit IBM Aptiva, and a library card (get off my lawn). You
whippersnappers just don't know how easy you have it with regards to
instant access to resources.

With the world at your fingertips, it still takes an
immense amount of practice, trial/error, and persistence to really get
the hang of coding. You just can't learn this stuff in a short period
of time. Coding didn't really click for me until I was a Senior in
highschool. You have to comb through the same concepts over and over
again. And frankly, no one will hold your hand. As with this entry,
I'm going to point you to some resources, give you some simple
programs to make, but it's up to _you_ to read, ask questions online,
and do the work.

**Coding is a Lifetime of Learning**

Coding, game development, software development (any craft) requires a
lifetime of learning. Every time I look up, some new
framework/language/network stack has come out (and needs to be
learned). It's an endless cycle of feeling like a god, to feeling like
a complete idiot, and back again. You'll face countless hurdles to get
something working, everything will be rainbows and unicorns for a
split second, and then you'll be confronted with another set of
hurdles to overcome. Once you feel you've figured everything out, you
find that a new game-changing tech is just over the horizon... sending
you back to square one. If you don't love doing that, this is the
wrong profession for you.

##Setting Up Your Environment

These steps will hopefully get you over the first few hurdles of
game development. All this is completely free. So don't worry about
having to pay if you can't afford to.

Download [Sublime Text 2](http://www.sublimetext.com/2): this is a
very nice looking editor and will be plenty sufficient for the code
you'll be writing here.

Register a username on [GitHub](http://github.com): all the code I
will point you to is on GitHub. This is where you'll "back up" all of
your source code. When you register on GitHub, use a professional
username. You can consider this as your public portfolio that
potential employers may look at.

Install [NodeJS](https://nodejs.org/en/): this is the language/runtime
you'll use to work through the programming problems below.

Install [Redis](http://redis.io): The
[Windows Install](https://github.com/MSOpenTech/redis/releases) can be
a little tricky. So if you can't get it to work, don't worry about it
just yet.

Install
[Chrome](https://www.google.com/chrome/browser/desktop/index.html):
This (and Firefox) are the browsers for developers. The thought of
supporting Internet Explorer and Safari give me nightmares (the former
more so than the latter).

##Your First "Games"

Create a file on your desktop called `index.html`, and
put the following lines in it:

    <html>
      <head>
        <title>My Game</title>
        <script src="http://code.jquery.com/jquery-2.2.0.min.js"></script>
      </head>
      <body>
        <div id="hello-world" style="display: none">
          Hello World
        </div>

        <button id="click-me-button">click me</button>

      </body>
      <script>
       $(function() {
         $("#click-me-button").click(function() {
           $("#hello-world").show();
         });
       });
      </script>
    </html>

Open the file up in Chrome and see the magic happen.

Great! Now,
[using the resources here](http://learn.jquery.com/about-jquery/how-jquery-works/). Complete
the following programs. You'll need to Google, use StackOverflow,
read, read some more, and try writing stuff. I'd recommend skimming
all the content on learn.jquery.com frankly (especially
[Events](http://learn.jquery.com/events/) and [Effect](http://learn.jquery.com/events/event-basics/).

Remember the story I told about my friend having to draw a circle and
a straight line before he could use Photoshop? Well this is your
(boring) trial by fire.

###"Game" Number One

Write an html page that has an `input` text box, with a `placeholder`
asking the user to enter their name. After they have entered their
name, the user can click a button. Once the button is clicked, an
`alert` box pops us saying "Hello, [Name]".

Enhance the webpage so that "Name is required." is displayed in the
`alert` box if the user doesn't enter a name.

Enhance the webpage so that instead of throwing up an `alert` box, a red
error text is displayed above the text box, if they fail to enter a
name.

Enhance the webpage so that instead of throwing up an alert box for
saying hello, text is displayed on the page in green (below the text box).

###"Game" Number Two

Write an html page that shows a `table` with 3 rows and 3 columns. When
a user clicks in any of the table cells, the color of the cell changes from
white to black.

Enhance the program to toggle between white and black. If a white cell
is clicked, it turns black. If a black cell is clicked, it turns white.

Enhance the program to print out all the colors of each square after a
square has been clicked (below the table in an `unordered list`). For example:

    - Row 0, Column 0 is white.
    - Row 0, Column 1 is black.
    - Row 0, Column 2 is black.
    - etc.

Enhance the program such that if all squares in a row are black, the
`unordered list` contains an "All squares in row X are black." entry
(along with color information for each square).

Enhance the program such that if all squares in a column are black, it
prints out "All squares in column X are black." (along with color
information for each square).

Enhance the program such that if diagonals are black it prints out
either "The left to right diagonal is black." or "The right to left
diagonal is black." or "Both diagonals are black." (along with color
information for each square).

Can you make this into Tic Tac Toe? Do that now. Break down the
problem step by step like I did for you. Seriously, do not move onto
the next program until you've built a fully functional Tic Tac Toe
game with win conditions (you don't have to worry about creating an
AI, just assume it's two players).

###"Game" Number Three

Write an html page that shows a table with 10 rows and 10
columns. Clicking on a column adds a black square to the _top_ row of
that column (regardless of what row within the column is clicked).

Using JavaScript's `setInterval` function. Every 1000 milliseconds, black squares
should "drop down" a row until they hit the bottom row, or another black square.

If an entire column is filled with black squares, all black squares in the
column are removed.

Save the current state of the game to `localStorage`. This means that
if I close the page and bring it back up, the grid will be just the
way I left it.

Make this into a two player Connect Four with win conditions.

Make this into Tetris like game where you control 2 by 2
squares that drop from the top randomly. Use [keymaster.js](https://github.com/madrobby/keymaster) for keyboard input.

Doing these exercises are important. It'll help you create realistic
time lines for your future projects. It's very hard for a seasoned
developer to take someone seriously when they say:

>I'm just starting to get into game development. I'm thinking of
>making a MMORPG. I'm setting my timeline to two months. I should be
>able to get it done. How hard can it really be? Any tips on getting started?

In all honesty, I think it'll take you about that time to just create
Tic Tac Toe, Connect Four, and Square Tetris (if you're coming at this
with no development experience). So power through and finish "drawing
these circles and lines". It'll put much larger endeavors into
perspective.

##Learn How To Deploy Your Stuff

Now that you have some familiarity with JavaScript, HTML, and
CSS, let's deploy some prebuilt apps. Each app comes with a
`README`. So follow the steps and see if you can get it out there. Then
after deploying, study and dissect the code. Go through these
codebases line by line and make sure you understand _everything_ that's
in them. Maybe try to expand these apps and create your own games (all
of this stuff is released under permissive licenses, so go wild).

##Word Finder

This app lets you search the entire English dictionary for words that
match a specific pattern. It's a great little website that will "help"
you in games such as Words with Friends. Warning, don't use this to beat
your significant other. It won't end well. Speaking from personal
experience.

Word Finder is a pretty bare bones app. There is enough non-trivial code
in here for you to get a grasp on the structure of a NodeJS app, and
how you can do something useful with the platform. It uses a lean and
powerful web framework called Express and a light weight templating
engine called EJS.

[Instructions and source code](https://github.com/amirrajan/word-finder)

##Celebrity Chat

A simple chat app. Each person that comes to the page gets assigned
the name of a celebrity. You can chat with each other. Role play. Keep
it PG.

This app shows, what I feel, is the killer feature of NodeJS:
websockets. The code is fairly simple. It exchanges a few messages
with server and client in realtime. The libraries used are Express,
EJS and a websockets library called Socket.io.

[Instructions and source code](https://github.com/amirrajan/nodejs-chat)

##Cards Against Humanities

This is a port of the game Cards Against Humanities. It’s released
under Creative Commons Non-Commercial.

This app shows a non-trivial (but still simple) usage of
Socket.io. It's also mobile friendly and has fallbacks in place for
clients that have a "not so reliable" internet connection. There is
also a test suite associated with this code base using a library
called jasmine-node. [Get 3 other friends and play it here](http://nahnahnah.herokuapp.com).

[Instructions and source code](https://github.com/amirrajan/nodejs-against-humanity)

##Dive Kick Clone

This is a real time, multiplayer fighting game [currently hosted
here](http://node-kick.herokuapp.com). This codebase is a cleaned up
version of what our team built for Node Knockout 2013. Out of 385
teams, we placed 15th overall and 6th in the "fun/utility" category.

The app shows a non-trivial usage of Socket.io and an HTML5 canvas
framework called Pixi.js. The app shows how you can share common code
on the server and client (in this case the "physics" engine). It also
shows how you can use interpolation techniques to handle updates to
clients for a game that runs at 60 frames per second. You'll also get
some insight on how to create "good" NodeJS modules (when to use
JavaScript in a class centric format vs a functional format). The
commit history is fairly clean. Step through the commit history to see
how the app evolved over time.

[Instructions and source code](https://github.com/amirrajan/nodekick)

###Learn Pixi.js

The last app in the list above was created using
[Pixi.js](http://pixijs.com). Here is where you're pretty much
on your own. Go through
[the examples they have on their website](http://pixijs.github.io/examples/), and
try to build a very simple Tic Tac Toe and Tetris game.

###Learn Some Math

Knowing a little bit of Trig and Geometry can go a long way. Understanding
SOHCAHTOA and whether two rectangles intersect was all I needed to
develop [A Noble Circle](https://www.youtube.com/watch?v=aPzpfDgofu0).

##Tips Moving Forward

If you were able to get through these items. You're to a point where
you have a cursory grasp of what it takes to build a video
game. Honestly, you don't need to know a whole lot to make something
really great.

So here are some tips moving forward.

**Build Small and Iterate**

If you have a game idea, you need to have something playable in 2 to
3 weeks. Any time frame larger than this is absolutely insane for
one man/two man teams. After you get something playable, then you
can iterate on that and go for bigger goals. Don't toil away on
your game. It's so ridiculously easy to get something out there with
free hosting options/websites. So just get something out there in
the public.

For the Dive Kick clone, a team of four of us had
something playable in a weekend. Once you get the hang of this fast
prototyping spikes, you'll find that it's fairly effortless to vet a
game mechanic (and see if it shows promise).

**Learn How to Ask Questions**

Learn how to ask questions. One of the most infuriating things about
receiving a question about problem X is a generic vague
statement. For example:

>How to make an atm machine on python using functions, please help me.
>The balance should be written to a file so the next time the user logs in the balance stays the same.
>I have no idea how to start this so a start would be very useful!
>Thanks.

I (and I'm sure others) have a visceral response to this kind of
blurb. The person doesn't say what he's tried. He doesn't give any
information about what his current thought process is, or what he's
Googled for already. There is no indication that the person has taken
any time on his own to figure things out.

[Here is an example of how to ask a good question](http://stackoverflow.com/questions/17600466/using-dynamicobject-idynamicmetaobjectprovider-as-a-component-of-a-static-type). In
here I:

- State the problem and explain the motivation behind it.
- Give a means to recreate the issue in a contrived way.
- I show what I tried, what worked, what didn't.
- I ask for a specific insight.

Communication skills (like asking questions and technical writing)
will set you apart from the rest of the herd. So start working on
these things.

**Practice Twenty Minutes a Day**

Get an egg timer. Set it to countdown from twenty minutes, and write
some code. Anything. If you don't know what to write, register an
account on [Code Wars](http://www.codewars.com/), skim through some
problems, find one that looks interesting, and work on them twenty
minutes at a time.

You may be in a situation where you can't do programming full time. If
it's something you really want to persue, you have to build up the
habit. Keep improving your development skills by doing these small
problems (or working on your next idea).

**Learn Other Languages**

As I said before, JavaScript is the red headed step child of
languages. Learning other languages will give your brain some
exercise. Here are
some examples:

- Object Oriented, Statically Typed: C# 5.0, Java 8.0
- Object Oriented, Dynamically Typed: Ruby, Python
- Functional, Statically Typed: F#, Haskell, Swift
- Functional, Dynamically Typed: Clojure, Erlang
- Low Level: Go, C, C++, Objective C
- Transpiled: ES6 (JavaScript 2015), ClojureScript, Elm, PureScript
- Specialized: R, APL

SYou want to learn different _types_ of languages. For example: if you
already know Python, you probably wont gain much from learning Ruby.

All these languages may not be _directly_ applicable to game
development. But they'll give you different ways of thinking about a
problem domain. The best analogy I can think of is:

- A musical composer can't make the best score unless he understands
  how to play a lot of different instruments.
- A good League of Legends player has familiarity with all the
  champions, and knows their pros and cons (even though he only
  prefers to play with a handful).

**Stay Hungry**

You have to really dig in and want to work at this stuff. If you feel
the interest tapering, take some time to reflect. Coding isn't
for everyone, there may be other creative outlets that are better
suited for your personality.
