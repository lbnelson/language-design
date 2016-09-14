_Fill in each this file with your responses, placing each response after its
corresponding question._

---

**Question**

Pick three quotes from the readings about language design. Good candidates 
are:

   + Something you agreed with / resonates with your own experience
   + Something you disagree with
   + Something that is interesting, a new idea or perspective you'd like to remember
   + Something you didn't understand

For each quote, describe what it was about the quote that led you pick it.

**Response**

"It is one thing to have learned the syntax of a language and another to have 
grasped the underlying paradigm" [Yang and Radkin, 2015]

We agree with this quote from _C is Manly, Python is for "n00bs": How False
Stereotypes Turn Into Technical "Truths"_ for the most part, but in the case
of Python and C, it is more complicated. Python does not require the user to
have as sophisticated of an understanding of underlying paradigms because
the intent of Python is to be user-friendly. To use C, on the other hand,
it is necessary for the user to have at least a basic understanding of 
underlying principles. An example is passing by reference. In C, you must
explicitly pass a reference to a variable, whereas in Python you simply
pass a parameter. 


```
integer i = 0
repeat 10 times
i = i + 1
end 
```
That still looks mostly like Greek to me, but Stefik compares it to this equivalent 
statement in Java ("which is similar to Perl is some ways," he says):
```
for(int i = 0; i < 10; i++) {
} 
```
That’s not Greek, it’s Klingon [Pavlus, 2012] 

To us as programmers, the second example of Java code is far clearer. The 
more English-y syntax of the Quorum example may be clearer to someone
unfamiliar with programming. The Java code is a form of shorthand for the
Quorum, and if you use a phrase enough times shorthand becomes quicker
and easier to understand. 

"A cathedral is a huge church. It may be made of stone; it may fill you with
awe; but the key thought, in the mind of Eric Raymond, is that there is but
one design, one grand plan, which may take a long time—many years—to make real"
[Steele, 1998]

This was a very appropriate metaphor for beginning to learn programming. 
Most people would learn a general concept language first, like Java, and
the amount it can do could be overwhelming. A smaller language, like Scratch,
might provide a gentler introduction to programming in general. When you're
first learning and being taught conventions, it throws back to the original
grand plan for how the language should be used. As you learn a language 
more, you can see that it's still growing and that it's not necessarily
a cathedral. 

---

**Question**

How would you know a well-designed language? What are the symptoms? How would
you know a poorly designed language? What are the symptoms?

**Response**

The most important feature of a well designed language in our opinion is
understandability. Steele mentions that including too many features for
specialized groups of users would "just be too much" [Steele, 2012]. This
is in line with understandability because users don't need to learn as 
many features. This is also in line with knowing the intended audience for
a language and catering to their needs - Java is a general purpose language
and therefore should not be too specialized for any one field. 

The syntax for a well designed language should be intuitive. It has to mesh
well with the native language of users because language dictates how users
think. According to Andreas Stefik, "usability testing showed that simply 
finding natural-language replacements for some of the more abstruse syntax 
went a long way" [Pavlus, 2012]. One example is Racket's syntax for addition,
for example, is not intuitive to English speakers because the operator is
first followed by the two numbers to be added. 

Another sign of a good language is having naming schemes and syntax that
lines up with expected behavior. Bloch mentions that a good API should 
"Obey the principle of least astonishment. Every method should
do the least surprising thing it could, given its name. If a method
doesn’t do what users think it will, bugs will result." [Bloch 2006]. 
The same logically extends to a programming language. In a talk called Wat 
by Gary Bernhardt at CodeMash 2012, he provides examples of astonishing 
behavior. In JavaScript, ` [] + [] ` produces the empty string 
[Bernhardt, 2012]. This, both according to the talk, and according to us makes
absolutely no sense. 

---

**Question**

How do the themes of _Growing a Language_ relate to the "sound lab" we did this week?

**Response**

In the sound lab, we were growing the sound library from the completed CS5 lab. We
were improving the usability and fluency of that library. One thing we could have
done to improve the sound library would be to overload the addition operator
such that two sounds could be added to each other. In Growing a Language,
Steele mentions "right now operators in the Java programming language can not
be overloaded by the programmer, though names of methods may be overloaded. I 
would like to change that." [Steele 1998]. That's an improvement to Java
that would allow a similar improvement in a sound library. This runs along
the same theme as a language's capability for growth. 

The sound library we were using has the characteristics of a "small" language.
It has basic capabilities of functions but everything writes to out.wav and you
must retype the source file name every time you want to modify it. This
provides many opportunities for the same kind of growth by wart removal 
described in Steele: "Users will not put of with the warts for all time". 
[Steele, 2012] We designed a way for users to no longer deal with warts. 

Additionally, when we were modifying the sound library, we were keeping
in mind the potential for future additions. In Steele, it is mentioned
that when making a language, "I should not design a small language, and
I should not design a large one. I need to design a language that can grow.
I need to plan ways in which it might grow—but I need, too, to leave some 
choices so that other persons can make those choices at a later time."
[Steele, 2012]. The ideas we had for improving the library also made
it more easily extensible by providing a class structure. 

---
 
**Question**


In what way is an API a language? 

**Response**

Outline:
- Refer to Bloch
	- Similar principles for a good language as for a good api
	- "Code will read like prose" backs up the way an api is 
	in a sense a language
	- inner workings of a language are obscured in the same way
	  inner workings of a good api should be
	- Connect things Bloch mentions to ideas for intuitiveness
	  in Pavlos
	- API as an extension of a language (bring in Steele)
