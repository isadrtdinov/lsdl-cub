## Homework 2
Deadline: __18.10.2024 23:59__

### General rules
In this homework assignment, we will use a dataset consisting of images of size 224x224 from 10 classes of animals. There are 8 times more _unlabeled_ images than _labeled_ ones. Your task is to maximize the classification accuracy by pretraining a model with classical pretrainings methods (pretext tasks, similar to those discussed in the lecture). 

It is not allowed to use more modern methods (e.g. contrastive learning) and test time augmentations or similar, it is also forbidden to use any additional datasets or pre-trained models. And, of course, data labeling in any form is forbidden. If these rules are violated, the grade for the assignment will be 0. If you are not sure if a method falls under "classical" or if it can be used at all, ask @amshabalin or @isadrtdinov about it. This is better than getting a ban after submitting your homework.

In order to compete only in pre-training methods, we fix the architecture of the model. Train the standard `ResNet-18` model. You can import it like this:

```
from torchvision import models
model = models.resnet18(num_classes=10)
```

This means that the final model used for classification should have exactly this architecture, during the pre-training itself you can change it as you like.


### Competition:
[Link to competition](https://www.kaggle.com/t/1d325798097f4735bff1f058855d0829), [link to data](https://bitly.com/98K8eH).

The score is formed of three parts:
* __4 points__ are awarded to all participants who achieve accuracy >= 0.65 on public test data.
* __2 points__ are awarded to all participants who achieve accuracy >= 0.7 on public test data.
* When a participant reaches 0.7 accuracy, he/she automatically participates in the competition, for which points are awarded according to the formula below.   
  $$points = 5 \cdot \bigg(1 - \frac{\text{participant place} - 1}{\text{\\# participants}}\bigg),$$   
where the participant's place is calculated on the private test data. Thus, if 10 people passed the baseline, 1st place gets 5 points, 5th place gets 3 points, and 10th place gets 0.5 points.

* __2 points__ are given for a report on the experiments done, where you describe in detail what methods you tried and what worked and what didn't. The report is a mandatory part of the assignment. Without a report, we will get __0 points__ for this assignment. When assigning a grade for the report, its design will be taken into account; try to make the report easy to read and sumbmit it as a pdf file.

#### Hints:
* Don't use complex decoders/heads, it only slows down learning.
* Use loggers like wandb or tensorboard to track the learning process in real time, if the model is not learning, don't wait until the end, stop and look for the error.
* Start early as experiments take time.
* If the training of any model takes much longer than 6 hours, you are doing something wrong.


In order to send a submission to kaggle, you need to save the predictions for all objects in `csv` format, where the `id` column is the file name and the `class` column is the text name of the predicted class.

Example:
```
id,class
0.jpg,chicken
1.jpg,chicken
2.jpg,dog
3.jpg,cow
4.jpg,horse
5.jpg,spider
6.jpg,cow
7.jpg,spider
8.jpg,elephant
9.jpg,spider
10.jpg,sheep
```
