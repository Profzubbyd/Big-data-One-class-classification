# One-Class classification with PSOAANN for Credit Card Fraud Detection

## I. Introduction

The issuance of millions of credit cards annually has led to an increase in credit card usage. This has, unfortunately, also increased the risk of credit card fraud. Financial institutions employ advanced machine learning techniques and big data technologies to detect and prevent fraudulent activities. Imbalanced data poses a challenge, and methods like SMOTE have been used to address it. This report presents the implementation and enhancement of a parallelized hybrid architecture that combines Particle Swarm Optimization (PSO) with Auto-Associative Neural Network (AANN) to improve credit card fraud detection.

## II. Related Work

Several works in literature have explored different approaches to credit card fraud detection. These include balanced random forest, streaming analytics with Kafka and Hidden Markov Model (HMM), federated fraud detection, genetic algorithms for feature selection, and frameworks using big data technologies like Hadoop and Spark. This report compares these papers, highlighting their methods and contributions.

## III. Proposed Method

Building upon the PSOAANN architecture, our implementation involves a parallelized hybrid model using PSO and AANN for one-class classification. The PSOAANN algorithm consists of training and testing phases, combining unsupervised and supervised learning. We propose enhancements such as parallelizing the entire algorithm, increasing swarm size in PSO, and changing the normalization method.

## IV. Dataset

Experiments were conducted using the "ccFraud" dataset with ten million samples. The dataset, a big data problem, presented challenges due to high volume, velocity, and class imbalance. The PSOAANN model was trained with legitimate transactions (negative samples) only, and distributed processing using Apache Spark was employed.

## V. Experiments

The experimental setup utilized a standalone Spark cluster, and the PSOAANN model was trained for 10 runs. Results show a classification rate ranging from 40% to 93%, with a mean MSE indicating better results than the research paper. Challenges in achieving higher accuracy are discussed.

<p align="center">
  <img width="800" alt="image" src="https://github.com/Profzubbyd/Big-data-One-class-classification/assets/46527701/4bd9516b-83b7-4069-bbdf-cb47d11eba5a">
</p>

<p align="center">
  Figure 1: Mean MSE Convergence Plot
</p>


## VI. Conclusion

The project presents improvements to the hybrid architecture, achieving an average true classification rate of 71.88% for credit card fraud detection. Future work includes parallelizing the PSO algorithm and exploring other bio-inspired algorithms.

## References

1. P. K. Chan, W. Fan, A. Prodromidis, and S. J. Stolfo, “Distributed data mining in credit card fraud  detection,” IEEE Intelligent Systems, vol. 14,pp. 67–74, 1999.

2.	S. Bhattacharyya, S. Jha, K. Tharakunnel, and J. C. Westland, “Datamining for credit card fraud:  A comparative study,” Decision Support Systems, vol. 50, no. 3, pp. 602–613, 2011.

3.	Kamaruddin, S., & Ravi, V. (2016). Credit card fraud detection using Big Data Analytics. Proceedings of the International Conference on Informatics and Analytics. https://doi.org/10.1145/2980258.2980319

4.	[Melo-Acosta, G. E., Duitama-Munoz, F., & Arias-Londono, J. D. (2017). Fraud detection in big data using supervised and semi-supervised Learning Techniques. 2017 IEEE Colombian Conference on Communications and Computing (COLCOM).](https://doi.org/10.1109/colcomcon.2017.8088206)

5.	[Rajeshwari U, & Babu, B. S. (2016). Real-time credit card fraud detection using streaming analytics. 2016 2nd International Conference on Applied and Theoretical Computing and Communication Technology (ICATccT).](https://doi.org/10.1109/icatcct.2016.7912039)

6.	[Yang, W., Zhang, Y., Ye, K., Li, L., Xu, CZ. (2019). FFD: A Federated Learning Based Method for Credit Card Fraud Detection. In: Chen, K., Seshadri, S., Zhang, LJ. (eds) Big Data – BigData 2019. BIGDATA 2019. Lecture Notes in Computer Science(), vol 11514. Springer, Cham.](https://doi.org/10.1007/978-3-030-23551-2_2)

7.	[Ileberi, E., Sun, Y. & Wang, Z. A machine learning based credit card fraud detection using the GA algorithm for feature selection. J Big Data 9, 24 (2022).](https://doi.org/10.1186/s40537-022-00573-8)

8.	[Dai, Y., Yan, J., Tang, X., Zhao, H., & Guo, M. (2016). Online credit card fraud detection: A hybrid framework with Big Data Technologies. 2016 IEEE Trustcom/BigDataSE/ISPA.](https://doi.org/10.1109/trustcom.2016.0253)

9.	[Carcillo, F., Dal Pozzolo, A., Le Borgne, Y.-A., Caelen, O., Mazzer, Y., & Bontempi, G. (2018). Scarff : A scalable framework for streaming credit card fraud detection with Spark.Information Fusion, 41, 182–194.](https://doi.org/10.1016/j.inffus.2017.09.005)
