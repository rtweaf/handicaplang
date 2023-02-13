# handicaplang
A lightweight and coherent programming language.

# Syntax examples

## Comments
```
# inline comment
```

## Variables
```
x: int
x = 1
y: char = 'a' # type is optional
```

## Arithmetic operators
```
p = ((a+b) * h) / 2
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
x = (x << n) | (x >> (8-n))
```

## Vectors
```
x = [0, 1, ['x', 'y']]
x[x.len-1] = x[x.len-1] + ['z']
```

## Funtions
```
f(a: int, b = 2): int # prototype
f() = {
  return a * b
}
```

## Structures
```
Name: OtherStructure {
  field1 = 0
  _field2: int # fields with underscore are private
  (field2: uint32) {
    # constructor
    field2 = self.field2
  }
}

x: Name(10)
y = Name(x.field1)
```

## Streams
```
stdout <- "Hello World"
stdin -> buf
file('asdf.txt') <- 2*16: str # x: y is cast x to y type
```
