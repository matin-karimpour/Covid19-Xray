## covid-19 x-rey

This is a exercise for CNN. 
I use a small dataset for compare two models.
- First, a CNN model 
- Second, a transfer model(ResNet-V1)
### Dataset and ResNet model
You can access dataset by this [link](https://www.kaggle.com/khoongweihao/covid19-xray-dataset-train-test-sets). And the ResNet model is [here](https://tfhub.dev/google/imagenet/resnet_v1_101/classification/5).

### Result
##### CNN model 

>  since this is a small dataset the model can't fit very well and goes to underfiting. I used image generator from TensorFlow to increase the data but it didn't help.
>
> GoogleColab [link](https://colab.research.google.com/github/matinkp/covid-19-x-rey-cnn/blob/main/x_rey_covid_19.ipynb)

##### Transfer learning

> I use a resnet_v1_101 model trained by ImageNet dataset. because of our small dataset I freezed this model and just trained the last layers.
> As we expected this model works well and it have great accuracy and loss. don't forget the epochs of this model much less than other model.
>
> GoogleColab [link](https://colab.research.google.com/github/matinkp/covid-19-x-rey-cnn/blob/main/x_rey_covid_19_transfer_learning.ipynb)
