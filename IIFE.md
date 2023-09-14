# Mastering Js

>**Topic**: Immediately-invoked Function Expression IIFE or iffy

## 1: Basic Style

```bash

!function() {
    alert("Hello from IIFE!");
}(); /// Shows the alert "Hello from IIFE!"

```
>**Note**: variation can be used by replacing “!” with “+”, “-”, or even “~” as well or void

## 2: Classical IIFE style

```bash
# variation 1
(function() {
    alert("I am not an IIFE yet!");
});
```

```bash
# variation 2
(function() {
    alert("I am an IIFE!");
}());
```

```bash
# variation 3
// Variation 2
(function() {
    alert("I am an IIFE, too!");
})();
```

## 3: Return value from IIFE 



```bash
var num =(function(){
    return 1
}())
```


## 3:  IIFE with arguments


```bash

var num =(function(a,b){
    return a+b
}(7,8))
```

