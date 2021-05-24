# Spark Weather Project


## Introduction
This repository contains data files for an Apache Spark project that was run on AWS EMR. This project was done for a Computer Architecture class at Johns Hopkins University. **Weather-Analysis.ipynb** was run on a AWS EMR cluster. The training data is taken from AWS S3 and result is stored back into S3. Then the result is read back in by **Data Plot.ipynb** and data is plotted.

## File Info
### **Weather-Analysis.ipynb**
- Trains and tests the models using data files in S3
- Saves the result back to S3

### **Data Plot.ipynb**
- Takes the result stored by **Weather-Analysis.ipynb** and plots the differences

### **sf.csv**
- Data used to train the models

### **sf_test.csv**
- Result outputted from **Weather-Analysis.ipynb**


## Technology Used
* PySpark
* AWS EMR, S3, EC2
* Jupyter Notebook
* pandas, numpy, matplotlib

## Steps To Reproduce
1. Create an AWS EMR cluster with access to Jupyter Hub and Spark. These options are visible after selecting advanced setup.
2. SSH into the master node.
3. Install the necessary libraries using pip.
4. Create a SSH tunnel to the master node using the links provided.
5. Store the CSV files in AWS S3.
6. Modify the S3 location in Section 9 of **Weather-Analysis.ipynb** and **Data Plot.ipynb**
7. Run **Weather-Analysis.ipynb**. Result should be stored in S3.
8. Run **Data Plot.ipynb**.


## Links
- [Data Files](https://drive.google.com/drive/folders/10vxgCxs-b4itfHWEpHjnIIOClGNwINqZ?usp=sharing)
- [Class Demo](#)
- [Set Up an SSH Tunnel Part 1](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-ssh-tunnel.html)
- [Set Up an SSH Tunnel Part 2](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-connect-master-node-proxy.html)