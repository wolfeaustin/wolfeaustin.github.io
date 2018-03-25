---
layout: post
title:  "Sorting with Ruby"
date:   2018-03-25 13:01:31 -0400
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

When using one of the many enumerable methods that Ruby has to offer, it's easy to take them for granted. With not much thought, we can determine characteristics of an integer or perform some fairly complicated functions on arrays of material.

What goes on behind the scenes?

Some of these methods wouldn't be too difficult to duplicate.  Like the Array.uniq method for instance. 'Given an array, return a new array with only uniq instances'.

{% highlight ruby %}
a = [1,2,3,2,3]
def uniq(array)
  temp = []
  array.each do |item|
    if !temp.include?(item)
      temp << item
    end
  end
  temp
end
#=> [1,2,3]
{% endhighlight %}

Easy enough.  Create a new array.  If the new array doesn't have this current object, then add it.

What about more complex functions?

Enter the .sort method. 

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
