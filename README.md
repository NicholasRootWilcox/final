# final

My final was very odd to begin with. I had to go through 3 different datasets before finally landing on my flowers one.

The CNN portion was not easy, but compared to getting the ML to "work" ("work" is being generous),
it was a far smoother ride. I had my dataset consist of purely images from 5 subfolders, I've 
had crap luck trying to use csv's and just getting anything to work well on Visual Studio Code, so 
only images was the way to go.

----------------------------------------------------

CNN Overview:

imagesize = 100 x 100, 100 epochs. Takes about 45-50 minutes to go through them all when predicting.
80 20 split. 

Did about 4 layers, last tested at around 94% (I think, don't want to wait another 50-60 minutes again).
Created a model only with convolution kernels and max pooling, messing with the second and third kernel
is what really helped. Because the accuracy was already decent, I did not touch the first layer's kernel.
But who knows, maybe that will make it even better. Once again, didn't have a whole lot of time (ML part...),
so I left it at that. Would be cool to see the difference with a (5, 5) kernel though.



----------------------------------------------------

ML Overview:

Could not get any form of ML to work on VSC. Has been a consistent problem, only Colab was the way to go 
which I could not figure out until 1AM of last night.

Want to use KNN and Random Forests, Colab doesn't have many options for ML Classification methods since it
cannot import certain packages from scikit. Want to find the optimal nearest neighbors first, and then go from
there to the actual KNN method.


ISSUES:
1.  Having trouble with fitting the shape, flattening the (3xxx something, 100, 100, 3) to (3xxx, 30000) seems
    appropriate, but it does not match up with the xTest parameters which I cannot figure out how to mend. 
    Really, dealing with shape is the big issue in this code. Once I get through that it should be fine. 
    
2.  Do I need one hot encoding? I used it in my CNN obviously, but when printing out images, It completely screws
    over the encoding (which makes sense) which obviously screws up the training. How else would I get my y list???

