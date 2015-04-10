---
layout: post
---

App Content & behavior.

---

# Index

- [General](#1)
- [Preloading Content](#2)
- [Pull-to-refresh](#3)
- [Tab bar](#4)
- [Feed view](#5)
- [Top navigation bar](#6)
- [Article navigation bar](#7)
- [Search](#8)
- [Now Playing](#9)
- [Picture View](#10)
- [Quizzes](#11)

---

<div id="1"></div>
## General
- Fonts: lots of stuff still Helvetica (most should be Source Sans Pro)

<div id="2"></div>
### Preloading content
- Currently, we are loading table views (reading list, feeds, search, etc) with empty images on them. That should never happen. Bad UX.
- Would prefer to have the entire page pre-loading and show the animation me and James created
- On feeds, we should load 10 (or X) posts at a time and have them all loaded when you scroll down

![Loading](/images/loading-more.png)

<div id="3"></div>
### Pull-to-refresh
- Currently missing
- Upon full pull, loop ? animation
- Should be available everywhere

![PTR](/images/ptr.gif =320x)

<div id="4"></div>
## Tab bar
- Replace current highlight (darker background) with **color** highlight
- Ensure font is Source Sans Pro
- Move "Topics" icon to the middle (most prominent spot) and "Quizzes" to leftmost

![Tab](/images/selected-tab.png)

<div id="5"></div>
## Feed view
- Need slightly more spacing between articles

![Feed](/images/feed-spacing.jpg)

- Add zoom animation when user taps (similar to Feedly)
- Perhaps the same kind of "pull down to dismiss" action?

![Feedly](/images/feedly.gif)

<div id="6"></div>
## Top navigation bar
- Add a 1px line to the bottom of it #D0D0D0
- On **Channels**, arrow icon should start pointing down. When I tap it, it should **flip** upwards. When I exit dropdown, it should **flip** back to the bottom.

<div id="7"></div>
## Article navigation bar
- Entire bar should popup a second after page has loaded
- Should **not** appear before its text is loaded
- Add a 1px line to the top of it #D0D0D0
- Height feels a bit too tight with the tab bar; bring back to old height (67pt)

<div id="8"></div>
## Search
- Missing the big X on the right
- X should clear the search and then close it (if empty)
- Exiting search is currently messed up

![Search](/images/search-bar.png =320x)

<div id="9"></div>
## Now Playing
- **Now Playing** icon should be animated

### On iPhone
- Should be full-screen
- Window should slide up from bottom and have an X control
- User can dismiss by dragging navbar down

![Now playing](/images/now-playing.png =320x)

### On iPad
- Same contents of iPhone control, inside a *popover* control

<div id="10"></div>
## Picture View
- Add same behavior from Twitter and Facebook when previewing image – I can drag it up or down and dismiss it rather than having to tap on a X or just tap on the image.
- See Feedly image above

<div id="11"></div>
## Quizzes
- Home looks super weird (not enough content?); check feeds.
- When home loads, the "Start Quiz"
- Updated the position/look of the score area
- After picking an answer, user should go to the next question when:
	a. tapping next
	b. swiping left
- After picking an answer, here's the order of events:
	- Selected answer turns green or red; other answers fade away
	- "Next question" overlay comes in from the right side

See this [Pixate demo](http://pixt.io/p77d81791ad04) for more details.

![Quiz 2](/images/quiz-2.png =320x)