- Ways in which an API is not like a language - public API versus
  growing language
- APIs should be self documenting but this completely translated to
  all languages because even Python takes some hand holding (pavlos)
- An API is kind of like a small language as described by Steele
---

**Question**

What does the post on grayscale tell us about the process of API design?

**Response**

- Target audience is important
- Doing the intuitive thing is important but it's hard to determine
  what is the most intuitive (bring in Pavlos)
- Growing an API like a language is a consideration (bring in Steele)
- Naming things is key and different people have different opinions
  on what a name should be 
- Principles in bloch are not as easy to follow as they sound
- Reference Bloch a lot in relation to the reality of designing
 an API according to the grayscale post

---

**Question**

The Yang and Rabkin article talks mainly about general-purpose languages. In 
what ways do the themes apply to the study and creation of DSLs?

**Response**

As the title of the article, “C is Manly and Python is For n00bs”
[Yang and Rabkin 2015] suggests, higher-level and less complex languages may
be looked down upon culturally. This bias most likely applies to many DSLs
as well because DSLs often have more limited, specialized syntax. However, 
that limitation of  a DSL may not be the only reason it would be looked down 
upon based on Yang and Rabkin. One of the points made in Yang and Rabkin is 
that “programmers confuse their strong views about languages with their views 
about users of the languages” [Yang and Rabkin 2015]. This suggests another 
reason why DSLs might be looked down upon by the larger programming community. 
Because DSLs have a specific domain, they might have users who are not 
stereotypical programmers and therefore looked down upon. There is even an 
example of DSL that is looked down on for this exact reason in Yang and Rabkin, 
“Software engineers sometimes deride statistical analysis languages like R or 
SAS as ‘not real programming’ ” [Yang and Rabkin 2015]. Like other DSLs, R is 
not typically used by software engineers and that likely contributes to the 
bias against it. As described in the article, “Languages often spread in 
disjoint real-world communities, making it easy for false perceptions to 
arise about a language’s user base” [Yang and Rabkin 2015]. This probably 
applies to DSLs even more so than for other languages since DSLs are often 
targeted at a specific group of users. 

Another aspect of DSLs that this article may touch on is their creation. 
Creating a DSL might be regarded as “manly” since it is challenging and 
might be done in a language like C, which is “Manly” [Yang and Rabkin 2015].
A DSL also implies that someone took the trouble to make things (probably) 
easier for the user of the language, which is in line with the language
being looked down upon in the same way Python might be. 

---

**Question**

The Pavlus article mentions the researchers' comments that people preferred
"natural-language replacements for some of the more abstruse syntax". In other 
words, people found it easier to work with code that looks more like a human language (e.g.,
English). Consider the following quote by William R. Cook, one of the creators
of AppleScript:


> The experiment in designing a language that resembled natural languages (English
> and Japanese) was not successful. It was assumed that scripts should be
> presented in “natural language” so that average people could read and write
> them. … In the end the syntactic variations and flexibility did more to confuse
> programmers than to help them out. It is not clear whether it is easier for
> novice users to work with a scripting language that resembles natural language,
> with all its special cases and idiosyncrasies. The main problem is that
> AppleScript only appears to be a natural language: in fact, it is an artificial
> language, like any other programming language. … even small changes to the
> script may introduce subtle syntactic errors that baffle users. It is easy to
> read AppleScript, but quite hard to write it.
[[Cook 2007, page 1-20]](https://dl.acm.org/citation.cfm?doid=1238844.1238845)

Are these two experiences of natural languages at odds with one another? Would
you choose to include natural language in the design of a DSL? If so, how might
you do so? If not, why not?

**Response**

It may be possible to have a language be in the same "grain" as a natural 
language without actually having the associated ambiguity. If it has a 
well defined structure and syntax, then the flexibility described in the
excerpt above may not be an issue.

In Pavlus, it is described that "finding natural-lanaguge replacements for 
some of the more abstruse syntax went a long way" [Pavlus 2012]. At first
glance, this seems to be a direct contradiction to the expriment described
in the above quote from Cook. However, in the case of Pavlus, novices were
the ones being expiremented on. For us, the more natural language-like 
syntax in Pavlus was less easy to understand than the Java syntax. In Cook, 
programmers were the ones using the natural language rather than novices.
It would be interesting to perform an expiriment about whether novices
or experienced programmers have more or less trouble with a specific 
natural language-like programming language. 

Additionally, in Pavlus, there was more focus on the readability of the
language rather than the writing - according to Pavlus, 
"
```
integer i = 0
repeat 10 times
i = i + 1
end 
```
That still looks mostly like Greek to me, but Stefik compares it to this equivalent statement in Java ("which is similar to Perl is some ways," he says):

```
for(int i = 0; i < 10; i++) {
}
```
That's not Greek, it's Kligon.
" [Pavlus 2012]. In both Pavlus and Cook, the code that resembled natural language
was easier to read than the more standard programming language. This raises a 
question about whether it is possible to strike a balance between that readability
and the stricter structure apparently necessary. 

---

**Question**

Briefly describe how you split up the work for this assignment.

**Response**
We both did the readings while in the same location. 
For the first several questions, we constructed answers together and for the
remaining questions we first wrote outlines and then divided them up
evenly to complete. 


---
