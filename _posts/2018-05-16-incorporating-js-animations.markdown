---
layout: post
title:  "Incorporating Javascript Animations"
date:   2018-04-25 13:07:31 -0400
categories: jekyll update
---

Javascript animations are a great way to spice up your projects.  These animations can be used to accomplish tasks such as rotating an object or creating a piece of art that becomes the center of your site.  This is an
extensive topic but libraries listed below would be a great place to start.

Starting off with simple animations, wickedCSS allows you to wrap elements in <div> tags to rotate an image
or to give some text a pulsating effect.


http://kristofferandreasen.github.io/wickedCSS/
![Wicked Instructions]({{ "/assets/WickedInstructions.png" | absolute_url }})


After the stylesheet is added, all you have to do is add the appropriate class tag.  If you wanted to
create an image that would be shown while something is loading you would write something like this.


{% highlight Javascript %}

<img src="images/mushroom.png" class="spinner"/>

{% endhighlight %}


Mojs.io is another library for Javascript animations that offers step-by-step tutorials.  Click on 'tutorials'
and from there you should see a large variety of really impressive shapes and animations created with this tool and implemented with Javascript


![Wicked Instructions]({{ "/assets/mojs.png" | absolute_url }})


http://mojs.io





If you have anymore questions about what is available, I found this blog post extremely helpful.
https://www.webdesignerdepot.com/2018/01/10-best-free-animation-libraries-for-the-web/






[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
