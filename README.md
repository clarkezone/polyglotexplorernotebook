# Polyglot Explorer's Notebook
The last 15 years or so of my professional life have been defined in no small measure by my early adoption of  the C# programming language when it was it was still in beta back in 2001.  After so many years focused more or less on a single language, it feels like about time to embark on a new era of learning.  This itch began over the 2016 holiday period where I started experimenting with Go as a lightweight backend for an Android app I was working on at the time. That has morphed into a stronger desire to catch up on modern trends in language and runtime design.  As such I have selected five relatively young languages to study that are interesting to me in different ways.  This project will be a living catalog of my journey of discovery and what I learn along the way.

|   | Go  | Kotlin | Rust | Dart | Swift |
|---|---|---|---|---|---|
|Site|https://golang.org/|https://kotlinlang.org/|https://www.rust-lang.org/en-US/|https://www.dartlang.org/|https://swift.org/|
|Twitter|@golang|@kotlin|@rustlang|@dart_lang|@swiftlang|
|Blog|https://blog.golang.org/|https://blog.jetbrains.com/kotlin/|https://blog.rust-lang.org/|https://news.dartlang.org/|https://swift.org/blog/|
|Podcast|?|?|http://www.newrustacean.com/|?|?|
|V1.0 stable released|March 2012|February 15, 2016|May 15, 2015|?|September 9, 2014|
|Canonical Book|The Go Programming Language by Alan A. A. Donovan,‎ Brian W. Kernighan https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing/dp/0134190440/ref=sr_1_1?ie=UTF8&qid=1514570808&sr=8-1&keywords=go+programming+language+books|Kotlin in Action 1st Edition by Dmitry Jemerov, Svetlana Isakova https://www.amazon.com/Kotlin-Action-Dmitry-Jemerov/dp/1617293296/ref=sr_1_1?s=books&ie=UTF8&qid=1514571373&sr=1-1&keywords=kotlin+in+action|"the book" https://doc.rust-lang.org/book/second-edition/||The Swift Programming Language https://swift.org/documentation/TheSwiftProgrammingLanguage(Swift4.0.3).epub|
|The Hook|Fast, lightweight, platform independent web server.  Ideal for micro-services, REST, etc.  Fun to use, simple, functional. ||||
||||||

## Tools
### Build
Rust:
```
cargo build
```

## Hello world
Go:
```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, 世界")
}
```
Rust:
```rust
fn main()
{
    print!("Hello 世界");
}
```

## Optional Values
Swift:
```swift
let test : String? = "cool"

if let valid = test {
    print(valid)
} else {
    print("no value")
}
```

Rust:
```rust
fn main() {
    let _my_optional = Some("hello");
    let _my_optional2 : Option<String> = Some(String::from("hello"));

    match _my_optional {
        Some(x) => println!("Result: {}", x),        
        None    => println!("no string"),
    }
}
```