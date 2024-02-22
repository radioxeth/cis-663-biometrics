# Week 7 Performance Evaluation

## Directory
- [Home](/README.md#table-of-contents)
- [Week 1 Introduction to Biometrics](/week1/README.md#week-1-introduction-to-biometrics)
- [Week 2 Workings of a Biometrics System](/week2/README.md#week-2-workings-of-a-biometrics-system)
- [Week 3 Physiological Biometrics: Fingerprint Biometrics](/week3/README.md#week-3-physiological-biometrics-fingerprint-biometrics)
- [Week 4 Physiological Biometrics: Facial Recognition Systems](/week4/README.md#week-4-physiological-biometrics-facial-recognition-systems)
- [Week 5 Other Biometrics: Iris, Hand Geometry, Palm Print, DNA](/week5/README.md#week-5-other-biometrics-iris-hand-geometry-palm-print-dna)
- [Week 6 Heart Beat and Some Machine Learning Algorithms](/week6/README.md#week-6-heart-beat-and-some-machine-learning-algorithms)
- **&rarr;[Week 7 Performance Evaluation](/week7/README.md#week-7-performance-evaluation)**
- [Week 8 Behavioral Biometrics: Keystrokes, Gait, Handwriting, Voice](/week8/README,md#week-8-behavioral-biometrics-keystrokes-gait-handwriting-voice)
- [Week 9 Continuous Authentication](/week9/README.md#week-9-continuous-authentication)
- [Week 10 Biometric Systems Security](/week10/README.md#week-10-biometric-systems-security)



## Live Session

### Iris Recognition Diagram

#### Image Acquisition
- capture sequence of iris images using cameras and sensors with high resolution and sharpness
  - show the entire eye, iris, pupil

- preprocessing images improves classification

#### Segmentation/concept

- first stage of iris segmentation to isolate the iris.
- edge detection
  - vertical and horizontal edge map
  - use OR function to overlap the two
    - use cannel or sobl filters for the edge detectors

#### Hough Transform

- circular hough transform can be employed to deduce the radius center coordinates of the pupil and iris regions
- looking for a circle within a circle

$x_c^2+y_c^2-r^2=0$


- remove eyelashes using a linear hough transform
- look for 4 45 deg angle with circular eye and linear eyelid

#### Normalization
- adjust for pupil size, bloodshot eyes et

#### Radial Vectors
- daugman's rubber sheet model
- the number of data points selected along each radial line is **radial resolution**
- the number of radial lines going around the iris region is defined as the **angular resolution**

- average pixel intensity in the resolution grid

#### Feature Encoding
- creating a template containing ony the most discriminating features of the iris
- Gabbor filter

#### Feature Matching
- Hamming Distance
  - lower the value the better


### ECG and Pattern Recognition
#### ECG (Electrocardiogram)

- ECG measures the change in electrical potential over time
- fiducial point plays a key bases

#### ECG Filtering
- fourier transform
- filter
  - high pass
  - low pass
  - band pass

#### ECG Normalization
- measure the distances
- normalize against time!
  - whole time window/measured distances

### Pattern Recognition

(next week)