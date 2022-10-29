# Accumulators
#SICP #Programming 

+ context-preserving (preserve context lost in natural recursion)
+ result-so-far accumulators (used to make function tail recursive by removing pending operations)
+ worklist accumulators (used to make function [[Tail recursion|tail recursive]] by removing pending operations on recursive calls)

When adding a accumulator to a [[Mutually recursive data|mutually recursive type of data]], you add it to all of its functions. 

In [[Mutually recursive data|mutually recursive functions]], usually only one of the functions provide NEW values for each accumulator.