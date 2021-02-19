# designPatterns
designPrinciples example
SOLID
SOLID Principles
:::::::: Single Responsibility Principle : Separate of Concerns(mainly Loosely Couple (LC)/High Cohesion(HC))
1. Create component which handle  unique responsibility.
2. Group functionality by class rather than adding entire fn in to one class
Eg:  We have a collection class where we add our fav images, videos, audios etc.
So adding , printing, deleting functionality can be grouped in to in to collection class.
Other Persistence items like editing , loading etc can be grouped in to some X class or a pPersistence class

***Take away: A class should only have one reason to change
Separation of concerns- diff class handling diff indecent task/prob

Refer (design-patterns/SOLID/single-resp.js)

:::::::: Open-clossed Principles

 Open for extension closed for modification.

It is not wise or we can say it is expensive to modify product deployed code(reg testing , entire module testing and  at the end there are chances to produce speggettyi code)

Example  product Filtering (filter by color, later req comes for filter by size, later filter by both, later filter by OR)

***Take away: 
Better is to separate req 
	create combitaors to combine specification

Refer (design-patterns/SOLID/open-clossed-principles.js)

::::::::  Liskov substitution Principles

 A function aspect a base class as a param, it should accept derived class also as a param without breaking the existing functionality

***Take away: U she be able to substitute a base type for a subtype

:::::::: Interface Segregation Principles——— 460…10 / 23
Actually in JS this principle is kind of mute because in Js we dont have interfaces, as it is duck type.

So basely this approach is kind of segregation of interface , it is kind of creating abstract (not having a physical or concrete existence)bas classes and extending it. for e.g.:  if we have a machine class refer the principle js
(design-patterns/SOLID/Interface-egregation-Principles.js)

***Take away: Dont put too. Much in to an interface split int o separate interfaces

YAGNI: if the usr/client dont want that modules dont face them to implement it.

:::::::: Dependency Inversion Principles

High Level Modules should not depend on low level Modules

For Eg in the js, the Research class should not depend on relationship module

Main take away here is to create an abstract method or follow an abstract approach to make the dev as well as test simply and less troublesome.
