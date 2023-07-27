# RP-fusion_Dataset
RP Dataset是论文RP-fusion:Robust Indoor Localization with RFID Fingerprints中所构建的基于RFID的双流数据集。
RP Dataset包含RSSI和相位两种数据，目的是为了匹配双流网络RSSI流和相位流可以同时进行特征提取，保证同时训练的双流数据来自同时刻的RFID标签数据。这里使用4个天线采集35个标签的数据，每轮数据的大小为140。取用52轮的数据作为一次数据输入，单流输入数据为52x140的二维矩阵。RP Dataset将两种数据纵向联合，即一次输入的数据是2x52x140的三维矩阵。
RP Dataset的构成为nx2x52x140的tensor。<br>
The RP Dataset is a two-stream dataset constructed in the paper "RP-fusion: Robust Indoor Localization with RFID Fingerprints". It includes two types of data, namely RSSI (Received Signal Strength Indicator) and phase data. The purpose of creating this dataset is to enable the simultaneous feature extraction from both the RSSI and phase data in the two-stream network, ensuring that the two-stream data used for training comes from the same time-stamped RFID tag data.
In this dataset, data is collected using four antennas to capture information from 35 RFID tags. Each round of data collection consists of 140 data points. For one complete data input, 52 rounds of data are used, resulting in a single-stream input data of size 52x140 as a two-dimensional matrix. The RP Dataset vertically combines these two types of data, resulting in a three-dimensional matrix of size 2x52x140 for one complete input.
Overall, the RP Dataset is represented as a tensor of size nx2x52x140, where 'n' represents the total number of samples or instances in the dataset.
