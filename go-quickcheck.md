## Explore quickcheck/hypothisis libraries for go
Quickcheck/Hyptothis provides a property based testing framework, it tries to "fuzz" inputs to find inputs that break the required properties.
I've explored hyptohsis in python before, but have not tried anything like this for go.

Most recently i came across a very interesting application of this property based testing, mentioned in the ["Using lightweight formal methods to validate s3 storage"](https://www.amazon.science/publications/using-lightweight-formal-methods-to-validate-a-key-value-storage-node-in-amazon-s3) paper
and i want to be able to replicate a similar framework. 

### Milestones

#### M1: Find a prod like example usage for a go check library
* Find a suitable propety based testing library -- https://github.com/leanovate/gopter is a good start
* Explore the api of the library
* Use the library for some example use cases
* Find a real life example to use this library.


#### M2: Explore building a fuzzer that is dependency aware
* How to build a custom fuzzer/ validatior
* Encode an operation as parts of a validatior
* Include dependcies as parts of a vlaidator.

#### M3: Explore the ideas from the s3 paper
* Try to implement examples similar to the ones mentioned in the paper ( this requires more breakdown)


### Useful links
* https://hypothesis.works/articles/quickcheck-in-every-language/
* https://github.com/leanovate/gopter/tree/master
* https://hypothesis.readthedocs.io/en/latest/
* https://www.amazon.science/publications/using-lightweight-formal-methods-to-validate-a-key-value-storage-node-in-amazon-s3
