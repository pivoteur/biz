# Development

HWÆT, pivoteurs, and well-met!

I've been fighting the compiler on types.

What's the return-type of a Trait that has functions that return Futures? 

![Traits returning Futures](imgs/01a-types.png)

Although allowed by the Rust Language Spec, implementations can be tricky.

![Tests pass](imgs/01b-tests.png)

I figured out the return-type. It took 2 days. *sigh*
