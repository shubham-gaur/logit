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

## Output

```bash
∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙
[sgaur@fedora logit-test]$ 
 🔆 go run main.go 
🔵 Test | INFO | main.main                | Example 1
🔵 Test | INFO | hello world
🟠 Test | WARN | hello world
❌ Test | ERR  | hello world
🟣 Test | DBUG | 2022/11/06 00:24:25 main.go:12: hello world
🔴 Test | CRIT | 2022/11/06 00:24:25 /home/sgaur/logit-test/main.go:13: hello world
∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙∙
```
