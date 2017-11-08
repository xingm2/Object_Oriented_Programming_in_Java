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
