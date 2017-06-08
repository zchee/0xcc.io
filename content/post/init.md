+++
date = "2017-06-08T17:34:03+09:00"
title = "init"
+++

This is first my blog article.

pseudo code. no meaning.

```go
package main

const int3 = 0xcc

func main() {
	BKPT := make(chan int, 1)
	go func() { BKPT <- int3 }()
	select {
	case sigtrap := <-BKPT:
		println(sigtrap)
	}
}
```
