# FourierNet
This Fourier Net repo looks at answering the question: Can the introduction of the Fourier series principle into a neural net improves its "universal approximator" 
functionality.
Neural Networks are known to be be "universal approximator". The universal approximation theorem (1996, Hornik and al) even establishes that you can approximative
any continuous function within a specific range with even a single hidden layer neural net. 
In practice though, using a single layer neural net, even if you add up a great number of neurons to it will not get you really far as it is going to be difficult 
to have the optimization algorithm converge. 
This repo explores one way of improving this method by using another famous function approximation theory: Fourier series (or their extension to non periodic functions
with the Fourier transform). 
We are going to see if we can improve a simple (even simplistic) net performance without making it deeper, by using series of sines and cosines as in a Fourier series, 
and actually implementing a Fourier series generator with the powerful neural net libraries around (or quasi Fourier as we 
add activation functions that are not in the Fourier principle) .

We use Pytorch for its great flexibility in the net architecture. 

Remark: We are not trying here to use Neural Net in the way they are usually used for, ie, forecasting. We simply use and explore what we can 
do around their approximation functionality but the datasets we are going to use are theoretical, or random, and there is nothing to predict from it
