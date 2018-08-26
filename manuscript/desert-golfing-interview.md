# Interview With Justin Smith - Desert Golfing

I played this game way too much. Desert Golfing is a true testimate how
building with constraints in design can acomplish (that plus you don't
need to be an amazing artist to make a successful game).

>How old are you? What's your professional and educational background?

I'm 39. I graduated with a degree in computer science in 1998 and
immediately got a job in triple-A games. I worked for about 9 years
before going semi-indie. Being semi-indie means I split my time about
50/50 between working for small studios and working independently.

>What technologies/frameworks did you use to build Desert Golfing?

Desert Golfing was made with my own C++ game engine. I call it the
Crusty engine. It started life as something I downloaded off the
Internet called Haff's Game Engine. I added OpenGL, Box2D physics, iOS
and Android code, and lots of other stuff, all held together with
bubble gum.

>The physics in Desert Golfing are so nice. The game as a whole is
>almost peaceful (I'm on hole 4494 by the way). How did you go about
>perfecting how the game "feels"?

Desert Golfing is about the 20th game I've made with Box2d
physics. Practise! I'm getting good at knowing all the right friction,
density, impulse, and dampening parameters I need to get the feel I
want. Little things are also very important, like how the ball sinks
into the sand, and how the platform rises so satisfyingly. I sensed
early on that Desert Golfing was developing a very zen like feel, so I
made sure not to add anything that would ruin it like flashy effects
and juice.

>How long did it take to build Desert Golfing?

It took 2 solid weeks of dedicated don't-bug-me-I'm-coding coding,
plus about a month of more casual testing, tweaking, bug fixing, and
porting.

>How big is the code base?

About 4500 lines of code that I personally wrote (engine code plus
golf code), not including library code.

>How much lifetime revenue (gross) has the game generated on iOS? On
>Android?

I little over 100k on iOS and half that on Android. I'm really happy
that Android is genuinely worth it now. I was also really happy how
the Canadian Dollar tanked at the perfect time.

>During the sale and development of Desert Golfing, what was one of
>your happiest moments?

Seeing how obsessed people got with the cactus. It's just what I was
hoping for. And the gradual palette transformation. Someone made giant
grid of two thousand holes all pasted together and it looks really
lovely.

>Your saddest moments?

This is an easy one. All the Android bugs. There's still something
critically wrong with my save/load code that causes the ball to get
stuck inside the terrain occasionally.

>What tips do you have for those that are just starting with
>programming and game development?

This will seem at odds with "the saddest moment question", but my answer
is to embrace awful code. Your game just needs to get out the
door. There's a tendency to look for the best, most elegant way to
solve a problem. Most of the time that elegant solution has just as
many unknown problems as your naive solution. You're trading a bunch
of problems you know about for a bunch of problems you don't know
about. And sometimes trading simplicity for complexity.

>Also, we may have a couple of ad men reading this interview. Any tips
>for them with regards to marketing a game?

I don't have tips for ad men, but for other indie devs who are
clueless about marketing, my one tip is this: find interesting stories
about your game, or failing that, invent them. If you get asked a
question and the truth is boring, make something up, stretch the
facts. You're in the entertainment business.

>You went for a premium game as opposed to a game that was free with
>IAP. Why?

Be the change that you want to see in the world. I personally hate
looking at ads, and I hate games with micro transactions. I do like
the idea of a one-time IAP to unlock levels in a game, but the
minimalist aesthetic of Desert Golfing forbade it.

>Given hindsight is 20/20, would you have done anything differently
>with regards to building and selling Desert Golfing?

I would have thought more about an ending. I had no idea people would
want to play 10000+ holes. Originally the game ended at around hole
3000 with an infinitely long flat desert. I did an update to make the
game keep going until an impossible hole was generated. But this only
switched things from one anti-climactic ending to another. With
regards to selling the game, I should have tried to get it on Steam.

>Any other tips? EG: Any "must do this or don't come crying to me" kind of stuff?

This is Justin's secret miracle tip: Have a line of code in your game
that looks like this: `if Random(10000)==0 { do fun stuff }`. Games are
about systems, but often the idiosyncrasies are what people remember.
