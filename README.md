# Easy Rust Code Snippets

Do simple things in rust using simple code, no crates. No bloatware.

## Why does this exist in the first place?

I love the Rust programming language and its wide variety of applications, however I don't love how the language community is becoming an `npm` like flock of sheep importing crates randomly to make things that **SHOULD** be simple to work. This would be a "solve-able" problem if some crates were documented properly, however some crates have docs that could have been written by a monkey and be more readable, others have horrible examples using raw strings instead of actual files or very simple one line non-existant use cases that nobody has / will ever use. 

This repository exists to (try) end this rant about the horrible rust practices lurking on the internet (and as a personal notepad if I ever need to use these kind of snippets for personal code).

## Rust Snippets

### Get current user

**The simple way**
``` rust
use std::env;

// ...

let key = "USER";

let user: String = match env::var(key) {
    Ok(val) => val,
    Err(e) => e.to_string(), // Process error as you like, save it to string or panic!
};

println!("{}", user);
```

You save:
 - Around 10.5 ~ 22Kb
 - From 3 - 5 dependencies
 
---

#### Snippet Template 
### Title

**The simple way**
``` rust
// rust code here
```

You save:
 - Around comp1 ~ comp2
 - From comp1 - comp2 dependencies
