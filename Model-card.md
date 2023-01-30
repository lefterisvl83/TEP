# Model Card

## Model Description

The model identifies anomalies in the operation of the Tennessee Eastman Process and returns 
*1* 

**Input:** Describe the inputs of your model 

**Output:** Describe the output(s) of your model

**Model Architecture:** Describe the model architecture you’ve used

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

An additional requirement for the anomaly detection algorithm is interpretability, i.e. not only being able to detect the fault, but also specifying what caused it to occur. Was it due to an incorrect flowrate set point? Or potentially a faulty valve? Thanks to this dataset, we know that the fault was caused by abnormal behaviour one of the process variables. The ability to pinpoint the offending variable is an important challenge to any anomaly detection algorithm.

It does not show what the fault is caused from. 

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
