# Neural Translation of Musical Style
This is a model that can learn to perform sheet music like human does, which can pass "musical Turing tests". The key for just playing a note and human-performed music is a global structure and dependency of music. 
This is why we have LSTM to solve it. RNN: of course it has vanishing gradient problem. 


### architecture: GenreNet
Sheet music -> birectional LSTM -> linear layer ->dyanmics 
* bidirectional LSTM: "can look ahead" 
* linear layer: activation function 

StyleNet: rendition model that can play variety of styles 
    Interpretation layer: converts musical input into own representation and then go through bidirectional LSTM

### implementaiton details 

# thoughts 
One of our experiment as previous encoder-decoder neural network is this "musical turing tests". We produce sounds and let them pass "sound turing test". 

This model is less random than other implementation that I read. I think it is because the music itself is more structured(by sheet music, for example) and the model does not have so many factors to influence the fluency of music.  

If I really wanted to implement a model that 
Still it is pretty good to read about their source code on 
[github](https://github.com/imalikshake/StyleNet)