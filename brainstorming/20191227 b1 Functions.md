# B1 Function definition

## Proposed implementation

Main option similar to Rust:
```
fn add_one_v1(x: u32) -> u32 { x + 1 }
fn add_one_v1(x)             { x + 1 }
             |x|             { x + 1 }
             |x|               x + 1

fn greeting(name: str) -> str {
    "Hello " + name
}
```

Alternative 1:
```
fn add_one_v1(x: u32) -> u32 {
    x + 1
}

Closure:
x x + 1 
x,y x + y
x,y {x + y}
```

Alternative 2:
```
var multiply = (a, b) => { a * b }
```

## How it is implemented in other languages
Python
```python
def greeting(name: str) -> str:
    return 'Hello ' + name

lambda x: x + n
```

Rust
```rust
fn another_function() {
    println!("Another function.");
}

|x| x + 1;
```

Scala
```scala
def foo(x: Int = 6, y: Int = 7): Int = x + y

(x: R) => x * x
(1 to 5).reduceLeft(_ + _)
```

Clojure
```clojure
;;    name   params         body
;;    -----  ------  -------------------
(defn greet  [name]  (str "Hello, " name) )
```
Lisp
```lisp
(defun name (parameter-list) "Optional documentation string." body)
```

Haskell
```haskell
add :: Integer -> Integer -> Integer   --function declaration 
add x y =  x + y                       --function definition 
```

OCaml
```ocaml
fun n -> n + 1;;
let average a b =
  (a +. b) /. 2.0;;
let f = fun n -> n + 1;;
```

F#
```Fsharp
let f (x : int) = x + 1
let f x = x + 1
let f x = (x, x)
```

C#
```csharp
public int AddNumbers(int number1, int number2)
{
    int result = number1 + number2;
    return result;
}

Func<string,string> myFunc = var1 => "some value";
```

Java
```java
public class Math
{
     public static    int multiply(   int a,    int b) { return a*b; }
     public static double multiply(double a, double b) { return a*b; }
}
```

Javascript
```javascript
function multiply(a, b) { 
  return a*b; 
}

var multiply = (a, b) => a * b;
var multiply = (a, b) => { return a * b };
```
