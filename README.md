### date of creation: May, 2023

## Problem:
To develop an algorithm for detecting various objects in images. The following classes are taken: car, plate, person.
What is it for? Keep count of the number of incoming cars with further calculation of financial metrics, as well as track the work activities of car mechanics.

## Dataset:
The dataset is collected from a photo stream from a videcam installed in a car service center. Photos should be collected at different times of the day, maintaining an approximate balance between classes. Taking into account augmentation, as a result, 2500 photographs were collected and labeled (2042 - train, 458 - valid). Approximate class balance - _(car:person:plate - 1:1:0,7)_. Link to dataset: [dataset here](https://drive.google.com/file/d/1h9YXqBQPVcNbE2OexByA6guXohmZryO4/view?usp=drive_link).

## Model:
To implement the task, we use the pre-trained _Yolov7_ model, modified for our three classes.

## Files:
- training_model_yolov7 - model training on 50 epochs                                                                                                                                                               
- pt_to_onnx - to convert the best.pt model to best.onnx                                                                                                                                                            
- testing - testing the model

## Results:
The model training accuracy is _0.9535_. Various graphs, as well as testing models on unlabeled data, are located in folder named _"results"_.
