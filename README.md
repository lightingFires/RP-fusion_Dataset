# RP-fusion_Dataset
RP Dataset是论文RP-fusion:Robust Indoor Localization with RFID Fingerprints中所构建的基于RFID的双流数据集
RP Dataset包含RSSI和相位两种数据，目的是为了匹配双流网络RSSI流和相位流可以同时进行特征提取，保证同时训练的双流数据来自同时刻的RFID标签数据。这里使用4个天线采集35个标签的数据，每轮数据的大小为140。取用52轮的数据作为一次数据输入，单流输入数据为52x140的二维矩阵。RP Dataset将两种数据纵向联合，即一次输入的数据是2x52x140的三维矩阵。
RP Dataset的构成为nx2x52x140的tensor
