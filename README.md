lexicographic-tuples
====================

Go library for encoding and decoding tuples of values that sort lexicographically.

Import as `github.com/sburnett/lexicographic-tuples` and use as `lex`.

```Go
import (
    "github.com/sburnett/lexicographic-tuples"
)

// ...

encodedValue := lex.EncodeOrDie("hello, world!", int32(42))

var greeting string
var meaningOfLife int32
lex.DecodeOrDie(encodedValue, &greeting, &meaningOfLife)

```
