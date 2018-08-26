# App Store vs Google Play #

A Dark Room is (finally) on the Google Play Store. I've waited a few months to write this chapter primarily to gather as much data as possible before reaching the following conclusion:

Deploy to iOS first. There, you'll have your best chance for your mobile game to succeed. Revenue on iOS is 3x to 10x higher on iOS for what I've observed in the past six months. Other games Monument Valley, Badlands, Alto's Adventure, Heads Up! have seen similar breakdowns in revenue when comparing App Store to Google Play.

My most direct advice is:

>Keep it simple. Don't worry about going cross platform for now, just make sure your game runs well on an iPhone 5s and get it to the App Store as quickly as possible. Iterate publicly, listen to the feedback the reviews give you. From there, you can decide if you want to take it to Android. I can't recommend with clear conscience going in the other direction, even though the development environment and devices are much much cheaper (and free to some extent).

So, buy a Mac and get to work. Target iOS only. After you're done building the iOS version (and have some revenue numbers), take the annual revenue potential on iOS and divide by seven (divide by three if you feel hopeful). If that number is more than the cost of building/supporting your game on Play, don't build for Play. Period. Build another iOS game instead.

Each section will have the Android download numbers, historic iOS numbers, and same month iOS numbers. Honestly, no matter what angle you view it from, Android isn't viable (unless you've already had a very successful iOS deployment).

## Initial Release ##

When A Dark Room first released on Play, I expected a modest initial
number of downloads. And that's what I got the first month.

- First month of the Android release (7-2016): 3,123.
- First month of iOS release (12-2013): 698.
- Same month on iOS (7-2016): 12,100.

There was definitely some "press coverage" the first week of A Dark Room
Android's release. It took a week for the game to be searchable in the
Play store. After that, /r/AndroidGaming picked up the news and I got
a good bump for about a week. A total of 1,700 downloads came
from
[that Reddit post](https://www.reddit.com/r/AndroidGaming/comments/4qzbyw/a_dark_room_is_now_on_android/).

## Leveling Out Period ##

Each month contained "spike" events (which I'll talk about later). But
before I talk about that, I wanted to find a long enough steady period of time to
see what my "low end" looks like. Generally speaking, when these
"spike" events occurred, the Web, iOS, and Android versions of ADR all
benefited.

- Leveling period on Android (8-29-2016 to 9-20-2016): 583.
- Month two and three on iOS (1-2014, 2-2014): 981, 2,580.
- Same period on iOS (8-29-2016 to 9-20-2016): 10,600.

Not sure what to say honestly. After the initial hype died down about
ADR on Android, I'm left with 583 downloads while iOS (for the _same_
time period) gets _eighteen times_ the number of downloads. Also,
month two to three on Android was _lower_ than month two to three on
iOS back in 2013: 981 and 2,580 (keep in mind no one knew about ADR
iOS). Guys and gals, no matter how you slice these "leveled off"
numbers, Android loses. Android loses. Do not build your game solely
for Android. You will make an _order of magnitude_ less than on iOS.

## Marketing Bumps and Decay Time ##

There were two occasions during this the first five months of Android
that ADR got some good
notoriety. Specifically
[this BuzzFeed article](https://www.buzzfeed.com/chelseypippin/7-things-you-really-need-to-check-out-this-week?utm_term=.evN1NpY2Q#.ubpGlMBP6),
and
[this /r/AskReddit post](https://www.reddit.com/r/AskReddit/comments/5gzzwb/what_is_the_best_browser_game_to_play_at_work/dawfki4/). During
this time period, all versions of ADR saw significant spikes over
their daily averages. Here is the revenue captured the day of and five
days after.

Downloads from BuzzFeed Recommendation:

- First day spike and next five days on Play: 25, 331, 38, 25, 25, 24, 44
- First day spike and next five days on iOS: 455, 549, 590, 461, 475, 443

Both Android and iOS saw a spike, albeit Android shot up big time (but
fell just as quickly).

Downloads from /r/AskReddit post:

- First day spike and next five days on Play: 30, 288, 351, 117, 111, 92, 92
- First day spike and next five days on iOS: 125, 656, 329, 296, 292, 240, 224

I love Reddit. Reddit loves ADR. But as you can see, the numbers just
aren't as high on Android.

## ADR on Play Hits the Number 5 Spot in the Game Category ##

This was of course an exciting time when ADR started climbing the Play
Store. Here are the numbers for its rise.

- Rise to the #5 spot under the game category (few days before and
  the point at the #5 spot):
  - 40
  - 34
  - 30
  - 174
  - 227
  - 388
  - 508 ADR as #5 game on Play
- I went back through my iOS revenue to see what I was pulling in at
  the #5 spot on iOS back in the day:
  - 1,600
  - 2,400
  - 2,000
  - 1,960
  - 2,300
  - 4,100
  - 6,200 ADR as #5 on iOS

I'm not sure how many different ways I can show you how much your
limiting the success of your game by deploying to Android only. There
is a _10x_ difference in revenue at the _same_ spot.

## Why I Waited So Long to Get on Play ##

The framework I was using didn't gain support for Android
until 2015. And during that time, [I was buckling down to pay off a
house so I can take some more time off](https://www.indiehackers.com/businesses/a-dark-room).

## Multi Platform Deployment is Hard ##

Even if the framework you choose supports multiple platforms,
supporting Android just isn't fun:

- You have vendor fragmentation (both OS and device). Why are there
  devices out there that are five versions behind on Android? This
  doesn't happen on iOS.
- There are some really slow ass Android devices out there. You'll end
  up changing parts of your game to get it working on this slower
  devices, or feel the wrath (entitlement) of these individuals when
  they give you a "well deserved" one star review.
- Refunds have to be processed by you, the developer. It's just
  infuriating to get an email from someone to get a refund for a one
  dollar game. I never say "no" of course, it's just frustrating.
- You won't be able to share all the code you write on both platforms
  (or worse, you'll have two completely different code bases to support).

## Final Thoughts ##

Do I regret deploy to Android? Nope. Over the five month period, I've
made $12,717. That's a good chunk of change. But, during that same
time period, I've made $57,600 on iOS. **Once you're at these kind of
levels, of course you should deploy to Play. But if you're just
starting out, with no idea if your game will be successful, _cut the
Android overhead and get your game out on iOS_**.
