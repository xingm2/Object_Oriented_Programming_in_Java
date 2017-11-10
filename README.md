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
