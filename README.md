# Functions


**Function without parameter and without return:**
```
func function1() {
    print("function")
}
function1()
```

**Functions with parameter:**
```
func function2(param: [Int]) {
    for index in param {
        print("\(index)")
    }
}
function2(param: [1, 5, 11])
```

**Function with two parameter:**
```
func twoParametersReturningFunction1() -> [String] {
    ["1" , "2", "3", "4"]
}
let object1 = twoParametersReturningFunction1()
print(object1[2])
```

**Returns function:**
```
func returningMultipleValue() -> (returnedParam1: String, returnedParam2: String) {
    (returnedParam1: "Ahmet", returnedParam2: "Ali")
}
let object2 = returningMultipleValue()
print(object2.returnedParam1)
```

**Function with argument label 'for':** 
```
func paramaterLabel(for string: String) {
    print("Hey \(string)")
}
paramaterLabel(for: "Ahmet")
```

**Default Parameter Function:**
```
func defaultParam(_ first: String, second: Bool = true) {
    if second == true {
        print("\(first)")
    }else {
        print("\(second)")
    }
}
defaultParam("Veli")
defaultParam("Vehbi", second: false)
```

**Variadic function:**
```
func variadicFunction(params: Int...) { // params is taking different parameters with Variadic functions 
    for param in params {
        print("\(param)")
    }
}
variadicFunction(params: 4, 6, 9, 12, 5)
```


**Throw functions:**
```
enum throwEnum7 : Error {
    case throwenum7
}
func throwFunction12(_ function12: String) throws -> Bool {
    if function12 == "function12" {
        throw throwEnum7.throwenum7
    }
    return true
}
try throwFunction12("function12")
```

**inout parameters:**
```
func inoutFunction(param: inout Int) {
    param = param * 8
}
var mutableParam = 8
inoutFunction(param: &mutableParam)
```
