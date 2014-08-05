---
layout: post
title: When not to use a tool
date: 2012-09-02 15:02:00
categories: career hacking "software engineering"
---

Mastering a tool means much more than just knowing how to use it. When you know something really well, you should also know the problems and limitations it has. In other words, you know exactly why and why **not** use it in certain circumstances.

To exemplify the idea I will illustrate with a coding question:

_"You have a string containing parentheses. Write a function to validate if the parentheses are properly nested"_

The answer that comes from 9 out of 10 programmers is, without even thinking: "**_REGEX_**!"

And if asked to elaborate the answer they get stuck and keep struggling with this alternative that is not appropriate for this case - _it requires some recursive pattern trick that is not implemented in every regex engine and is expensive in terms of memory usage. Also it's against the idea of **finite automata** that is the basic theory behind regexs_ - while there's a **dead simple** algorithm that can do that with the best performance possible O(n) in one single traversal through the string and with constant memory space:

{% highlight go %}
//O(n) and constant space
func nesting(s string) bool {
    x := 0
    for i := 0; i < len(s); i++ {
        if s[i] == '(' {
            x++ // Increments when '(' is found
        } else if s[i] == ')' {
            x-- // Decrements when ')' is found
            if x < 0 {return false}
        }   
    }   
    return x == 0
}
{% endhighlight %}

Bringing this idea to daily situations, how many times developers are choosing their preferred tool/language/framework to use in a project without really thinking about the problem they need to solve and the limitations the tool has, just to don't leave their comfort zone?

Things like: using PHP-GTK to build desktop apps; Rails to highly trafficked websites with a lot of user-generated content where you can't really cache that much the generated pages; using NoSQL databases to store data that is naturally relational (and vice-versa), etc… that when used in this kind of improper way usually imply in a high cost of maintenance, and in many cases require rewriting whole systems from scratch when problems start to pop everywhere.

But everybody has preferences, so how to avoid those biased decisions? In my opinion it can be avoided by not letting the decision be influenced by hype and not restricting the possible solutions by just the one or two that decision makers already feel comfortable with. Take some time to analyse the nature of the problem and the many different ways to attack it.

Assuming that good developers don't [take things for granted](/2012/06/taking-things-for-granted.html) they might be able to understand how things work internally, (if they're mature enough, they will also accept that their favourite option might not be the best one) and adapt themselves to a tool that might come as a better solution.

## Related links
* [http://engineering.twitter.com/2011/04/twitter-search-is-now-3x-faster_1656.html](http://engineering.twitter.com/2011/04/twitter-search-is-now-3x-faster_1656.html)
* [http://blog.feliperibeiro.com/2012/06/taking-things-for-granted.html](/2012/06/taking-things-for-granted.html)