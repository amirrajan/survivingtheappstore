# Interview With Ryan McLeod - Blackbox

I actually heard about Blackbox during an interview/podcast called
iPhreaks. At the end of the podcast we gave our "top picks". The
cohost talked about Blackbox and how awesome it was (word of mouth
recommendations are incredibly powerful, so don't underestimate
them). Additionally each connection you make is a long unforseen chain
of events that could lead to something important, so pursue
_everything_ if you can (especially at the beginning). For me it was:

- Having lunch with a friend who told me about an iOS Remote
  Conference that was looking for speakers.
- Me taking the time to submit a talk (it got accepted).
- Me giving a good presentation.
- The facilitator of the conference liking the presentation and
  inviting me to talk on his podcast (iPhreaks).
- Me saying yes and actually doing the podcast.
- Him recommending Blackbox on the podcast as one of his top picks.
- Me downloading it (and loving it).
- Me hunting down Ryan on Twitter and asking him if he wanted to be
  interviewed.
- Him being a good guy and saying yes. Remember what I said about
  pursuing every opportunity? He's doing that.
- 18+ email exchanges over 15 days.
- And here we are.

>How old are you? What's your professional and educational background?

I'm 25. I grew up loving computers, robotics, and design (I was pretty
convinced my destiny was to compete on Battle Bots). I got into web
design in high school and somehow landed an internship at a 50 person
web start-up. After high school I went to California Polytechnic San
Luis Obispo for a BS+MS in Computer Science. Low-level C and assembly
wasn't really my passion so I spent a lot of time goofing off trying
to gain design skills and learn more about user experience concepts on
the side. When our school offered a new iOS development class I was
one of the first people to sign up. I actually got to show my final
app in that class to Peter Oppenheimer (former CFO of Apple). After
that I interned at Apple and then Airbnb doing web work, but learned a
ton about design too. Once I graduated I tried my hand at a music
discovery start-up with some friends, consulted some start-ups, and
decided it was now-or-never to try to learn iOS and try creating this
idea of a "blackbox" game.

>What technologies/frameworks did you use to build Blackbox?

Hah, Blackbox is built almost entirely with native cocoa/UIViews and
is written in Objective-C (when I started Swift was still very
young). I didn't realize building a game with native views wasn't
normal until I got called crazy a few times. I think the naivety paid
off though. Blackbox is working creatively within constraints and if I
had used a proper framework like cocos2d or SpriteKit I think the game
would have lost a lot of its unique look and native feel. Beyond that
Blackbox relies on almost every sensor API the phone has to offer and
a dozen or so third party libraries to help me keep my sanity (I still
had to learn how to patch together a pitch detection algorithm
though). Along the way I've built a handful of mini-libraries that
have made Blackbox a lot easier to expand, including a modal card
library, a permission management system, and an interesting time
tracking (cheat-prevention) system. Would love to open source some
when/if things calm down.

>How long did it take to build?

A little over a year ...but I was also learning iOS/Objective-C along
the way. I've gotten a lot faster.

>How big is the code base (lines of code that you wrote)?

Excluding all 3rd party code and blank lines Blackbox is comprised of
35,730 lines spread over ~600 Objective-C files (half are headers of
course). An additional 7,333 lines are comments! I like comments. (The
entire binary would likely be less than 2MB but offline speech
recognition makes the whole thing swell to around 45MB.)

>How much lifetime revenue (gross) has the game generated on iOS?

((((( After Apple's cut, right? revenue/profit/gross always trip me up
))))) $32,000 in the 5 months since launch February 25th, 2016. Keep
in mind that $15,000 of that was made in the first two weeks (Blackbox
was featured in Best New Games during the first week). Don't
underestimate the long tail.

>During the sale and development of Blackbox, what was one of your happiest moments?

It's hard to choose just one! I've wanted to become "an iOS developer"
since the App Store opened. There was a point amid the week long blur
of launching when I realized I had become exactly that—I was pretty
giddy.

Besides that, reading the reviews and talking to players has been
incredible. I'll never be able to really play the game and get the
same enjoyment from it as my players do so I get to live vicariously
and it's glorious. So many games have made strong impressions on me
over the years and now I get to do the same. Getting to hear all the
stories and see pictures of mountains players have climbed, planes
they've flown, perfect pitch they've sung, or crazy weather balloon
purchase they've almost made all to solve Blackbox challenges is
always moving. One woman messaged me from the side of a mountain; she
had just ran out the door to drive up in the rain–to the confusion of
her husband–so she could "fill in this last little unfilled box."

The game's voice is my voice and I try to be pretty accessible to my
players; those who get far enough in the game get a direct line to me
too :) It can be overwhelming but it provides constant motivation to
get back to work!

>Your saddest moments?

Probably when people started trying to scam me. It was the first week
and this one person came up with an elaborate story of how they had
dropped their phone in a pond and the insurance company just replaced
it and could I please unlock the paid levels for free. I asked when
she had bought it and she said a week or so ago; the game had launched
a day earlier. I called her out and we had a funny chat, but that
happened A LOT. Sometimes I'd try to explain that without charging a
dollar and change I'd have to put ads in or charge for the app upfront
and people would get mad! Some people still suggest in the reviews
from time to time that I add ads. I refuse.

