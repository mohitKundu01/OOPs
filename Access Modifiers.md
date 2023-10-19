# Access Modifiers in Java
Access Modifiers help to restrict the scope of a class, constructor, variable, method or data member.
It provide security, accessibility, etc to the user depending upon the access modifer used with the element.

## Type of Access Modifiers in Java
There are four types of access modifiers available in Java
1. Default - No keyword required
2. Private
3. Protected
4. Public

### 1.Default
When no access modifier is specified for a class, method, or data member - It is said to be having the default
access modifer by default.
The data member, method, class which can't specified/declared by using any access modifer and they are only accessible
within the same package only.

```Java
// java Program to illustrate default modifier
package p1;

// class Geek is having Default access modifer
class Geek{
    void display()
{
   System.out.println("Hello World!);
}
```

```Java
// Java program to illustrate error while  
// using class from different package with  
// default modifier  
package p2;  
import p1.*;  
  
// This class is having default access modifier  
class GeekNew  
{  
    public static void main(String args[])  
    {  
        // Accessing class Geek from package p1  
        Geek obj = new Geek();  
  
        obj.display();  
    }  
}
```
Output: Compile time error.

### 2. Private Access Modifier
The private access modifier is specified using the keyword private. The methods or data member is 
accessible only within that class in which they declare.
#### Note: Any other class of the same package will not able to access these members.
#### Note: Top-level classes or interfaces can not be declared as private because
-> Private means "only visible within the enclosing class"
-> Protected means "only visible within the enclosing class and any subclasses"



```Java
// Java program to illustrate error while 
// using class from different package with 
// private modifier 
package p1; 

class A 
{ 
private void display() 
	{ 
		System.out.println("GeeksforGeeks"); 
	} 
} 

class B 
{ 
public static void main(String args[]) 
	{ 
		A obj = new A(); 
		// Trying to access private method 
		// of another class 
		obj.display(); 
	} 
} 

```


### 3.Protected Access Modifier
The data members or methods are only accessible within the same package or subclasses in different packages



### 4.Public Access Modifier
. The Public access modifer is the widest scope among all other access modifiers.
. Classe, method, data members that are declared as public are accessible from everwhere
  in the program. There is no restriction on the scope of public access modifier.

Program 1:
```Java
// Java program to illustrate 
// protected modifier 
package p1; 

// Class A 
public class A 
{ 
protected void display() 
	{ 
		System.out.println("GeeksforGeeks"); 
	} 
} 

```

Program  2:
```Java
// Java program to illustrate 
// protected modifier 
package p2; 
import p1.*; // importing all classes in package p1 

// Class B is subclass of A 
class B extends A 
{ 
public static void main(String args[]) 
{ 
	B obj = new B(); 
	obj.display(); 
} 
	
} 
```













