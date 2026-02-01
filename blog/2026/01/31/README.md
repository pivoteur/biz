# Development and Testing

So, how do I create an an enumerated type in Rust that captures a 
`future <F: Future<Output=Result<(), String>>` and a function-type 
`fn() -> Result<(), String>`.

You see how those two types are exactly the same after the future is met?

![Compiler errors](imgs/01-future.png)

Tell the Rust compiler that, though.

## Pinned Box

Okay. Got it.

![Unit tests pass](imgs/02b-tests.png)

In case anybody's interested, the type of

`async fn() -> ErrStr<()>`

is 

`Pin<Box<dyn Future<Output=ErrStr<()>> + Send>>`

![Type of async call](imgs/02a-type.png)

but only after the future is activated (that is the asynchronous call is called asynchronously and pinned)

...because that's super-obvious. 🙄

