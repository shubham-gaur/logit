# Test

```go
package main

import "github.com/shubham-gaur/logit"

func main() {
    app := "Test"
    logit.Init(&app)
    logit.Info.Println(logit.GetCurrentFunctionName() + "Example 1")
    logit.Info.Println("hello world")
    logit.Warn.Println("hello world")
    logit.Err.Println("hello world")
    logit.Debug.Println("hello world")
    logit.Critical.Println("hello world")
}
```
