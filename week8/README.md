# Week 8 Behavioral Biometrics: Keystrokes, Gait, Handwriting, Voice

## Directory
- [Home](/README.md#table-of-contents)
- [Week 1 Introduction to Biometrics](/week1/README.md#week-1-introduction-to-biometrics)
- [Week 2 Workings of a Biometrics System](/week2/README.md#week-2-workings-of-a-biometrics-system)
- [Week 3 Physiological Biometrics: Fingerprint Biometrics](/week3/README.md#week-3-physiological-biometrics-fingerprint-biometrics)
- [Week 4 Physiological Biometrics: Facial Recognition Systems](/week4/README.md#week-4-physiological-biometrics-facial-recognition-systems)
- [Week 5 Other Biometrics: Iris, Hand Geometry, Palm Print, DNA](/week5/README.md#week-5-other-biometrics-iris-hand-geometry-palm-print-dna)
- [Week 6 Heart Beat and Some Machine Learning Algorithms](/week6/README.md#week-6-heart-beat-and-some-machine-learning-algorithms)
- [Week 7 Performance Evaluation](/week7/README.md#week-7-performance-evaluation)
- **&rarr;[Week 8 Behavioral Biometrics: Keystrokes, Gait, Handwriting, Voice](/week8/README,md#week-8-behavioral-biometrics-keystrokes-gait-handwriting-voice)**
- [Week 9 Continuous Authentication](/week9/README.md#week-9-continuous-authentication)
- [Week 10 Biometric Systems Security](/week10/README.md#week-10-biometric-systems-security)

## Behavioral Biometrics: Keystrokes, Gait, Handwriting, Voice

### Machine Learning Methods Applied to Security Domain

#### Introduction
- Keystroke based authentication
- Authentication on mobile devices
  - authentication
  - data definition, feature extraction
  - cleaning
- BCI - brain computer interface

### Keystroke Dynamics
- An example of behavioral biometrics
  - relatively high variability between successive samples
  - still provides disciminability to distinguish
  - stable over shorter time spans
  - prone to replay attacks
- Advantages
  - samples can be collected remotely, for example, on the internet
  - widespread use: desktops, laptops, and mobile devices
  - non-intrusive
- Choice of device, for example, desktop keyboard or mobile device can affect sample variability
  - methods to find invariants are successful
- useful as a second-factor in authentication

### Feature Extraction, Fixed Text and Free Text

- KHT: Key Hold Time
  - KP_r - KP_s
- KIL: Key Interval Latency
- KPL: Key Press Latency

3 people typing the same word will have different timings
- can be second factor authentication with password

<hr>
- Fixed text: password
- Continuous text: describe an event

### Feature Cleaning

#### Outlier Detection
- Method 1
$X\in{\{\bar{x}-w\sigma{},\bar{x}+w\sigma{}\}}$
- Method 2
- define a neighborhood of a feature value as region
N= a feature vector is an outlier if fewer than &beta; values fall within the neighborhood.

$x_i=\{247,476,281,250,281,265,1235\}$