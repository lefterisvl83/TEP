# Anomaly detection of the Tennessee Eastman Process (TEP)


The Tennessee Eastman Process (TEP) emerges as a standard benchmark for anomaly detection in the fields of process control and process engineering. The TEP is essentially a real industrial process that was modeled computationally in 1993 by Downs and Vogel. The data recovered from this study is consistently utilised for comparing and benchmarking algorithms, especially anomaly detection algorithms. 


The TEP is comprised of 8 chemical components in total: 4 reactants, 2 products, 1 by-product and 1 inert component. These components undergo a chemical process dominated by 5 main process units: a reactor that allows for the reaction of the gaseous feed components (A, C, D and E) into liquid products (G and H), a condenser to cool-down the gaseous product stream coming out of the reactor, a gas-liquid separator to split gas and liquid components from the cooled product stream, a centrifugal compressor to flow this gas stream back into the reactor and a stripper to handle the efficient separation of the 2 products from any unreacted feed components. There is also a purge to remove the inert (B) and the by-product (F) from the system . A schematic of the underlying industrial process is given below.

![Screenshot](TEP.png)


Based on the   Here we will attempt to construct a machine-learning anomaly detection algorithm for the TEP based on a dataset referenced in Rieth et al. (2017).



