# WTF Go

While learning about golang, I stubled upon many things that don't make much sense compared to other languages. 
The language has IMO high WTF factor. 
I want to list those WTFs so it either reminds me to get understanding of it or to serve as a strawman so I don't get tempted to touch the language. 

## Missing access modifiers

`type memberInfo struct {` means private access (only accessible within single package)

`type MemberInfo struct {` means public access (accessible from other packages)

Where are access modifiers?!

## Switch-case Indent

Is this a proper indentation for switch case? Why reinvent something that works... The outcome is definitelly worse.

```go
switch i {
case 1:
    fmt.Println("one")
case 2:
    fmt.Println("two")
case 3:
    fmt.Println("three")
}
```
