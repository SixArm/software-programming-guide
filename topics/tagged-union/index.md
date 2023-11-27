# Tagged unions

Tagged unions, also known as algebraic data types, enable complex data structures that can hold different types of data. They are commonly used in functional programming languages like Haskell, OCaml, and Rust.

A tagged union is a data structure that has a fixed set of possible types, each of which is associated with a tag. The tag identifies which type the value of the union is currently holding. The structure of a tagged union is similar to that of a C union, but the difference is that a tagged union allows you to store multiple types of values in a single variable.

The tag of a tagged union allows the program to know which type of data is stored in the union at any given time. The tag can be a simple integer value, an enumerated value, or even a string. Depending on the programming language, the tags may be implicit or explicit, meaning they are either built into the language or defined by the programmer.

For example, a tagged union in a programming language might define a "Shape" type that could hold values of type "Rectangle", "Circle", or "Triangle". Each of these types would have its own set of properties and methods, allowing the program to manipulate them in different ways.

Tagged unions can be useful for modeling complex data structures in a way that is both efficient and easy to read. They can be used to represent a wide variety of structures, from simple lists to more complex tree structures. They are also useful for creating extensible data structures, as new types can be added to the union without breaking existing code.

One potential drawback of tagged unions is that they can be difficult to work with if the tag values are not well-defined. If the tags are not well-defined, it can be easy to accidentally access the wrong type of data or to introduce bugs into the code.