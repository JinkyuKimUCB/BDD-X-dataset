# Berkeley Deep Drive-X (eXplanation) Dataset

We focus on generating textual descriptions and explanations, such as the pair:<br />
*“Vehicle slows down”* (description) and *“Because it is approaching an intersection and the light is red”* (explanation)

<center><img src="/img/overview.png" width="90%" height="90%"></center>

### How to Download.
Download the BDD-X videos and annotations. <br />
See the folder *BDD-X-Dataset*, which contains:

- BDD-X-Annotations_v1.csv: Our annotations for textual descriptions and explanations.
- {train, val, test}.txt: Splits for Training, validation, testing set

### Statistics.
Our dataset is composed of over 77 hours of driving within 6,970 videos. The videos are taken in diverse driving conditions, e.g. day/night, highway/city/countryside, summer/winter etc. On average 40 seconds long, each video contains around 3-4 actions, e.g. speeding up, slowing down, turning right etc., all of which are annotated with a description and an explanation. Our dataset contains over 26K activities in over 8:4M frames. We introduce a training, a validation and a test set, containing 5,597, 717 and 656 videos, respectively.

<center><img src="/img/statistics.png" width="20%" height="20%"></center>


<!--
### Preview of the Annotations.
[![Video Label](/img/bdd-x.png)](https://youtu.be/kbft0HEWdpk)
-->

### Citation.
If you find this dataset useful, please cite this paper (and refer the data as Berkeley DeepDrive eXplanation or BDD-X dataset):
```
@article{kim2018textual,
  title={Textual Explanations for Self-Driving Vehicles},
  author={Kim, Jinkyu and Rohrbach, Anna and Darrell, Trevor and Canny, John and Akata, Zeynep},
  journal={Proceedings of the European Conference on Computer Vision (ECCV)},
  year={2018}
}
```

### How we collect.
Our explanation dataset is built on top of Berkeley Deep Drive dataset (<https://bdd-data.berkeley.edu/>) collected from dashboard cameras in human driven vehicles. Annotators view the video dataset, compose descriptions of the vehicle’s activity and explanations for the actions that the vehicle driver performed.

<center><img src="/img/interface.png" width="70%" height="70%"></center>
