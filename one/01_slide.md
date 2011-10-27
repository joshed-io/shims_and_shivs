!SLIDE center
## Polyfills:
# SHIMS AND SHIVS
By Josh Dzielak
<div class="spacer"></div>
<div class="spacer"></div>
![DisneyHTML5Summit](wordmark.png)
<div class="shivs">halloween 2011</div>

!SLIDE bullets incremental
# About Me:
* Founding Developer at ![DisneyHTML5Summit](tv_logo.png?123)
* We're a Safe Social Network for Kids
* We joined Disney in 2011
* Shivs of choice: JavaScript & Ruby

!SLIDE bullets incremental
.notes not about geometry, not a rock band, not a winter coat lining

Let's talk about
# POLYFILLS
"A shim that mimics a future API providing fallback functionality to older browsers." - Remy Sharp


Polyfills help you use new technologies without breaking in old browsers

!SLIDE center bullets incremental
# Does it matter?
* Yes! Polyfills speed HTML5 adoption.
* B/c they let developers do the new stuff...
* with less duplication...
* to support the old stuff

!SLIDE center bullets incremental
# The Spooky Example
* ## Using HTML5 tags in an 'older' browser...
      @@@ html
      <footer>...</footer>

!SLIDE center
.notes 'use horrible'

...like

# Internet

# "Expect Horror"

# 8

!SLIDE center
### HTML5 Tag support:
![footer_without_shim](footer_without_shim.jpg)
### With [html5shim.js](http://code.google.com/p/html5shim/)
![footer_without_shim](footer_with_shim.jpg)

!SLIDE center
## Don't worry. There's more.
But first,
# Let's settle
# an old score...

!SLIDE bullets incremental
.smalls Is it
# "Shims" OR "Shivs" ?
* ## Yes!

!SLIDE bullets incremental
## Shims are tools.
* ## Shivs are weapons.
* ## And \(tools + weapons\) =

!SLIDE center
# MACGYVER
![macgyver](macgyver.jpg)

!SLIDE center bullets incremental
## If
* ## MACGYVER

!SLIDE center
![macgyver](macgyver.jpg)

!SLIDE center bullets incremental
# MACGYVER
* ## OK

!SLIDE center bullets incremental
## can use shims as shivs
* ## (in the name of peace)
* # THAN SO CAN YOU!
!SLIDE center

!SLIDE center bullets incremental
# ShimWOW!
* Got a project? Ask:
* Who am I supporting?
* What modern feature do I need?

!SLIDE center incremental
Maybe we want geolocation

for desktop and mobile browsers.

## What now?
Sure,
# LMGTFY

!SLIDE commandline incremental

	$ google 'new guy needs polyfill'
	processing........
	processing........
	$ hurry up
	i'm going as fast as i ca

!SLIDE center
### Results Found!
![support](support_table-1.jpg)
### http://caniuse.com/
## Verdict:
Need polyfill for earlier Safari, IE, and Opera.

!SLIDE center bullets incremental
detect features, not browsers
# Modernizr
* Know when to shim.
* Bundled /w Yepnope, a conditional script loader.
* It's EASY enough to show you an example using BIG fonts.

!SLIDE incremental
      @@@ javascript
      Modernizr.load({
        test: Modernizr.geolocation,
        yep : 'geo.js',
        nope: 'geo-polyfill.js'
      });
# Proved it!

!SLIDE center bullets incremental
# Things Commonly Polyfilled
## Let's explore a few.

!SLIDE center bullets incremental
## Audio
* [jPlayer](http://github.com/happyworm/jPlayer) -  jQuery, Flash Fallback
* [audio.js](http://kolber.github.com/audiojs) - Drop-In, Flash Fallback
* ## Video
* [video for everybody](http://web.archive.org/web/20101205155004/http://camendesign.com/code/video_for_everybody) - Markup, no JS. Nice!

!SLIDE center bullets incremental
## CSS3
* [css3-mediaqueries-js](http://code.google.com/p/css3-mediaqueries-js/)- Media Queries Everywhere
* [cssFx](http://imsky.github.com/cssFx/) - Inserts Vendor-Specific Properties
* [Scoped CSS](https://github.com/thingsinjars/jQuery-Scoped-CSS-plugin) - Limit Styles!

!SLIDE center bullets incremental
## Web Sockets
* [sockjs](https://github.com/sockjs/sockjs-client) - Full solution for WebSocket emulation
* [socket io](http://socket.io/) - Client+Server
* [pusherapp](http://pusherapp.com/) - WaaS

!SLIDE center bullets
Now, some general
## DO's
and
# DON'TS

!SLIDE center bullets
Don't be
# AFRAID
to try new technologies...

!SLIDE center bullets incremental
##...just because you have to support users on old platforms.
# YOUR'E NOT ALONE

!SLIDE center bullets incremental
a few

# philosophies

## can help you

structure the problem.

!SLIDE center bullets incremental
you might know about
# Progressive

# Enhancement

"Progressive enhancement is a strategy for web design that emphasizes accessibility, semantic HTML markup, and external stylesheet and scripting technologies."
\- [From  wikipedia](http://en.wikipedia.org/wiki/Progressive_enhancement)

!SLIDE center bullets incremental
and there's also
# Regressive

#Enhancement

"The “polyfill” or “regressive enhancement” technique just means that you go ahead and use the new features, then use JavaScript to emulate native behavior in older browsers."
\- [From Alex Sexton](http://www.sitepoint.com/regressive-enhancement-with-modernizr-and-yepnope/)

!SLIDE center bullets incremental
# Recap
* ## So that's

!SLIDE center bullets incremental
* ## Progressive Enhancement
  * design and build something that works everywhere (to the baseline)
  * extend to new capabilities where you can
* ## Regressive Enhancement
  * design and build with the latest and greatest
  * backfill where it breaks

!SLIDE center bullets incremental
# Reality Check

## Both philosophies are useful.

There are myriad considerations.

## What's important to you?

Use your <em>Best Judgment</em>®.

## You'll be fine!

!SLIDE center bullets incremental
## So, we're using shims now?
# Great
## What if we need to make a shim?

!SLIDE center bullets incremental
# A few guidelines
* Don't shimitate. Does it exist already?
* Strive for API Compatibility
* Be supertiny
* Read [Addy's Guide](http://addyosmani.com)

!SLIDE center bullets incremental
# Thanks!
* I hope you have a better idea of
* ## what polyfills are
and more importantly
* ## how to think about them

!SLIDE center bullets
# Further Reading
* [What is a polyfill?](http://remysharp.com/2010/10/08/what-is-a-polyfill/)
* [HTML5 Cross-Browser Polyfills](https://github.com/Modernizr/Modernizr/wiki/HTML5-Cross-Browser-Polyfills)
* [Quirksmode Compatibility](http://www.quirksmode.org/compatibility.html)
* [Mozilla Developer Network](https://developer.mozilla.org/en-US/)
* [History of the HTML5 Shiv](http://paulirish.com/2011/the-history-of-the-html5-shiv/)

!SLIDE center bullets
# HAPPY HALLOWEEN!


# QUESTIONS?
