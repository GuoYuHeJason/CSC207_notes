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

































    
