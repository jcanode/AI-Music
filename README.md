# AI-Music

I attempted to have an AI model generate music resembling Bach pieces. 

#Method
First I downloaded Bach Chorals as midi Files

The model that I chose to use was charCNN from Andrej Karpathy (https://github.com/karpathy/char-rnn). 

However this model only works on text data. So I used midicsv (http://www.fourmilab.ch/webtools/midicsv/) to convert the midi files to CSV and text. 

I then trained the model on the data and sampled the output. 

I manually copied that into a csv file and cleaned up the data so that it fit the expected file format. 

Finally I converted it back into a midi file and played it. 


#Results
The results from the first round of testing are located in /Samples.

Clearly these are not good and are not recognizable as Bach or even music. 

Some obvious things to try are more data and more epochs as well as looking into tunning the hyperparameters.

The biggest issues seems to be that the model doesn't get a sense of rhythm and mostly just plays all the notes at once. 
