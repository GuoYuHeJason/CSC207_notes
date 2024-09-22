Java compiler (Java c): .java to .class(bytecode)
JVM (java): excute .class, translate

Overloading: same name, different parameter type/number

Call methods (Overriding): always lowest 
@Override
public String toString(){
    return "My name is " + this.name;
}


But abstract method needs to exist in current class, use casting to change current class
Call attributes (Shadowing) : current class, can be changed by casting

Arrays.copyOf :deep copy

hashCode, equals, memory address?

Static
https://github.com/CSC207-UofT/207-course-notes/blob/master/02-classes-in-java.md#27-class-static-methods
https://github.com/CSC207-UofT/207-course-notes/blob/master/02-classes-in-java.md#22-variables-in-classes
static can be called by both class name and instance name, don't have access to instances

this is only used when 
this.name = name
(already declared with the class)
differentiate between local and global variable (constructor)
other times don't have to 

Comparable
the sort method requires that all elements in the array must implement the Comparable interface. This interface in turn requires any class that implements it to define this method:

int compareTo(T o)
    Compares this object with the specified object for order.
    Returns a negative integer, zero, or a positive integer
    as this object is less than, equal to, or greater than
    the specified object.

    @Override
    public int compareTo(Review other) {
        if (this.rating < other.rating) {
            return -1;
        } else if (this.rating > other.rating) {
            return 1;
        } else {
            return 0;
        }
    }

    The comparator interface
    https://github.com/CSC207-UofT/207-course-notes/blob/master/02-classes-in-java.md#29-comparator



Quiz 2 (string pool):
        System.out.println("1" == "1");
True







    Interface
    class Myclass implements Myinterface













Generic Classes
T
Allows code to work with multiple types without complie time error








Week 3

Overriding: variables don't get overriden, but when method gets overriden and method calls for that variable, because method is in child class, it calls the child class variable.

# Java visualizer doesn't show the parent variable


class A { 
int x = 5;
void printX() { System.out.println(x); } 
} 

class B extends A { 
int x = 10;
void printX() { System.out.println(x); } 
}

What will be the output if we execute the following code?

A a = new B();
a.printX();
System.out.println(a.x);


Ask about 
Run time exception
and 
Compile time error

On mentimeter
What is the difference between Run time exception and Compile time error, how do we distinguish them?
































    
