# GAN_performance_dlsys

This repository contains code to evaluate performance of GANs on several metrics namely:
* Inception Score
* FID Score
* GAN-Train
* GAN-Test

The following table shows these metrics calculated for GAN models with varying hyperparameters
                     
|Exp| Discriminator LR |	Generator LR |	Batch Size	| Iterations	|Discriminator-Generator Ratio|Inception Score|FID Score|GAN train Score|GAN test score
----|---------------|----------|-----|---------|---|--------|--------|----------|---------------------------------------------------------------------------------
|1     |	1.00E-02  | 1.00E-02 | 128 |	10,200 | 1 |	1.54 |	15.646 |	0.14120 |	0.11070 
|2	   | 1.00E-04   | 1.00E-06 | 128 | 5,100  | 3 | 1.55 |	22.413 |	0.13250 |	0.10610
|3     |	1.00E-03  | 1.00E-04 | 128	| 12,200 | 3 |2.277 |	11.03 |	0.11150 |	0.12580
|4     |	1.00E-04  | 1.00E-04 | 128	| 12,000 | 5 |	2.461	| 10.58	| 0.14700	| 0.13600
|5     |	1.00E-04  | 1.00E-04 | 256	| 6,000  |	5 -> 2(last 3000 iters) |	1.988 |	12.046|	0.11000	| 0.10260
|6     |	1.00E-04  | 1.00E-04 | 64	| 30000	| 5 -> 2 (last 10000 iters) |	3.12 |	9.732	| 0.12000	| 0.10000
|7     |	1.00E-04  | 1.00E-04 | 128	| 100000	| 5 -> 4 (5000 iters) -> 3 (10000 iters) -> 2 (20000 iters)" |	3.84	| 7.772 |	0.15000 |	0.10000
|8     |	1.00E-04  | 2.00E-04 | 100	| 500 epochs |	1	| |		| 0.21000	| 0.14000
