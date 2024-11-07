***GAN  Generative Adversial Network*** :

 its a type of neural network that used in machine learning to generate new data that looks similar to a given data.
 
 it consists of two main components:
 
***1 Generator***: its a neural network takes random noise(vector of random numbers) as input and tries to generate data that looks realistic enough.

**2 Discriminator**: its also a neural network , it takes both real data from the dataset and fake data from the generator as input and tries to do a binary classification, if it as real or fake.

These two networks are compeeting to win if we could say, at some point, the generator gets so good at creating realistic data that the discriminator wont descriminate .

applications of GAN :
       
                      -Image to Image translation

                      -Image to Text / Text to Image translation
                      
                      -Deep Fake


***GANs Don’t Work Well for Text ?***

GANs perform well with continuous data, like images, because the generator can create smooth, flowing values ( for example : pixel intensities), but when it comes to text and words; it cant perform good results beacus the input is **discrete valuse** , and this causes two main issues:

**1.Hard to Learn with Words:**

GANs learn by making smooth and continious changes, but with text, it has to pick exact and precise words, which prevents smooth transitions

**2.Sentences Have Order and Meaning:**

 GANs aren’t designed to understand grammar or how sentences should flow so its struggle with text, becuz the order of words is important: sentences need to follow a structure to make sense.

***THATS WHY*** >>>   Researchers suggest various architectures to handle text generation with GANs, including models that combine **RNNs** or **LSTMs** with adversarial training, enabling to improv coherence and structure in the faked text.

one such intersting architecture is **SeqGAN**

***what's a SeqGAN  ?***

SeqGAN (**Sequence GAN**) is a special type of GAN that was created to deal with the challenges of text, it adapts the GAN structure so it can generate text sequences, handling the unique structure and rules of language better than a standard GAN could.
