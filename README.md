<h1 align="center">Event-Based Crossing Dataset (EBCD)</h1>



<p align="center">
  <img src="https://github.com/user-attachments/assets/56aaab7a-6471-47ec-b400-c9a3c26b6673" alt="bbox_comparison_github" />
</p>


# Citation
Please consider citing our paper:
------------------------------------------------------------------
@ARTICLE{mule2025EBCD,
  author={Mulé, Joey and Challagundla, Dhandeep and Saini, Rachit and Islam, Riadul},
  journal={IEEE Data Descriptions}, 
  title={Descriptor: Event-Based Crossing Dataset (EBCD)}, 
  year={2025},
  volume={},
  number={},
  pages={1-11},
  keywords={Event detection;Vehicle dynamics;Pedestrians;Real-time systems;Computer architecture;Cameras;Voltage control;Neuromorphics;Convolutional neural networks;Computational efficiency;Pedestrian detection;Vehicle detection;dynamic vision sensing (DVS);sparse vision;convolutional neural network (CNN);Pedestrian crossing dataset},
  doi={10.1109/IEEEDATA.2025.3561760}}
------------------------------------------------------------------

<p align="center">
  <b>Example setup for Inferencing using sample Threshold ↓</b>
</p>

<h1 align="center">Inferencing with MobileNet-v1</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/a98e20ad-80f7-4435-b0a0-7128e95459b4" alt="bbox_comparison_github" />
</p>

# First steps (setting up tensorflow SSD)
```
git clone https://github.com/tensorflow/models.git
cd models/research
protoc -I=./ --python_out=./ ./object_detection/protos/*.proto
pip install .

or if 'pip install .' doesnt work
cd object_detection/packages/tf2 (or tf1 depending on your tensorflow version)
pip install .
```

### MobileNet_Thresh_20(.zip)/
### │── MobileNet_T20/            → Main MobileNet model files
### │── sample_all_thresholds/    → Sample data for all thresholds
### │── threshold_20/             → Configuration and training files for threshold 20
### │── Run_MobileNet.ipynb       → Jupyter Notebook to run MobileNet inference

# Please go through 'Run_MobileNet.ipynb'

### If you desire any other weights/configuration for other thresholds or other models labeled in our paper, please reach out:
```
[Joey Mulé]
jmule2@umbc.edu

[Dr. Riadul Islam]
riaduli@umbc.edu
```
