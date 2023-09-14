
# Mastering closures in Js



##  Basic Examples
>**#1**: 
```bash

function getNewLife(age) {
    var message = "My karma score is: " + age;
    
    // This is function nesting - declaring a function inside a function.
    function nextLife() {
        // Please notice the usage of the "message" variable
        console.log(message)
    }
    
    // We can return a function from another function
    return nextLife;
}


// myNextLife is a function now.
var myNextLife = getNewLife(90);

// alerts "My karma score is: 90".
myNextLife();

// myOtherLife is another function now.
var myOtherLife = getNewLife(95);
myOtherLife();
// alerts "My karma score is: 95".

```

>**#2**: 
```bash


function squenceMaker(){
    var counter =0
  
    function sequence(){
            counter  +=1
        return "S" + counter
        
    }

    return sequence
}


const sequence=squenceMaker()

squenceMaker=null
console.log(sequence())
console.log(sequence())
console.log(sequence())
console.log(sequence())
console.log(sequence())
```
