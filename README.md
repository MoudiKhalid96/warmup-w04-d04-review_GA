[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)<br>
![Misk Logo](https://i.ibb.co/KmXhJbm/Webp-net-resizeimage-1.png)<br>
<small style="color: gray">This was work from <span title="General Assembly">GA</span> and Misk Academy</small><br>

## Requirements

Respond to the following questions based on what we've learned (and maybe what we haven't covered yet).

---

## Questions

1. What's the difference between **member variables** (also called **instance variables**) and **class variables** (with the `static` keyword)? Which can be accessed without creating an instance of the class?<br>
member variables: can't access it without creating an instance of class.<br>
static variables: can be accessed without creating an instance of class.
<br><br>

2. Does it make sense to write **getter** and **setter** methods for a `public` member variable? What about `private` variables?<br>
No, set and get methods used to access vaiables when use it outside the class.
<br><br>

3. What are some benefits of making member variables `private`?<br>
To protect code from the other codes and from accessing it directly outside the class
<br><br>

4. If Class A extends Class B, which is the superclass and which is the subclass? Which would you call the parent, and which would you call the child?<br>
Class A: subclass, child.<br>
Class B: superclass, parent.
<br><br>

5. What does it mean for a class to **inherit** methods or variables (or both) from its parent class?<br>
Means to inhirit all variables and methods in superclass, and can over-write the methods.

6. Consider the following code, where the `Refrigerator` class extends the `Appliance` class, and `getTemperature()` is a method in `Refrigerator`, but **not** in `Appliance`:

    ```
    Appliance myAppliance = new Refrigerator();
    double temperature = myAppliance.getTemperature();
    ```

   Why will this call to `getTemperature()` cause an error? How will **casting** help solve this issue?<br>
It's causing an error because the method is in `Refrigerator` class, not int `Appliance` class.<br>
In order to solve this,  down-casting must be used like this:<br>
```
double temperature = ((Refrigerator) myAppliance).getTemperature();
```
<br><br>

7. In a normal class (also called a **concrete** class), do you need to **implement** all the methods, or can you simply **declare** some? What about in an `abstract` class?<br>
Abstract class: must be implement the abstract methods, other methods are optional to implement.
Concret class: methods are optional to implement
<br><br>

8. What about an `interface`? Can you implement any methods in an `interface`? Can you declare methods in an `interface`?<br>
Interface is a fully abstarct, methods can be declared but not implemented.
<br><br>

9. Can you create an instance of an `abstract` class? Also, look up the Java keyword `final` and see if you can explain why a class **cannot** be both `abstract` and `final`.<br>
Abstarct classes is in-complete, so that's why can't create an instance of it.<br>
Final classes is a completed class and un-extendable classes.<br>
they're both mutually exclusive.
<br><br>

10. What happens when a method **overrides** another method? If parent and child classes have methods with the same name, when you call that method on an instance of the child class, which implementation of the method will be executed?<br>
The method that the **child class** override it.
<br><br>

11. What's the relationship between `List`, `LinkedList`, and `ArrayList`? <br>
They're all implements `Collections` interface.
<br><br>

### Deliverable

This file, with your answers added.

---

## Additional Resources

Refer to the "Classes and Objects" lesson, the "Subclasses" lesson, and the "Abstract Classes and Interfaces" lesson.

Feel free to do a Google search for these concepts as well. There are plenty of Java tutorial websites and Stack Overflow posts that can help you. But be sure to write up your answers in your own words — copying and pasting some text does **not** help you actually learn (and is, in fact, cheating).
