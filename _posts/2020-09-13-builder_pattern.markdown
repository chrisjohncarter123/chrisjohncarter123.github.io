---
layout: post
title:      "Builder Pattern"
date:       2020-09-13 18:24:00 +0000
permalink:  builder_pattern
---


Sometimes, contructors can have a long list of paramaters and become very complicated in various ways. The builder pattern is a way to simplify complicated contructors by providing a ObjectBuilder class that gives an organized list of methods that may be applied in the process of creating a new object, instead of only using a single constructor.

**Example**:


```
public class Dog
{
    Dog(name, numberOfSpots, numberOfStripes, numberOfOwners ){
		    ...
		    
		}
}
```

```
class Dogs
{
    generateDogs(){
		    Dog d1 = new Dog("Spot", 6, 0, 1)
				Dog d2 = new Dog("Greg", 0, 0, 1)
				Dog d3 = new Dog("Jeff", 0, 0, 1)
				Dog d4 = new Dog("Daisy", 0, 0, 3)
		
		
		}
}
```

In the above code, most of the time, the arguments will be set to default values. One way to simplify this code is to use a DogBuilder class that allows each feature to be added individually, instead of requiring each instance to be given the same default value:



```
public class DogBuilder{

    Dog dog;

    public void reset(){ dog = new Dog(); }
		public void getProduct() { return dog; }
		public void setName(string name){ ... }
    public void setSpots(int spots){ ... }
		public void setStripes(int stripes){ ... }
		public void setOwnsers(int owners){ ... }

}
```

Now, the generateDogs method can changed to this:

```
class Dogs
{
    generateDogs(){
		    DogBuilder db = new DogBuilder();
				db.reset();
				db.setName("Spot");
				db.setSpots(6);
				Dog d1 = db.getProduct();
				
				DogBuilder db = new DogBuilder();
				db.reset();
				db.setName("Greg");
				Dog d2 = db.getProduct();
				
				DogBuilder db = new DogBuilder();
				db.reset();
				db.setName("Jeff");
				Dog d3 = db.getProduct();
				
				DogBuilder db = new DogBuilder();
				db.reset();
				db.setName("Daisy");
				db.setOwners(3);
				Dog d4 = db.getProduct();

		
		}
}
```

Although this way requires more lines, it can make it more readable to the programmer. Instead of memorizing each argument in the constructor, it can be much easier to just rember "setX". 

This example is simple, but imagine a more complicated constructor that takes 10 or more optional arguments. The builder pattern would be more useful in a situation like that.


Imagine a contructor like this:

```

class ImportantClass{
    public ImportantClass(string color, int num1, string color2, int num2, int goodNum, int greatNum, byte max){
		    ...
		}


}

```

It would be very difficult to remember the order, names, and types of each variable.


Sources:

Builder. (n.d.). Retrieved September 13, 2020, from https://refactoring.guru/design-patterns/builder
