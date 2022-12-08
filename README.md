# Covid-19 x-rey
The 2019 novel coronavirus (COVID-19) presents several unique features. While the diagnosis is confirmed using polymerase chain reaction (PCR), infected patients with pneumonia may present on chest X-ray and computed tomography (CT) images with a pattern that is only moderately characteristic for the human eye Ng, 2020. COVID-19’s rate of transmission depends on our capacity to reliably identify infected patients with a low rate of false negatives. In addition, a low rate of false positives is required to avoid further increasing the burden on the healthcare system by unnecessarily exposing patients to quarantine if that is not required. Along with proper infection control, it is evident that timely detection of the disease would enable the implementation of all the supportive care required by patients affected by COVID-19.​

In late January, a Chinese team published a paper detailing the clinical and paraclinical features of COVID-19. They reported that patients present abnormalities in chest CT images with most having bilateral involvement Huang 2020. Bilateral multiple lobular and subsegmental areas of consolidation constitute the typical findings in chest CT images of intensive care unit (ICU) patients on admission Huang 2020. In comparison, non-ICU patients show bilateral ground-glass opacity and subsegmental areas of consolidation in their chest CT images Huang 2020. In these patients, later chest CT images display bilateral ground-glass opacity with resolved consolidation Huang 2020.​

COVID is possibly better diagnosed using radiological imaging Fang, 2020 and Ai 2020.

# This is a exercise for comparing CNN and transfer learning using ResNet model. 

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
