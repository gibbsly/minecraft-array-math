# minecraft floating point arithmetic
a basic utiltiy pack to do math with floats and/or doubles

## 2 input functions
these functions all require the arguments `{x:(number),y:(number)}` and ouput the result to the `storage gm:io out` as well as returning the result as an int

### `gm:add`
> does `x + y`

### `gm:subtract`
> does `x - y`

### `gm:multiply`
> does `x * y`

### `gm:divide`
#### this has 2 different sets of fuctionality
when specifying `x` as a number

> does `x / y`

when specifying `x` as an array of numbers (will only divide up to the first 3 numbers in the array)

> does `[0] / y, [1] / y, [2] / y`

outputs the resulting numbers in an array in the default output location and returns the length of the outputted array

### `gm:distance`
> gets the distance between `x` and `y`

for this operation 2 position arrays must be given instead of single values. If an array is empty or values are unspecified, the values will default to 0

## single input functions
these functions only requires `{x:(number)}` as an argument

### `gm:negate`
> does `x * -1`

### `gm:reciprocal`
> does `1 / x`

### `gm:sin`
> does `sin(x)`

### `gm:cos`
> does `cos(x)`

### `gm:tan`
> does `tan(x)`

also outputs sin to `storage gm:temp var1` and cos to `storage gm:temp var2`

### `gm:square`
> does `x^2`