# Objects

## What you will learn

  - Create basic objects
  - Get/set object fields
  - Run object methods
  
  
 Now let’s put together everything we have learned so far. 
  - **Objects** are code entities with ```state``` and ```behavior```. 
    - The ```state``` is represented by **variables** which make up various properties or attributes. 
    - The ```behavior``` is managed by **functions** the object can run; typically, these functions modify the ```state``` in some way. 

JavaScript is **not** a true object-oriented language so these objects act more like ```key-value``` structures such as maps or dictionaries in other languages than like true objects. 

When we use JavaScript objects, we create the **blueprint** and fill in the values at the same time. 
  - Each **value** needs a ```key``` which acts similar to a variable name. Even functions are mapped onto keys.

    For example, let’s say I wanted to create a ```gameCharacter``` which had a ```name```, ```pos```, and ```health``` and     could change its ```pos``` with a ```move``` function:

```
var gameCharacter = {
  name: “Nimish”,
  pos: 2,
  health: 100,
  move: function(byAmount) {
    this.pos += byAmount;
  }
}
```

We’re doing quite a bit here so let’s start at the top. 

  1. We create a variable called ```GameCharacter``` that, instead of containing a single value or a list of values, contains some ```key-value``` pairs. You can see for the first three ```key-values``` the keys are the names of variables and the values are whatever values we want the ```gameCharacter``` to have at that time. 
  2. The ```move``` function is mapped to the ```move``` key and we will show you how to use that in a minute. 
  3. The last thing I want to point out here is the use of the “```this```” keyword. This just signifies we are changing the ```pos``` value which belongs to the currently working object.
  
With JavaScript **objects**, we can use them right at the time of declaration. If we wanted to get the attributes of ```gameCharacter```, we use ```dot``` syntax like this:

```
var name = gameCharacter.name;
var pos = gameCharacter.pos;
var health = gameCharacter.health;
```

Similarly we can change those values like this:

```
gameCharacter.pos = 10;

```

Or by calling the ```move``` function (although this only changes ```pos```):

```
Or by calling the move function (although this only changes pos):

```

This calls whatever is stored at the ```move``` key (in this case a function which needs one value passed into it). 
  - So although JavaScript objects are not true objects such as you might see in object-oriented languages like Java, they serve a similar purpose as data structures which contain multiple values to make up their ```state``` and ```functions``` which allow them to execute ```behaviors```. 
  
  
Try to add more values and functions to this object and then try creating your own custom objects.

---
