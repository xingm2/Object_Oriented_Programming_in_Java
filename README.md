# Object_Oriented_Programming_in_Java
by University of California, San Diego
   
-- Setting up map visualization
setup() // excuted once

    size() // set canvas dimensions
    
    MapUtils.createDefaultEventDispatcher(); // create interactivity

draw()   // excuted repeatedly

    background() // set canvas color
    
    map.draw() // draw a map legend using methods from Processing library

-- Adding content

    map.draw will go through all the objects that are associated with our attached to our map object and will refresh them as well.

-- ArrayLists and Generics
List<Feature> countries = new ArrayList<Feature>();
List is an Abstract data type, interface
ArrayList is actual java class implements list behaviors
To have a interface as the type of the variable, and the actual class as the type of the thing you instantiated
   
ArrayList is in java.util
    Array vs ArrayLists
    
    countryArray[0] = f;
    coutries.set(0,f);
    
    int len = countryArray.length;
    int len = countries.size();
    
    Feature f = countries.get(0);
    
-- Module 3 Programming Assignment Walkthrough
    
    With GUI coding, do not hesitate to use javadoc
    
    
-- Week 4


base/super class VS derived/sub class

Private vars can be accessed only through public methods

Person p = new Student(); // since a student "is-a" person

Rule of thumb: Make member variables private (And methods either public or private)

protected : can access from same class
            can access from same package 
            can access from any subclass
            
package :  can access from same package

NEW Rule of thumb: always use either public or private

"new" means create memory space, and it's an operator

Objects are created "inside out" : Indirect Superclass -> superclass -> subclass

--- Compiler Rules
1. No superclass? Compiler inserts: extends Object
2. No constructor? Java gives you one for you.
3. 1st Line of a constructor must be either: this(args) or super(args); otherwise, Java inserts: "super();" (means it's gonna insert a call to the default constructor of your super class)

--- Overloading vs Overriding
Overloading: same class has same method name with different parameters
Overriding: subclass has same method name with the same parameters as the superclass

Println automatically calls toString if you pass an object as a parameter to print line.

--- Polymorphism
---- compile time and runtime
step 1. Compiler interprets code
step 2. runtime environment executes interpreted code
---- compile time rules
1. compiler only knows reference type
2. can only look in reference type class for method
3. outputs a method signature
---- run time rules
1. follow exact runtime type of object to find method
2. must match compile time method signature to appropriate method in actual object's class


---- Casting

Automatic type promotion (like int to double)
Superclass ref = new Subclass(); //widening

Use casting of objects to aid the compiler
Explicit casting (like double to int)
Subclass ref = (Subclass) superRef;  // narrowing

Person s = new Student("Cara",1234); // person dont have this method 'getSID', but student has this
s.getSID();
Compile Time Error!
((Student)s ).getSID(); // Works fine this time!

Person s = new Person("Tim"); // person dont have this method 'getSID'
((Student)s ).getSID();
Runtime Error! Java.lang.ClassCastException: From Person to Student

---- Runtime type check
instanceof 

---- Interfaces
Interfaces only define required methods
Classes can inherit from multiple interfaces
Abstract class or interface?
1. if you just want to define a required method: Interface
2. if you want to define potentially required methods AND commen behavior: abstract class

--- Project
1. figure out class hierarchy.
2. predict
3. identify changes
4. IsLand method -> IsInCountry
5. printQuakes: all the eq in each country, use "country" property in the earthquakes
6. test
7. UML,look into EarthquakeMarker -> SimplePointMarker -> Marker
8. complete the method definition for draw()
9. drawEarthquake() and LandQuakeMarker()

-- Week 5
MapUtils.createDefaultEventDispatcher(this, map); // make our map interactive

PApplet implements (MouseListener and KeyListener)
UnfoldingMap implements EventListener
