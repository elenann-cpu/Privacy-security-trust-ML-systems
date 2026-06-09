# Privacy, Security and Trust in Machine Learning Systems

## Overview
This project explores privacy-preserving techniques in Machine Learning and Data Analytics. The work focuses on privacy threats in ML systems, Differential Privacy (DP), Local Differential Privacy (LDP), and traditional data anonymization methods. The implementation demonstrates how privacy-enhancing technologies affect data utility and machine learning performance.

The project was developed as part of the Privacy, Security and Trust in Machine Learning Systems course.

## Project Structure
The project is divided into four main tasks:

### Task 1: Privacy Considerations and Attacks in ML
Analysis and implementation of common privacy threats:
* Reconstruction Attacks
* Model Inversion Attacks
* Membership Inference Attacks
* De-anonymization (Re-identification) Attacks
* Correlation Attacks
* Identification Attacks

Implementation of Differential Privacy mechanisms:
* Laplace Mechanism
* Exponential Mechanism
* Binary Mechanism (Randomized Response)
* Sequential Composition

Evaluation of the privacy-utility trade-off for different privacy budgets ($\varepsilon$).

### Task 2: Differentially Private Machine Learning Models
Implementation and evaluation of privacy-preserving ML models:

* **Classification**
  * Differentially Private Naive Bayes
  * Differentially Private Logistic Regression
  * *Dataset:* Bank Marketing Dataset

* **Regression**
  * Differentially Private Linear Regression
  * *Dataset:* California Housing Dataset

* **Clustering**
  * Differentially Private K-Means Clustering
  * *Dataset:* Iris Dataset

Performance is analyzed under multiple privacy budgets ($\varepsilon$).

### Task 3: Local Differential Privacy (LDP)
Implementation of LDP mechanisms:
* Randomized Response
* Direct Encoding
* Histogram Encoding
* Threshold Histogram Encoding (THE)
* Summation Histogram Encoding (SHE)

Applications include:
* Binary survey data
* Categorical attributes
* Numerical attributes

The experiments demonstrate how local privacy protection impacts estimation accuracy and data utility.

### Task 4: Data Anonymization Techniques
Implementation and analysis of classical anonymization methods:
* Suppression
* Generalization
* Perturbation
* Anatomization
* K-Anonymity
* L-Diversity
* T-Closeness

The project investigates the balance between privacy protection and data usability.


## Results
The experiments demonstrate that:
* Stronger privacy guarantees (smaller $\varepsilon$ values) introduce more noise and reduce utility.
* Larger $\varepsilon$ values improve model accuracy but provide weaker privacy protection.
* Differentially Private machine learning models can achieve performance close to non-private models when moderate privacy budgets are used.
* Local Differential Privacy successfully protects individual data while preserving useful aggregate statistics.
* Traditional anonymization techniques reduce re-identification risks but have limitations against inference attacks.

