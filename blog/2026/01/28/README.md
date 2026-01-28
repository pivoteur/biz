# Testing-suites

## Integration testing

💥💥💥ANNOUNCEMENT💥💥💥

`itr`

![Integration test-suite: itr](imgs/01-itr.png)

Separate integration test-suite for Rust dapps that executes `cargo build` in 
all subdirectories of `<dir>`.

Rust unit testing integrates integration testing and doesn't have functional 
tests.

I need all three kinds: unit, functional, integration.

## Functional testing

Furthermore, `itr` allows me to run integration tests separately from unit 
tests (and I have a separate ad-hoc functional test-suite – called `main()` 
(eheh 😅) – at module- and library-levels).

![ad-hoc Functional testing](imgs/02-fn.png)

These separate testing-suites will allow me to deliver to production more 
rapidly.

## Code-coverage

Rounding out testing, I've added new features and reports.

![tarpaulin code-coverage](imgs/03d-tarpaulin.png)

* tarpaulin (https://github.com/xd009642/tarpaulin) for code-coverage (now at 44.38% code-coverage)

![Test suite-progress](imgs/03c-tests.png)

* I'm now charting test-suite progress 

![Protocol unit-tests](imgs/03a-protocol-unit-tests.png)
![Book unit-tests](imgs/03b-book-unit-tests.png)

