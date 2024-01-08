# Advanced Transfer Learning
## Ratatouille Model Merging with ResNet-50

The purpose of the project is to perform a **Ratatouille Model Merging** to obtain the best model to distinguish the different **colorectal tissues and diseases**.

This technique is very efficient because it allows to train multiple Neural Networks with the same architecture on different task separately (so called *auxiliary tasks*), fine-tune the models on the final task of interest, and then merge the models into a single definitive model.

In order to find the best model to classify the colorectal tissues, I decided to use auxiliary data that may help my model as much as possible, so I will train my models on datasets related to the human body: I will initially train the model on **eye disease dataset** and **lungs disease dataset**.
After training the models on the data above, I will **fine-tune** them on the colorectal histology data, and successively merge the models.
