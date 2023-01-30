# Model Card

## Model Description

The model monitors working conditions and identifies anomalies in the operation of the Tennessee Eastman Process. 

**Input:** 

Process variables such as flowrates, pressures, temperatures, levels, mole fractions, compressor power outputs, valve positions and the reaction agitator speed.


**Output:** 

The model returns an integer ranging from 0 to 20 each associated with a fault-free or faulty operation. Specifically, the output is 
**1** zero if the processs is under nominal working operation,
**2** a nonzero integer ranging from 1 to 20 each associated with the faul class detected.

**Model Architecture:** 



## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

An additional requirement for the anomaly detection algorithm is interpretability, i.e. not only being able to detect the fault, but also specifying what caused it to occur. Was it due to an incorrect flowrate set point? Or potentially a faulty valve? Thanks to this dataset, we know that the fault was caused by abnormal behaviour one of the process variables. The ability to pinpoint the offending variable is an important challenge to any anomaly detection algorithm.

It does not show what the fault is caused from. 

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
