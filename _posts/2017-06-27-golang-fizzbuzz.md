---
published: true
---

```
package main

import (
	"fmt"
)

func main() {
	for i := 1; i <=100; i++ {
		fmt.Println(fizzBuzz(i))
	}
}

func fizzBuzz(i int) interface{} {
	result := ""
	if i % 3 == 0 { result += "Fizz" } 
	if i % 5 == 0 { result += "Buzz" }
	if (len(result) == 0) { return i }
	return result
}
```
