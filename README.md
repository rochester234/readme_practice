#**Single Responsibility Principle**

##*Introduction*

Wikipedia describes the Single responsibility principle (SRP) as being that every class should have responsibility over a single part of the functionality provided by the software, and that responsibility should be entirely encapsulated by the class.

SRP forms part of the SOLID good working practices; Single responsibility, Open-closed, Liskov substitution, Interface segregation and Dependency Inversion.

###**Reasoning**

To make our code more robust, it is important to keep a class focused on a single concern. In practice this means that only one change in a users specification should be able to affect the specification of the class. If you can think of more than one motive for changing a class, than that class has more than one responsibility.

###Example

```ruby
  class coffeeAndSoupFactory

    def coffee
    end

    def soup
    end
  end

```
It would be quite distasteful to imagine an appliance that makes coffee and soup in the same place. Generally if the class description contains 'and' then it needs to be split.

###*Conclusion*

A simple method to check for SRP is in the name choice. When you design a class, if you easily find a name for a class that specifies exactly what it defines, you're heading the right way. A difficulty to choose a name is near always a symptom of bad design.
