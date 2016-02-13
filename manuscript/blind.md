#Raising Awareness, The Blind Use iPhones

**tl;dr;**

_If you are building a native iOS app, consider making it accessible to the blind. The out of the box accessibility features of iOS devices are pretty damn impressive. The API's are simple. Use them. **You'll be surprised at how little you have to do to make your app better for the visually impaired.** I don't have any experience with accessibility on Android (yet), but from what I've read, the accessibility features are good. As of the publish date of this blog entry, Windows Phone has no out of the box screen readers or assisted navigation, though it is something they are working on (part of the Windows Phone 8.1 release maybe)._

**Let's Paint a Picture**

Think of your favorite blog, the one that you just love to read while sitting on the can (admit it, you know you do it). So you're sitting in the dark. On the _toilette_ (saying it in French help?), about to do your thing. You don't need to turn on the lights in the bathroom. Cause you're blind. Not _blind-without-your-glasses_ blind, but **NLP (no light perception)** blind. You have your pants down to your ankles, your phone is in your hand. **Can you navigate to your favorite blog using the phone's browser, find the latest blog entry, and have your phone read it to you?** If you have an iOS device, the answer is a definite _yes_ (it's also a yes for Android phones).

**How The Blind Use Mobile Devices**

[This slide deck](http://www.slideshare.net/AdrianoMartino/ruby-motion-andiosaccessibility) by [Austin Seraphin (a blind software developer)](http://austinseraphin.com/about/) goes into details about how the blind use mobile devices.

Some highlights:

- Color reader apps. You walk up to your closet and need to find a shirt that matches with a pair of pants. You don't really care, but the rest of the seeing world does. So you hold up your phone and let it read the colors of all your clothes to you.

- Money reader apps. You have cash in your wallet. You pull out a bill. Are you holding a $1 bill or a $100 bill? Hold your phone up to the bill and it'll tell you.

- Image recognition apps. Tells you what object you are "looking" at based on image recognition.

##Some Help if You're Developing iOS Apps

I found [this library called SSAccessibility](https://github.com/splinesoft/SSAccessibility) extremely helpful. It provides a facade over iOS's accessibility apis and does a great job of managing/queueing VoiceOver notifications (something that you'd have to build yourself... since the core libraries simply interrupt what's currently being spoken, if another notification comes in).

There are already plenty of resources out there that will help you with the api, here are a few search terms that you can type into Google, leading to a wealth of material:

- UIAccessibility Protocol Reference
- UIAccessibilityIsVoiceOverRunning
- UIAccessibilityPostNotification
- accessibilityElementsHidden
- setAccessibilityLabel
- setAccessibilityHint
- screen curtain iPhone
- accessibilityPerformMagicTap

##A List of Undocumented Edge Cases That You Definitely Want to Look Out For

- There are plenty of people over at [AppleVis](http://applevis.com) that will beta test your app and give you feedback.

- Manipulating the alpha values of a control will break accessibility labels. The blind will not be able to touch a control and have it read out (but swiping to the control still works... weird, I know). Be sure to only hide/show controls if accessibility is enabled (do not change any alpha values).

- With VoiceOver enabled, users can triple tap on a button which will call the event handler for the button, twice, in lighting fast succession. This can lead to some unintended exceptions (since it's not something a seeing user can do). If you are showing modals, you could accidentally show two modals (which will cause an exception). If you are using a NavigationController, you could accidentally push two things onto the navigation stack, which will throw an exception if it's executed during an animation event (or if the controller instance you are pushing onto the navigation stack is a singleton). Showing views without animations helps, but it won't handle all cases. You'll need to comb through all controls and triple tap things.

- Screen transitions _usually_ cause the top most element on the screen to gain focus, but not always. This can be disorienting to the blind. You'll want to explicitly set the focus to the top most element. But, don't do it immediately when the screen shows up, if the element hasn't been painted on the screen entirely, the focus will _not_ be set. You'll need to add a minor timer delay (I did half a second) before setting focus (this will ensure that all things are definitely painted).

- UIAlertViews and UIActionSheets suffer from the same problem above. Most of the time they'll get focus, sometimes they won't. You'll need to employ the same minor timer delay before explicitly setting the focus to the views.

- If you choose _not_ to use SSAccessibility, you'll need to implement your own VoiceOver queueing mechanism to handle back to back update notifications. You can save yourself a lot of pain by just using the library. If you still insist on doing it yourself, good luck.

##Make Mobile a Better Place for the Blind, Because We've Broken the Web

I know many of us feel that having an app for something that can just be a website is silly. I myself get extremely annoyed every time I visit a web page and I get a nag screen telling me to download the iPhone app. **But, we've pretty much broken the web for the blind. Our websites aren't linear, top to bottom. We have "like" buttons, and sidebars, and modals with tiny pngs for close buttons (with no alt-text), and partial async page rendering all over the place.** All of which is nightmarish for a screen reader that is taking a two-dimensional medium, and shoving it into a one-dimensional voice over. Native iOS apps are extremely, extremely valuable to the blind... just something to be aware of next time you get a download-the-app nag screen.

When I first developed A Dark Room for the iOS, I was ignorant. I didn't think that mobile devices were such a life changer for the blind (and that there are blind gamers out there). I've went back and made a ton of accessibility changes to the game (available in v1.2), and am now writing this blog post. It is my meager attempt to raise a little bit of developer awareness. So, go forth, and make a difference. One of my friends said all this more succinctly when I was telling him about the updates I was making to A Dark Room:

>**Their happiness is more important to me than the happiness of 1,000 spoiled nerds with $2. It matters.**
