Title: Markdown Sample
OriginalAuthor: James Quigley

Level 1
=======

Level 2
-------

# Level 1
## Level 2
### Level 3
#### Level 4
##### Level 5
###### Level 6

This text is *emphasis*
This test is **bold**
This is `monospace`
Symbols: (R) (C) (V) (TM) -> <- => <= &#182; -- 

* Milk
* Bread
* Cheese
    * Cheddar
    * Camembert
* Rice

Another list

- Milk
- Bread
- Cheese
    - Cheddar
    - Camembert
- Rice

Numbered List

1. Stuff
1. Stuff
     1. More Stuff
     1. More Stuff
1. Stuff
1. Stuff

<!-- Comment Block -->

> This is a block quote
> This is a continuation
>> Multi indent block text

This is a code block:

    code 1
    code 2
    code 3

C Programming Code Block

~~~ c
#include <stdio.h>
int main(int argc, char **argv) {
printf("showing a fenced code block!\n");
    return(0);
}
~~~{.c}

Perl Code Block

~~~ perl
#!/bin/env perl

print "something\n"
~~~

First Line

* * * * * * * *   

Second Line

***

---

- - - - - - -     

Third Line

Math Expressions:

\\[ \frac{H_{U_1}}{H_{U_1}} \\] 

\\[ \frac{1}{2} \\] 

$$ {e}^{i\pi } 1=0 $$

$$ {x}_{1,2}=\frac{-b\pm \sqrt{{b}^{2}-4ac}}{2a} $$

<% Tex \frac{123}{456}} %>|fraction

## Notes
### Header for the table

Question                           | Answer
-----------------------------------|---------------------------------------------------------------------------------
What is the objective of security  | The objective of security is to protect a company an its assets.
                                   |
What is risk analysis?             | (V) *Risk Analysis* -- identifies the assets, discovers threats, and estimates
                                   | the
                                   | possible damage and potential loss.
                                   |
What caused the need for           | The core networking architecture changed from one of being a localized, stand
better security?                   | alone computing environment to a distributed computing environment.
                                   |
                                   | Data has also become an asset the needs to be protected, not just systems.
                                   |
What are some of managements core  | Some of managements core functions include determining objectives, scope
functions?                         | policies, priorities and strategies.  Management is responsible for determining
                                   | the actual goals expected to be accomplished from a security program.
                                   |
                                   | 
                                   | 1. Test
                                   | 2. Another test
                                   |
                                   | - Test
                                   | - Test
                                   |
                                   | **some bold text in table**
                                   |
                                   | \\[ {x}_{1,2}=\frac{-b\pm \sqrt{{b}^{2}-4ac}}{2a} \\]
                                   |
                                   | ![munch with an id][1]
                                   | 
								   
# Links

[[Home|sample-markdown]]

* [Google Website](http://www.google.com "other google text")
* [Text Text File](test.txt)
* [Markdown Cheatsheet](markdown-cheatsheet.pdf)

[Google Website Id][2]

![munch](munch_scream.jpg "The Scream") 
![munch with an id][1]

[1]: munch_scream.jpg "The Scream" class=munch width=40px height=40px
[2]: http://www.google.com "Google ID site"
