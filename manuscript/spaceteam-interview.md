# Interview With Henry Smith - Spaceteam

My first time playing Spaceteam was during a lunch break. We got a
quick bite to eat and got on the topic of indie games. At which point,
he told me to download Spaceteam to play a quick round. Usually, when
a friend recommends a game to me (paid or free), I buy it. This game
was espcially easy to convice me of because it was free. I immediately
saw the "character/the developer's mark" as soon as I opened the
app. After hearing Spaceteam "theme" song, I was an instant fan of
anything Henry creates.

>How old are you? What's your professional and educational background?

I'm 37 years old. I've been designing games as a hobby since I was a
kid. First it was board games and card games. Then I started playing
with HyperCard on the family Mac Plus. I made and published my first
real shareware game at 15 (it was called "Squish"). Then I got a
Computer Science degree and worked in the AAA game industry, at
Irrational Games and BioWare, for about 10 years before going indie.

>What technologies/frameworks did you use to build Spaceteam?

The first version was iOS only and used the Cocos2d sprite engine and
native Objective-C code. I used the `CocoaAsyncSocket` and `HHServices`
libraries for networking.

Shortly afterwards it came to Android thanks to another company,
Apportable, using their custom technology to create an APK from the
iOS source code.

Now, many years later, I'm completely rebuilding the game in Unity
using C#. I'm using a bunch of libraries from the Asset Store. I'll
release a full list on my blog/website when the new version launches
in a few weeks.

>How long did it take to build?

The original iOS version took 3 months to build. But since then I've
spent the past 3+ years supporting the game, adding new features,
building a community, and creating spin-off projects.

The Unity rebuild is almost finished and took ~6 months to build. I
was learning Unity as I went and had to incorporate all the changes
and upgrades that the game has seen since it's initial release.

>How big is the code base (lines of code that you wrote)?

This is the first time I've counted them so this was interesting to
me!

Original game: 49k lines of Objective-C/C++

New Unity rebuild: 20k lines of C#

It's worth noting that this isn't an exact comparison because some
assets/data that were originally in code are now stored in other ways
in the Unity project.

>How much lifetime revenue (gross) has the game generated on iOS?

iOS In-App Purchase revenue: $38,131

However the game was also mostly responsible for:

- A successful fundraising campaign on Kickstarter ($83k)
- Prize money ($7k)
- Commissioned spin-off projects (~$22k)

>How much lifetime revenue (gross) has the game generated on Android?

Android In-App Purchase revenue: $18,836

Humble Bundle sales: $11k

>During the sale and development of Spaceteam, what was one of your
>happiest moments?

My happiest moments are interactions with fans:

- When I discovered the first piece of Spaceteam fan-fiction :-)
- Getting hugs and high-fives and autograph requests (!) from fans at festivals

>Your saddest moments?

My saddest times have actually been the last few months. For a long
time I was looking forward to moving on from Spaceteam to new games,
and the unexpected rebuild set me back longer than I wanted. It's also
pretty unmotivating to remake the the same game again. But the end is
in sight!

I also remember a particularly gut-wrenching moment. We were cleaning
up our exhibitor booth at PAX East in Boston and were told by a
passing stranger that Spaceteam was being used as the secret final
round of the Omegathon competition. It was being played live, as we
spoke, by two teams on stage in front of thousands of attendees. We
quickly opened a laptop and managed to get a livestream of the event,
only to see it start disconnecting again and again in the middle of
the game. It was painful to watch but also thrilling at the same time!

Luckily I think most people blamed the network conditions rather than
the game itself and the end result was pretty positive.

>What tips do you have for those that are just starting with
>programming and game development?

Start small and triple your estimates. Everything takes longer than
you think.

When I first quit my industry job I had stars in my eyes and wanted to
make an ambitious space-exploration game with a procedural world and
modular ships and interesting encounters and multiple ways to play (I
still want to make this game...)

But instead I forced myself to make a tiny practice project to learn
and grow from. That ended up being Spaceteam. It was the best decision
I ever made.

>We may have a couple of project managers reading this interview. Any
>tips for them with regards to managing a project/interacting with
>developers?

I'm not managing anyone now, but I did lead a small team at
BioWare. My advice shouldn't come as a surprise: give people as much
autonomy as you can, ask them what they want to be doing, prefer
positive feedback to criticism (even if you think it's constructive).

>Also, we may have a couple of ad men reading this interview. Any tips
>for them with regards to marketing a game?

I have no clue about marketing. I never did any paid advertising for
Spaceteam, just shared it with industry connections and on social
media. I also kept a development blog and entered some
competitions. It grew organically from there.

I did try various other things: cold-emails to press, reddit AMAs,
etc. but it's so hard to measure the effects of these things.

>You went with a free game with IAP (just wanted to say you've done it
>tastefully), any thoughts on this model vs premium? Why free and not
>paid?

From the beginning I had planned the game to be a free teaser project
to get my name out there. I had some savings and I never expected to
make any money with my first game. I added the "tip jar" IAP mostly as
a last-minute experiment so that people could support me if they
really liked the game.

But in retrospect free seems like the best model for a
multiplayer-only game like this. I think making four friends all pay
$1 just to try a weird new game would have severely hindered adoption
and growth.

I've always disliked ads and I was very sensitive to not being
exploitative with micro-transactions. I want to keep my next game free
as well if I can.

>Given hindsight is 20/20, would you have done anything differently
>with regards to building and selling Spaceteam?

Difficult question since Spaceteam was a much bigger success than I
expected and it's hard to tell which parts of its trajectory were
important to this. There are a couple of specific projects that I
probably would have said "no" to, but everything was so context
dependent that I'm not sure I learnt any lessons I can apply
elsewhere.

>Any "must do this or don't come crying to me" kind of stuff?

As a new indie it's so easy to be seduced by the idea that you can do
everything. Swallow your pride and start small.
