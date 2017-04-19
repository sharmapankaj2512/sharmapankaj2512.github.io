---
published: true
---

In groovy, ```left shift (<<)``` and ```right shift (>>)``` operators are used to achieve function composition. 

Difference between the two is that with ```right shift (>>)``` data flows from top to bottom whereas with ```left shift (<<)``` 
data flows from bottom to top.

```
def foo(t) { t + "foo" }
def bar(t) { t + "bar" }

def foobar = this.&foo >> this.&bar
def foobar_ = this.&bar << this.&foo

def barfoo = this.&bar >> this.&foo
def barfoo_ = this.&foo << this.&bar
```
#### Test Drive

```
println foobar("")  // foobar
println barfoo("")  // barfoo

println foobar("") == foobar_("") // true
println barfoo("") == barfoo_("") // true
```
