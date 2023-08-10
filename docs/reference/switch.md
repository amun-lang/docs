Amun has both switch statement and expression

## Switch Statement

By Switch statement is used to execute the branch if his case value is equal to the argument,
but you can also override the equality checks with any comparisons operator such as (==, !=, >, >=, <, <=).
and if no value match it will return the value of default block.

```
switch (10) {
    1       -> printf("One");
    2, 4    -> printf("Two or four");
    else    -> printf("Else");
}

var x = 10;
switch (x, >) {
    1       -> printf("x > 1");
    2, 4    -> printf("x > 2 or x > 4");
    else    -> printf("Else");
}
```

## Switch Expression

Switch expression is used to return a value of branch if his case value is equal to the argument, but like the switch staement you can also override the operator by any comparisons operator such as (==, !=, >, >=, <, <=).

```
var result = switch (10) {
    2, 4, 6, 8 -> true;
    else -> false;
};

var x = 10;
var result2 = switch (x, <) {
    2, 4, 6, 8 -> true;
    else -> false;
};
```

## Compile time switch expression

If the condition and all values are constants and can resolved during the compile time you can use it as value for global variable

```
var build_flavor = Build::RELEASE;
var config = switch (build_flavor) {
    Build::DEBUG   -> 1;
    Build::RELEASE -> 2;
    else           -> 3;
};

fun main() int64 {
    return 0;
}
```