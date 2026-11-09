# Differences between type aliases and interface
Introduction: We use type alias and interface for set the data type of a variable or object. It looks quit same but there is difference.
Body: We can use type alias for set data type with a new name. And create primitive type, union type and tuple. 
example:
```ts
type Student = {
  name: string;
  age: number;
};

type UserID = string | number;

type Status = "active" | "inactive";
```
Here Student create an object structure. On the other side it created UserID and status data type which is not possible using interface.
Interface use for object tructure.
 ```ts
interface Person {
  name: string;
  age: number;
}

interface Student extends Person {
  studentId: number;
}
```
Here we get name and age from Student interface. Means using extends we can create one interface to another. 

Conclusion: Main different is interface with same name can connect the property. But can not add same type alias.

Conclusion: I think type alias is more flexible, cause it can create various kind of data type. And interface it better for create object structure and uses of extends. Basically we can use both in object according to the requirement.
