
# Polymorphism &amp; Composition Homework - Quiz


### Polymorphism <br />

#### 1. What does the word 'polymorphism' mean?

Poly means many and morph means change - It means something can have many forms.

#### 2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It means we can wrap our objects in an enclosing type that defines a contract method between them all. 

```

public interface IConnect {
  public String connect(String data);
}
```


#### 3. What can we use to implement polymorphism in Java?

We can use Inheritence or Interfaces - its better to use interfaces.
Implementing polymorphism using inheritence can get messy. 
Using it through interfaces means you can treat a class as being of another type. When a class impliments an interface it gains the type of the interface
without having an inheritence chain. You can have as many interfaces as you like, rather than one superclass. 


#### 4. How many 'forms' can an object take when using polymorphism?

It can have many forms.

#### 5.Give an example of when you could use polymorphism.

You could use polymorphism in a case where you have multiple classes and the classes have some identical properties. You could make an interface to create a method which associates with that poperty and can then be used in each of the appropriate classes. 


## Composition and Aggregation

#### 6. What do we mean by 'composition' in reference to object-oriented programming?
   With composition an object is seen as being part of another object. Like a room is part of a house. It is composed of other objects.
   It also means it has ownership of the other object. This means that if the object is destroyed all the other objects it is composed 
   of are also desroyed.

#### 7. When would you use composition? Provide a simple example in Java.

You would use composition when you have an object composed of other objects linked to the main oject for example a house with a roof

```

class Roof {
    private int width;
    private int length;
    private String type;

    
}

class House {
    private Roof roof;
    
    public House() {
        this.roof = new Roof();
    }
}
```


   


#### 8. Give a difference between composition and aggregation?

  With Aggrigation the objects can exist independantly from the object that contains them. You can create the objects seperatly and implement them in the class.


#### 9. What is/are the advantage(s) of using composition/aggregation?
   Composition and Aggregation allow a class to use behaviour from a group of other classes, 
   and makes it possible for that behaviour to change at runtime.


#### 10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?
  They are also destroyed.

#### 11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?
      They still exist independanly of the destroyed object.

        
