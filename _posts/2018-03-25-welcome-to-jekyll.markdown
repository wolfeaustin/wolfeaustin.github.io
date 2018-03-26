---
layout: post
title:  "Sorting with Ruby"
date:   2018-03-25 13:01:31 -0400
categories: jekyll update
---


When using one of the many enumerable methods that Ruby has to offer, it's easy to take them for granted. With not much thought, we can determine characteristics of an integer or perform some fairly complicated functions on arrays of material.

What goes on behind the scenes?

Some of these methods wouldn't be too difficult to duplicate.  Like the Array.uniq method for instance. 'Given an array, return a new array with only unique instances'.

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

However, it seems like we're cheating if we can use another enumerable method that we haven't yet defined. So let's define include?.

Array.include? 'If the item we pass in is included in the array, then return true, otherwise return false'

{% highlight ruby %}
a = [1,2,3,2,3]
def include?(array, itemToCheck)
  t_or_f = false
  array.each do |n|
    if n == itemToCheck
      t_or_f = true
    end
  end
  t_or_f
end
a.include?(0)
#=> false
{% endhighlight %}

How about some of the boolean evaluation methods?

Array.min 'Return the smallest value'

{% highlight ruby %}
a = [2,3,2,3,1]

def min(array)
  array.sort[0]
end
a.sort
#=> 1
{% endhighlight %}

What about more complex functions?

We may know that sorting in general is one of the most discussed topics in Computer Science. The fact that we take this method for granted when there is so much going on 'under the hood' is absurd.

Ruby had quite a lot of options when it came to selecting a particular sorting algorithm to use to for this task. After some research, I've learned that Ruby has implemented an optimized version of the popular QuickSort algorithm.  QuickSort uses a 'divide-and-conquer' method to handle the sorting.  Which means it recursively splits the list up into increasingly smaller pieces, sorts those, and then puts the pieces back together.

Here is a link with a more in depth explanation with visuals: http://interactivepython.org/runestone/static/pythonds/SortSearch/TheQuickSort.html



[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
