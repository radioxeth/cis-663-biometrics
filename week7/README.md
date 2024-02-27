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

## Performance Evaluation

### Why We Need Performance Measures

- Why we need
  - needed to compare and evaluate performance of various systems
  - setting threshold a priori
  - selection of classification algorithms
- Various measures of performance
  - FAR, FRR, cost
  - Usability
  - Liveness detection
  - And many other

### Types of Errors: Classification
- X_I stored template of a user I
- X_Q acquired input
- Matching score S(X_Q,X_I) < t, then D_0, else D_1
<hr>
- H_0 X_Q does not come from the same person as X_I
  - Type I: False match (D_! is decided when H_0 is true)
- H_1 X_Q comes from the same person as X_I
  - Type II: false nonmatch (D_0 is decided when H_1 is true)
- D_0 person is not who she claims to be
  - FMR (false positive): probability of type I error = P(D_1|H_0)
- D_1 person is who she claims to be
  - FNMR (false negative): probability of type II error = P(D_0|H_1)

### Receiver Operating Characteristics (ROC)

#### Receiver Operating Characteristics Curve
plot FPR vs TPR
- need multiple rates
  - run same algorithm over different data sets
  - run same algorithm with different thresholds

### Detection Error Trade-Off (DET) and an Example

#### Detection Error Trade-Off Curve

- FPR vs FNR
- can use EER - Equal Error Rate
  - FPR and FNR are the same

- **gives info as to how well the attack is working**

### Detection Cost Function

#### Detection Cost Function and Half Total Error Rate (HTER)

- DCF = Cost(FR).P(client).FRR + Cost(FA.P(imposter)).FAR
  - P(client): prior probability that a client will use the system
  - P(imposter): prior probability that an imposter wil use the system
  - Cost(FR): cost of false rejection
  - Cost(FA): cost of false acceptance

Half total error rate when the costs are 1 each and the probabilities are 0.5 each.
- $\text{HTER} = \frac{\text{FAR}+\text{FRR}}{2}$

### Other Performance Measures
- Failure to enroll rate (FTE): The proportion of enrollment transactions in which zero subjects are successfully enrolled.
  - examples: fingerprint quality not good, for example because of rough hands

- Failure to acquire rate (FTA): the proportion or weighed proportion of recognition attempts in which a system fails to detect, identify, or acquire a sample of adequate quality
- Example: due to failures related to user presentation, sample segmentation, feature extraction, or quality control
  - depends on the thresholds established for sample quality, the duration of time allowed for sample acquisition, and the allowed number of presentation attempts
  - typically technology evaluations operate using a previously collected database, which eliminates the possibility of FTA during performance testing (although an FTA rate for the dataset may be available for consideration)

- Generalized false accept rate (GFAR)
  - combines enrollment, sample acquisition, and matching errors for single - attempt transactions. GFAR occurs when both the approved user and imposter are re-enrolled, the submitted samples are accepted, and a false match is made
  - generalized false accept rate 
    - > (GFAR) x threshold = (1-FTA) x (FMR x threshold) x (1 - FTE)

- Generalized false reject rate (GFRR)
  - combines enrollment, sample acquisition, and matching errors for single-attempt transactions. GFRR occurs when the user is not enrolled, or the submitted sample cannot be acquired, or a false match occurs.
    - generalized false reject rate (GFRR) x threshold = FTA + (1-FTA) x FTE + (1-FTA) x (1-FTE) x (FNMR x threshold)

### Usability Measures

- **Usability**: the extent to which a product can be used by specified users to achieve specified goals with effectiveness, efficiency, and satisfaction in a specified context of use (International Organization for Standardization (ISO))
- **Learnability**: the ease with which users can complete basic tasks on their first encounter with a biometric system
- **Efficiency**: the speed at which users can perform a task after becoming familiar with the system
- **Memorability**: the eas with which users can reestablish system proficiency following a persons of system disuse
- **Errors**: the number of user errors that occur during system use, the severity of suer errors, and the degree to which users can recover from such errors
- **Satisfaction**: the degree to which users find the system pleasant to operate

### Need for sufficient user data to make a classification decision
- Enrollment transaction duration/mean time to enroll (MTTE): the length of time required for subjects to completely enroll all positions into a biometrics system
  - for example, biometric employee enrollment in a human resources office might occupy several minutes of time while paperwork is being filled out
  - enrollment in point-of-sale biometric application may be conducted within seconds to address throughput requirements

- Recognition attempt duration/mean time to detection (MTTD)
- Throughput rates
- User throughput rates
- Matching algorithm throughput rates
- Verification time

### Performance Measures for Continuous Authentication

- Attributes
- Interaction quotient (% of interaction with a device) - give examples
- Interaction type: active/explicit, passive/implicit
- Session length
- time to recognize (imposter rejection time)
- Time to alert (time to correct rejection)
- Mean time to enroll (MTTE)
- Mean time to detect (MTD)
- Latency period -- no data is generated

### Performance Measures of Liveness Detection
- suspicious presentation detection; non suspicious presentation detection
- artifact detection; non artifact detection
- **False non-suspicious presentation detection (FNSPD)**: occurs when a liveness detection system classifies a suspicious biometric presentation as non-suspicious
- **False suspicious presentation detection (FSPD)**: occurs when a liveness detection system flags a non-suspicious biometric presentation as suspicious
- **False artifact detection rate (FADR)**: describes the proportion of nonartifact presentations erroneously flagged as artifacts
- **False non-artifact detection rate (FNDR)**: describes the proportion of artifact presentations erroneously classified as non-artifacts.


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