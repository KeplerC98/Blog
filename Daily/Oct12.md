# Markov Logic network 
Combining probability and first order logic into a single representation is a goal of AI. 
defintion: first-order knowledge base with a weight attached to each formula 

### Key words 
Markov network: joint distribution of a set of variables X = {X1 .. Xn}
first-order logic: a set of sentence/formula in first-order logic 

ground term of a formal system is a term that does not contain any free variables.

### First order logic 
a set of setences and formula
formula
* constant: objects of interest 
* variables 
* functions: mapping from objects to objects 
* predicates: relation and attribute 

Each possible grounding of a formula in the KB yields a feature in the constructed network.
ML,C contains one binary node for each possible grounding of each predicate appearing in L. The value of the node is 1 if the ground atom is true, and 0 otherwise.
ML,C contains one feature for each possible grounding of each formula Fi in L.The value of this feature is 1 if the ground formula is true, and 0 otherwise. The weight of the feature is

for MLN, 
given different sets of constants, it will produce different networks, and thesemay be of widely varying size, but all will have certain regularities in structure and parameters,

This network can represent any discrete / finite precision numeric variables. It can anwser arbitrary queries of transitional probability from F1 to F2. 

[sourcecode](http://www.cs.washington.edu/ai/alchemy)

#### Problem
assumption: closed world:): if a ground atom is not in the database, it is assumed to be false.