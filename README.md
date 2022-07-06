# MultiTaskNetworkAnomalyDetection

A multi-task deep neural network (MT-DNN) to perform network anomaly detection task, VPN (Tor) traffic recognition task, and traffic classification task, simultaneously.


## Datasets

### CICIDS2017
The CICIDS2017 is a state-of-the-art network intrusion detection dataset, which is generated and captured by the Canadian Institute for Cybersecurity. This dataset provides five days labeled real-world network traffic, including benign and attacks traffic in the PCAP format.

### ISCXVPN2016
The ISCXVPN2016 dataset is established by Draper-Gil et al. to detect VPN traffic and to characterize encrypted traffic. There are seven categories of applications, Browsing, Chat, Streaming, Mail, VoIP, P2P, and File Transfer, in this dataset. For each application, its regular session and VPN session traffic are stored in the PCAP format, respectively.

### ISCXTor2016
The ISCXTor2016 is generated to detect Tor traffic. Different from the ISCXVPN2016, the seven categories applications traffic in the ISCXTor2016 are encapsulated in Tor forms.

## Experminet Scenarios

### Scenario A
The first experiment focuses on the following three tasks: network anomaly detection task, VPN traffic recognition task, and traffic classification task. In this scenario, we used the CICIDS2017 and ISCXVPN2016 datasets to evaluate the performance.

### Scenario B
The second experiment focuses on the following three tasks: network anomaly detection task, Tor traffic recogni- tion task, and traffic classification task. The CICIDS2017 and ISCXTor2016 datasets are combined to evaluate the MT-DNN.

## Steps to run MT-DNN
1. Download the three datasets from the link [here](https://www.unb.ca/cic/datasets)
2. Use [CICFlowMeter](https://github.com/ahlashkari/CICFlowMeter) appliation to generate required features for the application in CSV format from PCAP format
3. Run above "multitasknn.ipynb" notebook to train and test the MT-DNN with the above data