I wanted as many people as possible to be able to enjoy Blackbox for
free and pay for a small percentage of extra levels if they were
really into the game and wanted to support it. The lengths people will
go to to save $1.99 was really disheartening, especially when I see
players who've completed every level EXCEPT the paid ones. I know
they'd enjoy them, but...

>What tips do you have for those that are just starting with
>programming and game development?

Do not move fast and break things. Some features might need to scoped
down, you may need to stop yourself from "gold-plating", or avoid
over-eager optimization, but don't pass up opportunities to learn and
to do it right. I think I'm a pretty slow programmer, but that's in
part because when I run into something I don't understand, or feel
"there has got to be a better way", I generally stop, go online, read
up, talk to a friend, and try to learn how to do it right. It's a
great way to build your skill-set while developing not to mention
you'll end up with a more solid codebase that you don't abhor
maintaining.

>We may have a couple of project managers reading this interview. Any
>tips for them with regards to managing a project/interacting with
>developers?

Hard to say... Blackbox never had a solid schedule and my meandering
direction and focus led to some of the most cherished parts of the
game. At a scale requiring project management, it's probably important
to let some wandering happen while keeping a finger on what
matters. When it comes down to it, there are always things worth
cutting or skipping but always step back and choose based on what the
player will notice and care about; analytics can be your barometers
but never let them be compasses.

Don't underestimate finesse. The extra day or two (or three) it takes
to add a gesture based transition or a downpour of confetti may not
seem worthwhile but it's the subtle things that sometimes create
guttural pleasure and attachment between player and game. That said
don't overestimate finesse either—just because the details are
beautiful or unique doesn't mean the game will be a success. The core
game has to be intriguing and fun, after that it's the details that
will make it beloved.

>Also, we may have a couple of ad men reading this interview. Any tips
>for them with regards to marketing a game (your in game advertising
>techniques are phenomenal btw)?

Thank you! Most smartphone users download an average of 0 apps a
month. Those that are downloading new apps are strongly influenced by
word of mouth so enabling and exciting your players to help you and
themselves by sharing your app is incredibly important! As an indie
you can't bank on broadcast methods so standing out and being creative
is key.

In Blackbox there are many ways to share screenshots of your
progress. Players that successfully refer a friend are rewarded with a
free hint and thanked (with trademark Blackbox snark). If they open
the sharing dialog and cancel I let them know that if they ever change
their mind in the future there's a new challenge waiting for
them. There's even some fun sass if I catch you trying to cheat the
sharing system. The placeholder share text is also tailored to each
sharing platform to be as easy as possible to blast off to friends and
not feel spammy. I try to make sure sharing or following never seems
forced or punitive, and instead try really hard to make it desired and
fun. Part of this involved letting the game's voice be my own instead
of a brand, which helped set apart the game, connects players, and
seems to make them more forgiving.

In addition to explicit and obvious sharing mechanics, parts of the
game are designed as more subtle conversational pieces. Did I really
need to add a fourth distance challenge that's 1000km away? Lol. Do
people talk about it a lot? Definitely.

>You went with a free game with IAP (just wanted to say you've done it
>tastefully), any thoughts on this model vs premium? Why free and not
>paid?

I've always been a premium advocate, but then I realized how
influential shareware/demo software was to me growing up: I must have
played the Starcraft demo campaign a hundred times over; I used
Sublime unpaid for years; I don't need to say anything about
Photoshop. I wanted as many people as possible to be able to play
Blackbox while still letting the people that love supporting good
software chip in without it feeling like charity. Freemium comes in a
dozen different colors and I've changed course over the years and
realized not all forms are bad. I also wanted it to be easy for people
to get their friends to download the game. How often do you get a
recommendation for an app but you hesitate downloading it because it
isn't free? I wanted to make downloading it a no-brainer, especially
since Blackbox is hard to explain without spoiling it! I needed to get
people in the door as soon as they were intrigued and not a minute
later. Could I be making more daily with a paid app? Maybe—but it
hurts me to imagine the number of people who would never get to enjoy
any of it. I on a bit of a mission to show that IAP can be done well
and be sustainable even without using ads for non-paying players.

>Given hindsight is 20/20, would you have done anything differently
>with regards to building and selling Blackbox?

I think things went pretty well. There isn't much I would change but I
definitely wish I had spent less time on certain things like a solar
path that is accurate to your location on the globe—that took way too
long and I don't think anyone has noticed except for those on the
equator that get to experience an interesting graphing bug.

>Any "must do this or don't come crying to me" kind of stuff?

Test your game, then swallow your hubris and listen—really
listen. Blackbox was continuously in beta for a year. Originally I
just shared with friends, but the group grew to over 500 people by
launch. Email feedback was okay but it came with the formal
intimidation of email. I eventually built in a great chat system using
smooch.io, this made giving and getting feedback so seamless that I
could hear everything. Sometimes you don't want to hear everything,
but you have to hear everything. Sometimes feedback feels mean, it
goes against your sensibilities, your design, what you wanted. When
two people have trouble with the same thing, it's likely not their
fault, it is yours. That doesn't mean you take every suggestion you're
presented with, you must differentiate between what's immediately
important and what are good ideas to hold onto and consider, but don't
be hurt; be thankful, iterate, and test again. Follow up, ask
questions, thank, and make your testers feel appreciated and
comfortable. It'll pay off in multitudes.
