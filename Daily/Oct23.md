# QA

### keywords 
query： keywords that system should look at and search for 

### IR
Anwser type classification: determine answer type. Word in a question can give extra information: question headword & anwser type word. 

Query formulation: rephrase the question: rephrase the question that look like substring of declarative answers 

passage retrieval: extract potential answer of the passage 
    passages are ranked based on named entities, keywords proximity 

answer processing: pattern extraction 


### Knowledge based QA
have a databased relations e.g. infoboxes that has structued tables associated with wiki's articles 

The supervised approach can be extended to deal with more complex questions that are not just about single relations.
argmax(lx:state(x) ^ borders(x;texas);lx:size(x))

most methods make some use of web text, either via semi-supervised methods like distant supervision or unsupervised methods like **open information extraction**, both introduced in Chapter 20