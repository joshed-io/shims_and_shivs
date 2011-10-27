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
* JavaScript shims that fill feature gaps amongst browsers
* "Poly" because they can be pretty diverse (i.e. canvas)

!SLIDE center bullets incremental
# Does it matter?
* Yes! Polyfills have sped up HTML5 adoption.
* B/c they let developers do the new stuff...
* without breaking old platforms.

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
* ## - in the name of peace -
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
## Audio and Video
## Web Sockets
## CSS3
## Cross Domain Messaging

!SLIDE center bullets
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
# Making a shim?
* Don't reinvent
* Strive for API Compatibility
* Be supertiny
* Read [Addy's Guide](http://addyosmani.com)

!SLIDE center bullets incremental
# Fashimable Ex. #1
### Object.keys

      @@@ javascript
      Object.prototype.keys = function() {

      }

!SLIDE center bullets incremental

!SLIDE center bullets
# Further Reading
* [What is a polyfill?](http://remysharp.com/2010/10/08/what-is-a-polyfill/)
* [HTML5 Cross-Browser Polyfills](https://github.com/Modernizr/Modernizr/wiki/HTML5-Cross-Browser-Polyfills)
* [Quirksmode Compatibility](http://www.quirksmode.org/compatibility.html)
* [Mozilla Developer Network](https://developer.mozilla.org/en-US/)
* [History of the HTML5 Shiv](http://paulirish.com/2011/the-history-of-the-html5-shiv/)