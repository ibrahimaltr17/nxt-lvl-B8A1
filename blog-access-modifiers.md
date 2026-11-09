Title: How access modifier works on type script
Introduction: Access modifier was an important part while learning Type script OOP. Public, Private, readonly and protected are main access modifier of type script. 

body: The default modifier is public, where we can access from outside of class.

class Student {
  public name: string = "Ibrahim";
}

const student = new Student();
console.log(student.name);

Here name can be access from outside.

If we use private the property can access from inside own class.

class Student {
  private password: string = "12345";
}

Protected is kind of same as private, but there is a different. It can access from own class and child class of own class.
example: 
class Person {
  protected name: string = "Ibrahim";
}

class Student extends Person {
  showName(): string {
    return this.name;
  }
}

At last readonly use set a unchangeable value of a property. The value is set while declaration. 

Conclusion: Overall access modifier help us to control the data of class. If we understand how public, private, protected and readonly works in type script OOP, it will be more easy to work on OOP.
