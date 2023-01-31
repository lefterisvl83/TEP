# Model Card

## Model Description

The model monitors working conditions and identifies anomalies in the operation of the Tennessee Eastman Process. 

**Input:** 

Process variables such as flowrates, pressures, temperatures, levels, mole fractions, compressor power outputs, valve positions and the reaction agitator speed.


**Output:** 

The model returns an integer ranging from 0 to 20 each associated with a fault-free or faulty operation. Specifically, the output is 
** zero if the processs is under nominal working operation,
** a nonzero integer ranging from 1 to 20 each associated with the faul class detected.

**Model Architecture:** 

XgBoost classifier with n_estimators and max_depth hyperparamters.

## Performance

We use the F1 micro score as performance metric. F1 score is suitable for evaluating in parallel high precision and model's high recall. In fact, we need to trade off precision for recall, and hence, F1 score is the a good choice. Since we have a multiclass classification problem, where we need to predict among 21 different working conditions, micro F1 score is a suitable metric.

**Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. **

## Limitations

An additional requirement for the anomaly detection algorithm is interpretability, i.e. not only being able to detect the fault, but also specifying what caused it to occur. Was it due to an incorrect flowrate set point? Or potentially a faulty valve? Unfortunately, the model as configured in this project is not able to address this task. This limitation represents a challenging subject for future work.


## Trade-offs

Since we deal with output-sensitive predictions, the underlying model needs to have high recall. Thus, the main trade-off considered in the model is between high precision and the model's high recall.

