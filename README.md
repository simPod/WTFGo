# WTF Go

While learning about golang, I stubled upon many things that don't make much sense compared to other languages. 
The language has IMO high WTF factor. 
I want to list those WTFs so it either reminds me to get understanding of it or to serve as a strawman so I don't get tempted to touch the language.

![#crymeariver](https://raw.githubusercontent.com/simPod/WTFGo/master/img/crymeariver.jpeg) 

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

Seems like it's the reason why it can't be collapsed

![Dreaming about collapsing switch statement](https://raw.githubusercontent.com/simPod/WTFGo/master/img/dreaming-about-collapsing-swtich-statement.png)

