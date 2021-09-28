# Java Primitives versus Objects

## Java Type System
Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean. Every primitive type corresponds to a reference type.

Every object contains a single value of the corresponding primitive type. The wrapper classes are immutable (so that their state can't change once the object is constructed) and are final (so that we can't inherit from them).

## Pros and Cons
The decision what object is to be used is based on what application performance we try to achieve, how much available memory we have, the amount of available memory and what default values we should handle.

If we face none of those, we may ignore these considerations though it's worth knowing them.


## Usage
As we've seen, the primitive types are much faster and require much less memory. Therefore, we might want to prefer using them.

On the other hand, current Java language specification doesn't allow usage of primitive types in the parametrized types (generics),  in the Java collections or the Reflection API.

When our application needs collections with a big number of elements, we should consider using arrays with as more “economical” type as possible, as it's illustrated on the plot above.


## Scanning
Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

Breaking Input into Tokens
By default, a scanner uses white space to separate tokens. (White space characters include blanks, tabs, and line terminators. For the full list, refer to the documentation for Character.isWhitespace.) To see how scanning works, let's look at ScanXan, a program that reads the individual words in xanadu.txt and prints them out, one per line.