# handicaplang
A lightweight and coherent programming language.

# Syntax examples

## Comments
```
# inline comment
```

## Variables
```
# defnition
name: type
# declaration
name = x
# initialisation
name: type = x
# or
name := x
```

## Arithmetic operators
```
p := ((a+b) * h) / 2
```

## Logical operators
```
x == y || (y > 4 && y < 8) # true or false
```

## Conditional statements
```
? logicalOperatorsExpression {
  # if
} ! {
  # else
}
```


## Foreach loop
```
i @ x {
  # process i
}
```

## Bitwise operators
```
x := (x << n) | (x >> (8-n))
```

## Vectors
```
x := [0 ... 10]
x = x[x.len-1] + 1
```

## Funtions
```
# prototype
name(): type
name(arg1: int32, arg2: int32, arg3 = 10): type
# initialisation
name() := {
  # code
  return x
}
```

## Structures
```
Name: OtherStructure {
  field1 = 0;
  _field2: uint32; # fields with underscore are private
  (field2: uint32) {
    # constructor
    field2 = self.field2
  }
}

# instance
x: Name(10)
y := Name(x.field1)
```

## Streams
```
stdout <- "Hello World"
stdin -> x # read from stdin to x
file('asdf.txt') <- 2*16: str
```
