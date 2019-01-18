# Berkeley Deep Drive-X (eXplanation) Dataset

We focus on generating textual descriptions and explanations, such as the pair:<br />
*“Vehicle slows down”* (description) and *“Because it is approaching an intersection and the light is red”* (explanation)

<center><img src="/img/overview.png" width="90%" height="90%"></center>

### How to Download.
Download our *BDD-X dataset* ([Download](https://drive.google.com/open?id=1Na-jxLK7VxOc6wcT5lnLQytfFi6rqhTF)), which contains:

- BDD-X-Annotations_v1.csv: Our annotations for textual descriptions and explanations.
- {train, val, test}.txt: Splits for Training, validation, testing set

### How to Use.
See [Textual Explanations for Self-driving Vehicles](https://github.com/JinkyuKimUCB/explainable-deep-driving.git).

### Statistics.
Our dataset is composed of over 77 hours of driving within 6,970 videos. The videos are taken in diverse driving conditions, e.g. day/night, highway/city/countryside, summer/winter etc. On average 40 seconds long, each video contains around 3-4 actions, e.g. speeding up, slowing down, turning right etc., all of which are annotated with a description and an explanation. Our dataset contains over 26K activities in over 8.4M frames. We introduce a training, a validation and a test set, containing 5,597, 717 and 656 videos, respectively.

<center><img src="/img/statistics.png" width="20%" height="20%"></center>


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
#### Berkeley DeepDrive dataset
Our explanation dataset is built on top of Berkeley Deep Drive dataset (<https://bdd-data.berkeley.edu/>) collected from dashboard cameras in human driven vehicles. This dataset contains dashboard camera videos, approximately 40 seconds in length, captured by a single front-view camera mounted behind the windshield of the vehicle. Videos are mostly captured during urban driving in various weather conditions, featuring day and nighttime. The dataset also includes driving on other road types, such as residential roads (with and without lane markings), and contains all the typical driver’s activities such as staying in a lane, turning, switching lanes, etc. Alongside the video
data, the dataset provides a set of time-stamped sensor measurements, such as vehicle’s velocity, course, and GPS location.

#### Annotation promt
Our annotation prompt is shown below. The annotation process is as follows. We provide a driving video and ask a human annotator to imagine herself being a driving instructor. Note, that we specifically select human annotators who are familiar with US driving
rules. The annotator has to describe what the driver is doing (especially when the behavior changes) and why, from a point of view of a driving instructor. Each described action has to be accompanied with a start and end time-stamp. The annotator may stop the video, forward and backward through it while searching for the activities that are interesting and justifiable.

<center><img src="/img/interface.png" width="70%" height="70%"></center>

### Preview of the Annotations.
[![Video Label](/img/bdd-x.png)](https://youtu.be/kbft0HEWdpk)

#### Need help?
Please contact us <bdd.x.data@gmail.com> with any questions/inquiries.
