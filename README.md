# conv
Golang library for safe base type conversion and struct/map manipulation.

## Install

go get github.com/night-codes/conv

## Documentation
[Docs on pkg.go.dev](https://pkg.go.dev/github.com/night-codes/conv)

## How to use

```golang
package main

import (
    "github.com/night-codes/conv"
    "fmt"
    "reflect"
)

func main() {
    a, b, c := "8", 1, 1.04
    a2, b2, c2 := conv.Rune(a), conv.Float64(b), conv.String(c)

    fmt.Println(a2, b2, c2)
    fmt.Println(reflect.TypeOf(a2), reflect.TypeOf(b2), reflect.TypeOf(c2))
}

// out :
// 8 1 1.04
// int32 float64 string
```

## License
The BSD 3-Clause License

Copyright (C) 2015 Oleksiy Chechel <alex.mirrr@gmail.com>
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided
that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions
   and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and
   the following disclaimer in the documentation and/or other materials provided with the distribution.
3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or
   promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
