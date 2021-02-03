# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

    -> Polymorphism means 'Many forms'. We can perform a single action in ways.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

    -> An example of polymorphism and inheritance with classes and subclasses, where we can implement the sound 
    method but can return a different message each time. 

    public class Animal {
    
        public String sound(){
            returns "I'm making a sound";
       }   
    }
    
    public class Dog extends Animal {
        
        public String sound(){  
            returns "Woof, woof!";
        }
    }
    
    public class Bird extends Animal {
        
        public String sound(){  
            returns "Tweet Tweet!";
        }
    }


3. What can we use to implement polymorphism in Java?

    -> We can use two methods to implement Polymorphism:

    1. Method overloading (static polymorphism) - where multiple methods can have the same name but contain different 
        types of parameters, different number of parameters or have the parameters in a different order. 
    2. Mehod overriding (dynamic polymorphism) - where a subclass/child class implements a method already used by 
        its superclass/parent class and 'overwrites' the previous method

4. How many 'forms' can an object take when using polymorphism?

    Many forms. 

5. Give an example of when you could use polymorphism.

    To take advantage of the fact that an object can take many forms; to refer to the child class by using the parent 
    class reference. 
    
    E.g. You can draw() a Shape. [Parent class]
                      (Extends to)
         You can draw() a Triangle [child/subclass]
         You can draw()  a Square [child/subclass]
         You can draw() a Circle [child/subclass] 
    


# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

    It describes the relationship or association between objects. 
    A class that references one or more objects of other classes; a 'has-a/an' association. 
    A car has an engine, tyres etc. 

7. When would you use composition? Provide a simple example in Java.

    You would use composition for code reuse - for example:
        A Person has a Job. 
        Write the role, salary, id in the Job. Then you can re-use this by simply referencing private Job job; , 
        and reusing this code. 

8. What is/are the advantage(s) of using composition?

    -> The ability to reuse existing code without hainvg to use inheritance and potentially creating a long messy chain
    -> Can control the visability if other object classes (encapsulation)
    -> Can change classes without breaking code 

9. When an object is destroyed, what happens to all the objects it is composed of?

    -> They will also be destroyed. E.g. if the Car object in the example above is destroyed then all of the objects 
        associated with it engine, tyres will also be destroyed. 