# Variables

In Go, variables are explicitly declared and used by the compiler to e.g. check type-correctness of function calls.

# Rules for Naming Variables:

- Variable names must begin with a letter or an underscore(_).
  And the names may contain the letters ‘a-z’ or ’A-Z’ or digits 0-9 as well as the character ‘_’.

```
Test, test, _test123  // valid variable
123Test, 23test      // invalid variable
```

- A variable name should not start with a digit.
- The name of the variable is case sensitive.

`test and Test are two different variables`

- Keywords is not allowed to use as a variable name.
- There is no limit on the length of the name of the variable, but it is advisable to use an optimum length of 4 – 15 letters only.

---

- `var` declares 1 or more variables.
- You can declare multiple variables at once.
- Go will infer the type of initialized variables.
- Variables declared without a corresponding initialization are _zero-valued_. For example, the zero value for an `int` is `0`.
- The := syntax is shorthand for declaring and initializing a variable, `var variable_name type = expression`

e.g. for
`var f string = "apple"` in this case.

Example of the above using a simple code snipette

```go
package main

import "fmt"

func main() {

    var a = "initial"
    fmt.Println(a)

    var b, c int = 1, 2
    fmt.Println(b, c)

    var d = true
    fmt.Println(d)

    var e int
    fmt.Println(e)

    f := "apple"
    fmt.Println(f)
}
```

The Output would be:

```go
$ go run variables.go
initial
1 2
true
0
apple
```

# Resources & References

[Go Variables - GeeksforGeeks](https://www.geeksforgeeks.org/go-variables/)
