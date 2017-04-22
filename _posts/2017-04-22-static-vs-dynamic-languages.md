---
published: true
---

Yes I know, already enough has been said and written about this topic :)

Fortunately, I have got opportunities to work with both static (C#, Java) and dynamic (Python, Groovy) languages. And after my first hand experience with these different languages, I have transitioned from being a hard core static language evangelist to be a more pragmatic developer. Now I am convinved that we need both and it is just about choosing the right one to get the job done cleanly.

In one of my recent gigs, I came across a xml manipulator written in Java. All it did was parse the xml and store it in database. The xml was huge and hence the code had lots of pojos with an awful lot of fields. Addition of a simple field in xml resulted in changes to praser, pojos and database layer. Messed up, duplicate code made things even worse.

We ended up re-writting this module in Groovy and it turned out to be a good decision. Groovy not only helped us in reducing the boiler plate code but also adding new fields became trivial. In order to improve readability of the code we employed [Martin Fowler's - Embedded Document Pattern](https://martinfowler.com/bliki/EmbeddedDocument.html). Embedded document pattern was the icing on the cake as it improved overall readabilty of the code significantly.

For me both static and dybamic laguages are winners of this age old debate!
