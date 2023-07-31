```bash
daml new <porject name>

daml studio
```

## Primitive datatypes
Numbers, Text, Booleans, Dates

`let` allows us to bind variables locally inside a block

Int 64-bit, signed 9.2 quintillion

Numeric n, precision up to 0-37 decimal digits

Decimal Numeric preset to 10

BigNumeric 2^15 decimal only intermediate compuations

date YYYY-MM-DD 0001-01-01 to 9999-12-31
date function `date 2022 Jan 01`

Time 

RelTime difference between 2 times values


### Collection Data structures

#### Lists

```haskell
intList = [1,2,3]
[10 .. 20]
[2, 4 .. 20]

fruitList = ["apple", "banana", "pineapple"]

--append no mutation
"mango" :: fruitList

--append with mutation
["mango"] <> fruitList
["mango"] ++ fruitList
```

head, tail, last, sort, init, reverse, take, elem, length

for Number lists:
sum, product

#### Tuples

can contain multiple datatypes

fst
snd
nTuple

#### Set

removes duplicate instances

#### Maps

key value pair
Map.lookup "key" wordMap
newMap = Map.insert "key" "value" oldMap

### Typeclasses

interfaces for functions
implemented by datatypes

Datarecord
tupple with fields having a name

custom typeclasses

```
class Encryptable i o where
  encrypt: i -> o
```