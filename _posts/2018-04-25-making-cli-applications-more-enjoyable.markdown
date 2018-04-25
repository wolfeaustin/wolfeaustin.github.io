---
layout: post
title:  "Making CLI Applications more enjoyable"
date:   2018-04-25 13:07:31 -0400
categories: jekyll update
---

While working with the CLI for the Module 1 project, we tried to think of ways to make the Command Line experience more enjoyable.  One of the ways we achieved this was by adding various ACII art.  

![Welcome ASCII]({{ "/assets/ASCIIdef.png" | absolute_url }})

Instead of greeting the user with 'Welcome to Our CLI Project'.  We could attain a more 3d vibe with ASCII characters.

![Welcome ASCII]({{ "/assets/ASCII Welcome.png" | absolute_url }})

Something like this is easily created using an ASCII generator like the one found here: http://patorjk.com/software/taag/#p=display&f=Graffiti&t=Type%20Something%20

Or if you want to generate an ascii version of your favorite photo, you could use something like this.
http://picascii.com/

Before and after we take an image and convert it to usable ASCII characters.

![Welcome ASCII]({{ "/assets/kang.png" | absolute_url }})
![Welcome ASCII]({{ "/assets/ASCIId.png" | absolute_url }})

If we want to add a bit more to the user experience, then we can animate these ASCII objects. These are generally created using a similar process to that of Claymation.  Each time the object appears to move, it's actually an entirely new picture that has been output to the terminal preceded by something clearing the old image (lots of "\n"'s).

One of the most impressive examples of this is a summary of 'Star Wars Episode IV: A New Hope', made entirely with ASCII animations.  

To play this little easter egg, copy and paste this in a new terminal window.

{% highlight ruby %}
  telnet towel.blinkenlights.nl
{% endhighlight %}


There are a ton of other resources out there and here are some of the best ones to get you started:





[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
