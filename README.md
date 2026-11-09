# SYN-MAD-2022

This is the repository for the IJCB-SYN-MAD-2022: Competition on Face Morphing Attack Detection Based on Privacy-aware Synthetic Training Data. The competition was held at the [International Joint Conference on Biometrics 2022](https://ijcb2022.org/#/). 

The final results of the competition were presented in a summary paper at IJCB 2022. The paper can be accessed here: [Paper](https://arxiv.org/abs/2208.07337)

## Competition Training Data ##
The synthetic training data that the competitors were allowed to use for training the morphing detectors was limited to the SMDD dataset. This can be requested [here](https://github.com/naserdamer/SMDD-Synthetic-Face-Morphing-Attack-Detection-Development-dataset). In addition, we also provide two files containing the bounding boxes and facial landmark points: 

* [Bounding box for morphed images of SMDD](https://drive.google.com/file/d/1-NmRcAnPTqVX1_Y7BKBBDsh9XTLYpySr/view)
* [Bounding box for bona fide images of SMDD](https://drive.google.com/file/d/1g9JfIubNlvjnHwxkTHeV8JaDMMWwsO-N/view)

### Bounding Box / Landmarks ###
The files contain in each line a sample, e.g.:
```
 ./m15k_t/morphed_img000184_img282038.png 43 197 41 240 97 123 161 123 133 156 95 182 158 183
```
The values in each row are structured as follows: 
```
/path/referene_1.jpg bb_x1 bb_x2 bb_y1 bb_y2 left_eye_x left_eye_y right_eye_x right_eye_y nose_x nose_y mouth_left_x mouth_left_y mouth_right_x mouth_right_y 
```
were x1, x2, y1 and y2 are the bounding boxs points. And all others number refer to the respective coordinates of the face landmarks (left eye, right eye, nose, mouth left, mouth right).

## Competition Testing Data ##
For the evaluation of the submissions a new benchmark, MAD22 has been created by the organizers of the competition. The benchmark is based on the [Face Research Lab London dataset (FRLL)](https://figshare.com/articles/dataset/Face_Research_Lab_London_Set/5047666). The created benchmark contains 4483 morphed face images and 204 bona fide images from the FRLL dataset and five different morphing approaches (three landmark-based, two GAN-based) has been used to create the dataset. For more details on the benchmark, we refer to the competition summary paper.


The MAD22 benchmark can be requested per mail at: marco.huber@igd.fraunhofer.de . **Please share your name, affiliation, and official email in the request form**. The bounding boxes and landmarks are included and presented in the same way as described above.

UPDATE Nov 2026: Due to an automatic update and content scan from Google Drive, some parts of the dataset has been removed. The completeness of the data provided previously over Google Drive cannot be ensured. The dataset will not longer be provided using Google Drive. Please request the dataset again with writing an Email to: marco.huber@igd.fraunhofer.de.


If you use the MAD22 benchmark, please cite:
```
@inproceedings{DBLP:conf/icb/HuberBLRRDNGSCT22,
  author       = {Marco Huber and
                  Fadi Boutros and
                  Anh Thi Luu and
                  Kiran B. Raja and
                  Raghavendra Ramachandra and
                  Naser Damer and
                  Pedro C. Neto and
                  Tiago Gon{\c{c}}alves and
                  Ana Filipa Sequeira and
                  Jaime S. Cardoso and
                  Jo{\~{a}}o Tremo{\c{c}}o and
                  Miguel Louren{\c{c}}o and
                  Sergio Serra and
                  Eduardo Cerme{\~{n}}o and
                  Marija Ivanovska and
                  Borut Batagelj and
                  Andrej Kronovsek and
                  Peter Peer and
                  Vitomir Struc},
  title        = {{SYN-MAD} 2022: Competition on Face Morphing Attack Detection Based
                  on Privacy-aware Synthetic Training Data},
  booktitle    = {{IEEE} International Joint Conference on Biometrics, {IJCB} 2022,
                  Abu Dhabi, United Arab Emirates, October 10-13, 2022},
  pages        = {1--10},
  publisher    = {{IEEE}},
  year         = {2022},
  url          = {https://doi.org/10.1109/IJCB54206.2022.10007950},
  doi          = {10.1109/IJCB54206.2022.10007950},
  timestamp    = {Tue, 13 Jan 2026 12:10:37 +0100},
  biburl       = {https://dblp.org/rec/conf/icb/HuberBLRRDNGSCT22.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}

```
