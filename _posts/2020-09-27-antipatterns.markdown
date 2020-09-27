---
layout: post
title:      "AntiPatterns"
date:       2020-09-27 23:53:50 +0000
permalink:  antipatterns
---

AntiPatterns are the opposite of design patterns. They are programming patterns that are deffective and may make code more complicated. They may appear to be good, but they are actually worse than they look.

"An AntiPattern is a literary form that describes a commonly occurring solution to a problem that generates decidedly negative consequences." (https://sourcemaking.com/antipatterns)

One example of a software arechetecture antipattern is the jumble pattern. "When horizontal and vertical design elements are intermixed, an unstable architecture results." (https://sourcemaking.com/antipatterns/jumble) This is antipattern will cause a lot of overly mixed parts of the code that will make things overly complicated.

Another example of an antipattern is the blob patern. In the blob pattern, "one class monopolizes the processing, and other classes primarily encapsulate data." (https://sourcemaking.com/antipatterns/the-blob) In other words, there is only one class that does almost all of the processing, and other classes are only holding the data that is used by the main class. However, there is a known exception that this is okay when wrapping legacy systems.
