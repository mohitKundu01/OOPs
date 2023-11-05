# OOPs

- Object-oriented programming aims to implement real-world entities like inheritance, hiding, polymorphism etc. in programming.

## Access Modifiers in Java
It helps to restrict the scope of a class, constructor, variable, method or data member. It provides security, accessibility.

__Types of Access Modifiers in Java__

There are four types of access modifiers available in Java:
1. Default - No keyword required
2. Private
3. Protected
4. Public

__1.Default Access Modifier__

When no access modifier is specified for a class, method, or data member 
It is said to be having the default access modifier by default. The data 
members, classes or method that are accessible only within the same package.

__2.Private Access Modifier__

- The private access modifier is specified using the keyword private. The methods or data members declared as private are accessible only within the class in which they are declared.
- Any other class of the same package will no be able to access these members.
- Top-level classes or interfaces can not be declared as private because
    - private means "only visible within the enclosing class".
    - protected means "only visible within the enclosing class and any 
      subclasses".

__3.Protected Access Modifier__

The methods or data memebers declared as protected are accessible within the same package or subclasses in different packages.

__4.Public Access Modifier__

- The public access modifier has the widest scope among all other access modifiers.
- Classes, methods, or data members that are declared as public are accessible from everywhere in the program. There is no restriction on the scope of public data members.
  
















