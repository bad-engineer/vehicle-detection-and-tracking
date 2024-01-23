# Vehicle Detection and Tracking in Aerial Videos

In this project, I used the VisDrone 2019 dataset to train a Yolov5 model for detecting cars. I also implemented object tracking using the DeepSort and StrongSort algorithms and performed a quantitative comparison of both. Finally, I implemented Yolo + DeepSort on the OpenCV AI Kit (AI Camera) interfaced with a Raspberry Pi to complete an edge AI setup for aerial traffic monitoring. I also collected my own test dataset using a DJI Phantom 4 Drone and demonstrated tracking results on it.

## Dataset Preprocessing

To reduce computational complexity, I cut down the dataset and filtered the annotations to extract just one out of the eleven classes of traffic objects present in the VisDrone dataset. 

## Results: Object Detection

![0000009](https://github.com/bad-engineer/vehicle-detection-and-tracking/assets/74527254/cb7c393b-419d-4771-ac68-1005310400e7)

## Results: Object Tracking with DeepSort (Occlusion Experiment)

I positioned the drone so that part of the road was hidden by a tree. DeepSort successfully tracked the car driven behind the tree and retained its ID.

![Occlusion- Deepsort](https://github.com/bad-engineer/vehicle-detection-and-tracking/assets/74527254/c36a716c-0d9c-4ccd-8705-a2318f8a3223)

## Results: Object Tracking with StrongSort (Occlusion Experiment)

I performed the same occlusion experiment using StrongSort, and the algorithm was able to redetect the occluded car:

![Occlusion-StrongSort](https://github.com/bad-engineer/vehicle-detection-and-tracking/assets/74527254/62e3e352-7e00-457b-b727-23e3e5af3290)

# References, Technical Calculations, and documentation 

For further details, real-time demonstration videos, technical calculations, and documentation, please see my thesis and relevant media at the following link:

- [Technical Documentation](https://drive.google.com/drive/folders/1E2AyGFjocogkloZulAZr_mlnPOpUrCxh?usp=sharing)
  




