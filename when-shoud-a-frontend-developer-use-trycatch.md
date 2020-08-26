When you were taking computer science courses,
or reading classic JavaScript Primer book,
you would often meet one topic -- throw an exception and catch them.

But when you joined a company and started to write some real code,
you would often find try/catch disappeared in your JavaScript code world and everything
seemed working fine. 

You don't feel bad most of the time, but sometimes when 
you think of the exception, you might ask: Have I missed something?

Someone said for JavaScript develops a good chance to use try/catch would
be this case:
```
var something;
try { something = one.two.three.four.five; }
catch { something = "default"; }
finally { doSomething(something); }
```
That seems to make sense because it is indeed easy to forget to determine if an object is undefined before
reading its prop in JavaScript world. 

But what I am sure is, the people who feel suddenly see the light
with this answer would still not know when to use try/catch days later.

Because this answer is actually saying: use try/catch in places you might forget to the right thing and occur exception.

OK... that will come to an absurd conclusion: If this is true, you will need to wrap a try/catch around your every function call, because: when you call a function, you might forget to define it first. I know people are easier to forget to determine if an object exists
than forgetting to define a function, but these two things are of the same nature.


