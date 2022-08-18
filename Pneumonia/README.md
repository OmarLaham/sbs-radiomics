# Pneumonia
Kaggle Url: [https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
# Improving Steps:
Used Score: Accuracy.
|Nr.|Score|Notes / improvements|Problems
|--|--|--|--|
|1|0.7842|Initial version with Xception pretrained on imagenet. Top excluded and sigmoid activation used as final layer|Eearly stopping for unknown reason|
|2|0.8526|Increase score to 0.8526 by setting shuffle to batch_size * 10 and increase batch_size to 64|Notice that tuning batch_size can play a significant role on model score|
