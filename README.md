# House Price Prediction 
### Train a CNN for regression prediction with Keras , **WITH INPUT IMAGES**
<br/>

# Description :
+ training a CNN to predict house prices from image data 
+ output of the network is a single continuous value , and its not categorical. 
+ Training the model with a continuous value prediction loss function such as mean squared error, mean absolute error



##  dataset  :
A total of 535 houses are included in the dataset, therefore there are 535 x 4 = 2,140 total images in the dataset. <br/>


+ clone dataset : <br/>
```
$ git clone https://github.com/emanhamed/Houses-dataset
```

This house prices dataset includes four images associated with each house:

+ Bedroom
+ Bathroom
+ Kitchen
+ Frontal view of the house

how are we going to use these images to train our CNN?
> # Important note :
> ## we should create a montage that combines each four images into a single image and then pass the montage through the CNN

<p float="center">
    <img src  = "assets\4image.JPG" width=350 /> 
</p>
in this order : <br/>
1- The bathroom image in the top-left <br/>
2- The bedroom image in the top-right <br/>
3- The frontal view in the bottom-right <br/>
4- The kitchen in the bottom-left <br/>
<br/>

this method Enables the CNN to learn different filters from all house photos at once and will not “confusing” the CNN with different images but with identical target values.


