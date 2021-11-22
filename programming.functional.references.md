---
id: 5mU9OZs48hBYyTa8CIQYG
title: References
desc: ""
updated: 1636914348346
created: 1636819650037
---

## FP Examples

https://github.com/alzateja/compare-api-tool

## FP Guides

http://www.tomharding.me/fantasy-land/ and the rest of his blog. He has many posts that I don't understand yet

## Libraries

- https://github.com/natefaubion/adt.js/
- https://github.com/fantasyland/fantasy-land
- https://github.com/fantasyland/daggy

### What does **catamorphism** mean?

It is used here in reference for pattern matching http://www.tomharding.me/2017/03/03/fantas-eel-and-specification/

### Type variables

are the variables used in a Heiner Miller type system

### Type Constraints:

```javascript
equals :: Setoid a => a -> a -> Bool
```

### Parametricity

https://en.wikipedia.org/wiki/Parametric_polymorphism

Constraints are very important. When we have a signature that involves a type variable with no constraints, we know that the function can’t manipulate it in any way. We know by looking at the signature id :: a -> a that all it could ever do is return the value it has been given, because we know nothing else about a - it could be a number, or a function, or anything! This feeds into an idea called parametricity that we’ll come back to several times in this series.

### Setoids

http://www.tomharding.me/2017/03/09/fantas-eel-and-specification-3/

A **setoid** is any type with a notion of equivalence. You already use plenty of setoids (integers, booleans, strings) almost every time you use the == operator, so this shouldn’t be too tricky. You also use things that aren’t setoids, like functions.

### Semigroups

http://www.tomharding.me/2017/03/13/fantas-eel-and-specification-4/

They are for concat or merging things together. It is different then reduce since reduce removes the surrounding data while this maintains it.

### Monoid

http://www.tomharding.me/2017/03/21/fantas-eel-and-specification-5/

Has a emptyfunction so that these laws are valid

```javascript
MyType(x).concat(MyType.empty()) === MyType(x);

MyType.empty().concat(MyType(x)) === MyType(x);
```

Monoids enable reduce/folding since u can use empty as the initial value
![](/assets/images/2021-11-14-12-24-50.png)
