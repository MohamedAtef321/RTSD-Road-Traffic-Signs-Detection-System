<div align="center">

<p>
    <a href="https://github.com/MohamedAtef321/RTSD-Road-Traffic-Signs-Detection-System" target="_blank">
    <img width="100%" src="images\RTSD_banner_round.png"></a>
</p>

# RTSD (Road Traffic Signs Detection) System
RTSD System can detect traffic signs 🚩 along the road. \
This project aims to enable self-driving cars 🚗 to see and interact with the road signs.

</div>

> 🙋‍♂️ **Who are we ?** : 
> - We are a team from Egypt studied at [Faculty of Engineering](https://engfac.mans.edu.eg/), [Electronics and Communications Department](https://www.facebook.com/people/%D8%A7%D9%84%D8%B5%D9%81%D8%AD%D8%A9-%D8%A7%D9%84%D8%B1%D8%B3%D9%85%D9%8A%D8%A9-%D9%84%D9%82%D8%B3%D9%85-%D9%87%D9%86%D8%AF%D8%B3%D8%A9-%D8%A7%D9%84%D8%A7%D9%84%D9%83%D8%AA%D8%B1%D9%88%D9%86%D9%8A%D8%A7%D8%AA-%D9%88-%D8%A7%D9%84%D8%A7%D8%AA%D8%B5%D8%A7%D9%84%D8%A7%D8%AA-%D8%AC%D8%A7%D9%85%D8%B9%D8%A9-%D8%A7%D9%84%D9%85%D9%86%D8%B5%D9%88%D8%B1%D8%A9/100057482558089/) in [Mansoura University](https://www.mans.edu.eg/en).
>
> - These features were created to be used for our graduation project 🎓 (RTSD System) to make a system that can detect Roads Traffic Signs in real-time. 
>
> - We are using YOLOv8 as a base model and we are adding new features to it to make it more suitable for our use case.
>
> - Our Gorgeous Team :
> - ![photo_2023-07-10_23-22-16](https://github.com/MohamedAtef321/RTSD-Road-Traffic-Signs-Detection-System/assets/73308647/b793d241-7cc9-421f-8f4a-7ac9df1579bf)


<div align="center">

## 📃 Table of Contents

</div>

- [👋 Introduction](#👋-introduction)
- [📑 Project Steps](#📑-project-steps)
- [💾 Dataset](#💾-dataset)
- [🌌 Model](#🌌-model)
- [✅ Results](#✅-results)
- [⚡ Additional Features](#⚡-additional-features)
- [📕 References](#📕-references)

<div align="center">

## 👋 Introduction

The main goal of this project is to detect traffic signs 🚩 along the road, this project aims to enable self-driving cars 🚗 to see and interact with the road signs. The project is implemented using [YOLOv8: Extended Edition](https://github.com/MohamedAtef321/YOLOv8-Extended-Edition) and [RTSD Dataset](https://universe.roboflow.com/classes-ehzdo/new_classes/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true) and ran on Raspberry Pi 4.

</div>

<div align="center">

## 📑 Project Steps

</div>

Throughout the project, we followed these steps:
1. First we used [RoboFlow](https://roboflow.com/) to create the dataset in YOLO format.
2. Then we used [Google Colab](https://colab.research.google.com/) to train the model.
3. Finally we used Raspberry Pi 4 to run the model on the real-time video stream from the camera.

<div align="center">

## 💾 Dataset

</div>

We created collected the data from multiple sources, and then we merged them all into one dataset. The dataset contains 20 classes of traffic signs 🚩and 1 class of bump. The dataset is divided into 3 parts:
1. Training set: 80% of the dataset
2. Validation set: 10% of the dataset
3. Testing set: 10% of the dataset

The dataset is available on [RoboFlow](https://universe.roboflow.com/classes-ehzdo/new_classes/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true)

<div align="center">

## 🌌 Model

</div>

We used [YOLOv8: Extended Edition](https://github.com/MohamedAtef321/YOLOv8-Extended-Edition) which is forked from [YOLOv8](https://github.com/ultralytics/ultralytics), but with some modifications such as "Night Vision", "Lane Line Detection" and "SPI Communication Protocol to send outputs". \
If you want to know more about the model, you can check the [YOLOv8: Extended Edition](https://github.com/MohamedAtef321/YOLOv8-Extended-Edition).

<div align="center">

## ✅ Results

</div>

The model was trained for 300 epochs, and the results are as follows:

| Metric | Value |
| :---: | :---: |
| Precision | 0.97 |
| Recall | 0.98 |
| mAP50 | 0.99 |
| mAP50-95 | 0.87 |

The model was tested on the real-time video stream from the camera, and the results are as follows:

![Results](

)

<div align="center">

## ⚡ Additional Features

</div>

We added some additional features to the project to make it more useful, some of these features are on the model and some are on the dataset.

### Model Features :
1. **Night Vision**: The model can detect traffic signs 🚩 at night using the night vision feature.
2. **Lane Line Detection**: The model can detect lane lines using the lane line detection feature.
3. **SPI Communication Protocol**: The model can send the outputs to the Raspberry Pi 4 using the SPI communication protocol.

### Dataset Features :
1. **Bump Class**: We added a bump class to the dataset, which is used to detect bumps on the road.

<div align="center">

## 📕 References

</div>

1. [YOLOv8: Extended Edition](https://github.com/MohamedAtef321/YOLOv8-Extended-Edition)
2. [YOLOv8](https://github.com/ultralytics/ultralytics)
3. [RTSD Dataset (RoboFlow)](https://universe.roboflow.com/classes-ehzdo/new_classes/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true)


<div align="center">

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

</div>

<div align="center">

## 🙋‍♂️ Authors

[Mohamed Atef](https://github.com/MohamedAtef321) - [Mohamed Wael](https://github.com/Elbahkiry) - [Ahemd Ezz Eldin](https://github.com/AhmedEzzeldeenn)

</div>
