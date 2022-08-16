# Object Oriented Programming

**Object/Entity:** A thing from real world
**Class:** A template for creating objects

```csharp
public class Person
{
    // Properties
    public string FirstName {get; set;}
    public string LastName {get; set;}
    public string Gender {get; set;}
    public DateTime DateOfBirth {get; set;}
    public string Occupation {get; set;}
    // Methods
    public void PayWages() {}
    public void BookHoliday() {}
    public void Appraisal() {}
    public void Promotion() {}
    public void SaveDetails() {}
}

Person P1 = new Person();
Person P2 = new Person();
```

Creating an object from a class is called instantiation.

**Abstraction:** To simplify reality
**Encapsulation:** Hiding data and complexity
**Inheritance:** A class can derive its methods and properties from another class

- Person -- base class
- Employee & Customer -- sub class
  **Polymorphism:** A class can implement an inherited method in its own way

If in (abstract) class a method simplify with "static" keyword, without create instance of this class, this method can be called.
