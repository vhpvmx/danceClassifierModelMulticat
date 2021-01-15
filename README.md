# danceClassifierModelMulticat

In notebook "danceClassifierModelMulticat", I explain the development of a deep learning model that identify the kind of dance based on an image. As a result the new model can identify one or more dance styles in the same picture.

I use around 450 images. It is possible to get good results with few images applying diferent techniques as Data Augmentation and Transfer Learning. For Data Augmentation i applied a technique call presizing from fastai, which apply these steps:

Resize images to relatively "large" dimensions—that is, dimensions significantly larger than the target training dimensions.
Compose all of the common augmentation operations (rotation, zoom, resize, etc) into one, and perform the combined operation on the GPU only once at the end of processing, rather than performing the operations individually and interpolating multiple times.
For Transfer Learning i used the model "resnet18" and "resnet50", both models were pre-trained on ImageNet (ImageNet contains over 1.3 million images of various sizes around 500 pixels across, in 1,000 categories, the model took a few days to train)

You can interact with the model using this app: https://dancereco.herokuapp.com/
You can see the deployment process in heroku here: https://github.com/vhpvmx/dancereco
