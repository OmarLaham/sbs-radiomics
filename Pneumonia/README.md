# Pneumonia
Kaggle Url: [https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
# Improving Steps:
Used Score: Accuracy.
|Nr.|Score|Notes / improvements|Problems / Notices
|--|--|--|--|
|1|0.7842|Initial version with Xception pretrained on imagenet. Top excluded and sigmoid activation used as final layer|Eearly stopping for unknown reason|
|2|0.8526|Increase score to 0.8526 by setting shuffle to batch_size * 10 and increase batch_size to 64|Notice that tuning batch_size can play a significant role on model score|
|3|X|Added support for VGG16, VGG19 and Xception. Also added data augmentation for train_set and tried to solve overfitting problem by adding more images to validation data sets| **Note**: Looks like we have validation problem. Must check and use quality metrics.
