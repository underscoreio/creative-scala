# Foreword {-}

Creative Scala is aimed at developers who have no prior experience in Scala.
It is designed to give you a fun introduction to functional programming.
We assume you have some very basic familiarity with another programming language but little or no experience with Scala or other functional languages.

We have three goals with this book:

1. To give an introduction to functional programming so that you can calculate and reason about programs, and pick up and understand other introductory books on functional programming.

2. To teach you enough Scala that you can explore your own interests in and using Scala.

3. To present all this in a fun, gentle, and interesting way via two-dimensional computer graphics.

Our motivation comes from our own experience learning programming, studying functional programming, and teaching Scala to commercial developers.

Firstly, we believe that functional programming is the future.
Since we're assuming you have little programming experience we won't go into the details of the differences between functional programming and object-oriented programming that you may have already experienced.
Suffice to say there are different ways to think about and write computer programs, and we've chosen the functional programming approach.

The reasons for choosing functional programming are more interesting.
It's common to teach programming by what we call the "bag of syntax" approach.
In this approach a programming language is taught a collection of syntactical features (variables, for loops, while loops, methods) and students are left to figure out on their own when to use each feature.
We've seen this method fail both when we were undergraduates learning programming, and as postgraduates teaching programming, as students simply have no systematic way to break down a problem and turn it into code.
The result is that many students dropped out due to the poor quality of teaching.
The students that remained tended to, like us, already have extensive programming experience.

Let's think back to primary school maths, specifically column addition.
This is the basic way we're taught to add up numbers when they're too big to do in our head.
So, for example, adding up 266 + 385, we would line up the columns, carry the tens and so on.
Now maybe maths wasn't your favorite subject but there are some important lessons here.
The first is that we're given a systematic way to arrive at the solution.
We can *calculate* the solution once we realise this is a problem that requires column addition.
The second point is that we don't even have to understand why column addition works (though it helps) to use it.
So long as we follow the steps we'll get the correct answer.

The remarkable thing about functional programming is that it works like column addition.
We have recipes that are guaranteed to give us the correct answer if we follow them correctly.
We call this *calculating* a program.
This is not to say that programming is without creativity, but the challenge is to understand the structure of the problem and once we've done that the recipe we should use follows immediately.
The code itself is not the interesting part.

We're teaching functional programming using Scala, but not Scala itself.
Scala is a language that is in demand right now.
Scala programmers can relatively easily get jobs in a variety of industries, and this is an important motivation for learning Scala.
One of the reasons for Scala's popularity is that is straddles object-oriented programming, the old way of programming, and functional programming.
There is a lot of code written in an object-oriented style, and a lot of programmers who are used to that style.
Scala gives a gentle way from object-oriented programming to functional programming.
However this means Scala is a large language, and the interaction between the object-oriented and functional parts can be confusing.
We believe that functional programming is much more effective than object-oriented programming, and for new programmers there is no need to add the confusion of learning object-oriented techniques at the same time.
That can come later.
Therefore this book is exclusively using the functional programming parts of Scala.

Finally, we've chosen what we hope is a fun method to explore functional programming and Scala: computer graphics.
There are many introductions to Scala, but the majority use examples that either relate to business or mathematics.
For example, one of the first exercises in the very popular Coursera course is to implement sets via indicator functions.
We feel if you're the type of person who likes directly working with these sort of concepts you already have plenty of content available.
We want to target a different group: people who perhaps thought that maths was not for them but nonetheless have an interest or appreciation in the visual arts.
We won't lie: there is maths in this book, but we hope we manage to motivate and indeed visualise the concepts in a way that makes them less intimidating.

Although this book will give you the basic mental model
required to become competent with Scala,
you won't finish knowing *everything* you need to be self-sufficient.
For further advancement we recommend considering one of the many excellent
Scala textbooks out there, including our own [Essential Scala][essential-scala].

If you are working through the exercises on your own,
we highly recommend joining our [Gitter chat room][underscore-gitter]
to provide get help with the exercises and provide feedback on the book.

The text of [Creative Scala][github-creative-scala] is open source,
as is the source code for the [Doodle][github-doodle]
drawing library used in the exercises.
You can grab the code from our [GitHub account][underscore-github].
Contact us on Gitter or by email if you would like to contribute.

Thanks for downloading and happy creative programming!

---Dave and Noel

## Notes on the Early Access Edition {-}

<div class="callout callout-danger">
This is an *early access* release of Creative Scala.
There may be typos and other errors in the text and examples.

If you spot any mistakes or would like to provide feedback,
please let us know via our [Gitter chat room][underscore-gitter]
or by email:

 - Dave Gurnell ([dave@underscore.io](mailto:dave@underscore.io))
 - Noel Welsh ([noel@underscore.io](mailto:noel@underscore.io))
</div>

## Acknowledgements {-}

Creative Scala was written by [Dave Gurnell][twitter-dave] and [Noel Welsh][twitter-noel]. Many thanks to [Richard Dallaway][twitter-richard], [Jonathan Ferguson][twitter-jono], and the team at [Underscore][underscore] for their invaluable contributions and extensive proof reading.

Thanks also to the many people who pointed out errors or made suggestions to improve the book: Neil Moore; Kelley Robinson, Julie Pitt, and the other ScalaBridge organizers; d43; Matt Kohl; Alexa Kovachevich and all the other students who worked through Creative Scala at ScalaBridge, at another event, or on their own; and the many awesome members of the Scala community who gave us comments and suggestions in person. Finally, we have large amount of gratitude for Bridgewater, and particularly Lauren Cipicchio, who perhaps unknowingly funded a good portion of the initial development of the second version of the Creative Scala, and provided the first few rounds of students.

Finally, Creative Scala owes a large intellectual debt to the work of many researchers working in programming language theory and Computer Science education. In particular we'd like to highlight:

- the work of the [PLT research group](http://racket-lang.org/plt.html), and in particular the book ["How to Design Programs"](http://htdp.org/), by Matthew Flatt, Matthias Felleisen, Robert Bruce Findler, and Shriram Krishnamurthi; and
- the "creative coding" approach to introductory programming pioneered by [Mark Guzdial](https://www.cc.gatech.edu/faculty/mark.guzdial/), [Dianna Xu](https://cs.brynmawr.edu/~dxu/), and others.
