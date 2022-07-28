# Go features

### Interfaces
```
type x interface {
    func Name() string
    func Age() int
}

type Person struct {
  ...
}

func (*Person) Name() {
  ...
}

func (*Person) Age() {
  ...
}
```

Interface describes terms (functions) that a type should have to correspond to that interface.
<br>It allows to have one function that accepts different types as an argument which is very convenient.


### Passing variables by pointer
````
func (*Person) Name() {
  ...
}
````
Passing variables by pointer is considered best practices in Go. It helps save memory because pointers size is only one byte when a variable can have much more. Some types of variables are pointer based like arrays, slices and maps so no * is needed.


