# WTF Go

While learning about golang, I stubled upon many things that don't make much sense compared to other languages. 
The language has IMO high WTF factor. 
I want to list those WTFs so it either reminds me to get understanding of it or to serve as a strawman so I don't get tempted to touch the language. 

## Missing access modifiers

`type memberInfo struct {` means private access (only accessible within single package)

`type MemberInfo struct {` means public access (accessible from other packages)

Where are access modifiers?!
