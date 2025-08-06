---
layout: post
title:  "Python VS C++"
date:   2025-08-06 00:44:45 +0200
categories: python cpp programming 
---

The first two programming languages I learned are Python and C++. These are the languages that I have some experience with from particular coding projects in University. Since these languages are very different and both have there own advantages and drawbacks, it seemed interesting to compare them.

Let’s start by explaining the difference between high-level and low-level languages. We can put any programming language on a ‘spectrum’ from low- to high-level.

Python is an example of a high-level language. C++ is an example of a low-level language. Is is mainly the reason why the two languages are so different. 

In a low-level language, the programmer has more control over what the processor eventually will do. To perform a set of calculations, there often is more than one way for the processor to handle this. The most low-level language there is, is assembly code. In assembly, every statement (or line) corresponds with exactly one processor instuction. So if you really wanted hundred percent control over your program, you could try to code it in assembly, but trust me, you’ll need a lot of time (and it probably wouldn’t be fun to do). That actually reminds me of my first year of CompSci, where we first learned about assembly and then had to make our own Maze Game in MIPS assembly language. You can view this project of mine [here](https://github.com/joachimverleysen/MIPS-game).

So if we move a bit further on the spectrum of languages, we arrive at C++. C++ is a low-level language because it allows for a lot of processor control. This means that you can tell C++ more accurately not just what you want it to do, but also *how* you want it to execute it (not as accurately as assembly ofcourse). This also makes C++ a bit more complex to learn and understand.

On the other end of the spectrum, we have Python, a high-level language. In contrary to C++, Python is syntactically simple, which makes it easier to learn. Python is a high-level language because you can tell Python what you want it to do, but you can’t really control *how* it’s going to execute it. 

Having that said, there’s another fundamental difference in the process between code and execution. C++ is a compiled language. That means, you write something in C++, than you compile it, and that generates an executable file which you r processor can then run. 

Python on the other hand is an interpreted language. It works with an interpreter. What is that? Well, an interpreter is kind of a program on its own that is responsible for executing the code. So what is the difference with compiled languages? Interpreters execute the code directly from the source code and in the case of Python, the code is executed *line by line.* So in other words, Whereas C++ first analyzes the source code, compiles it and than executes it, Python analyzes and immediately executes the source code line by line. 

Let’s now go over a couple of syntactical differences to illustrate the power of the languages in their own way. As mentioned earlier, Python is simple, while C++ is more strict and allows for more control. Let’s just consider a simple variable assignment.

# Snippet 1
{% highlight python %}
num = 5   
{% endhighlight %}
#

# Snippet 2
{% highlight cpp %}
int num = 5;
{% endhighlight %}
#

What difference can we notice? First of all, we observe that in Python, we don’t have to specify the type when assigning a variable. This is called *dynamic typing.* In C++ on the other hand, we speak of *static typing.* So essentially what this means is that in C++, once you’ve declared a variable as int, it will stay an int forever. Its type is *static.* In Python, the type is ‘guessed’ by the interpreter based on the value that the variable holds. The type of a variable can change in Python, it just depends on what the variable contains.

# Snippet 3
{% highlight python %}
num = 5   # Integer
num = True   # Boolean
num = "Hello, world!"   # String
{% endhighlight %}
#

# Snippet 4
{% highlight cpp%}
// Declaration
int num = 5;   // num is defined as an integer.

// Reassignment
num = "Hey";   // ERROR: "Hey" is not an integer
{% endhighlight %}
#


