# Build documentation

Just an example of how you can document the build commands in a markdown file - and actually use them as the build commands
This example to run the commands below:

````
mask clean
mask build
````

## clean

````sh
cargo clean
````

## build

````sh
cargo build
````

## test

````sh
cargo check
````

## doc

````sh
cargo doc
````

## all

````sh
mask clean
mask build
mask test 
mask doc
````
