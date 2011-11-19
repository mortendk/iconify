#Icon Font CSS.
A couple of SASS file(s) that makes it super easy to include font based icons into the css, without remembering what they key to that icon is.
Got inspired by Chris Coyiers excellent (http://css-tricks.com/examples/IconFont)
so i whipped up a couple of css file for the Drupal CMS (http://drupal.org) but thought this might be usable for others.

Check out css tricks if you don't get the whole idea of icon fonts.



##Usage
The idea is to use SASS @extend to add the icons directly without having to remember what the key was to that particular library.

So if you wanna shift icon library, you change the @import to "whatever" style and keep using the same .icon-[iconname]

All the icons are predefine in the 	iconfont-[NAME].scss
fx the cloud icon is defined like this:

.icon-cloud { 
	content: "C"; 
	@extend .icon;
}


so to add an icon you use the :before / :after to add an icon in the ccss

```
h1:before {  
  @extend .icon-cloud;   
  font-size:1em;
  margin:-1em 1em 0em 0em;
  color:rgba(255,255,255,.9);
  text-shadow: 0px 0px 5px lightblue;
}
```



##create new font icon sets
use the fonticon-template.css


##Icon Fonts
**Websymbols**:
http://www.justbenicestudio.com/studio/websymbols _OFL license_

**Pictos**:
http://pictos.drewwilson.com _Commercial_

**Tipogram**:
http://tipogram.com _Commercial_

**Fico**:
http://fico.lensco.be _Commercial_


## What about xxx
right now I'm wanna get the different libraries mapped up, then I'm maybe gonna a LESS version
