# Week 1 Introduction to Biometrics

## Directory
- [Home](/README.md#table-of-contents)
- **&rarr;[Week 1 Introduction to Biometrics](/week1/README.md#week-1-introduction-to-biometrics)**
- [Week 2 Workings of a Biometrics System](/week2/README.md#week-2-workings-of-a-biometrics-system)
- [Week 3 Physiological Biometrics: Fingerprint Biometrics](/week3/README.md#week-3-physiological-biometrics-fingerprint-biometrics)
- [Week 4 Physiological Biometrics: Facial Recognition Systems](/week4/README.md#week-4-physiological-biometrics-facial-recognition-systems)
- [Week 5 Other Biometrics: Iris, Hand Geometry, Palm Print, DNA](/week5/README.md#week-5-other-biometrics-iris-hand-geometry-palm-print-dna)
- [Week 6 Heart Beat and Some Machine Learning Algorithms](/week6/README.md#week-6-heart-beat-and-some-machine-learning-algorithms)
- [Week 7 Performance Evaluation](/week7/README.md#week-7-performance-evaluation)
- [Week 8 Behavioral Biometrics: Keystrokes, Gait, Handwriting, Voice](/week8/README,md#week-8-behavioral-biometrics-keystrokes-gait-handwriting-voice)
- [Week 9 Continuous Authentication](/week9/README.md#week-9-continuous-authentication)
- [Week 10 Biometric Systems Security](/week10/README.md#week-10-biometric-systems-security)

## Course Outline

- physiological
    - fingerprint
    - face
    - iris
    - palm print
    - dna

- behavioral
  - typing patterns
  - hand moving patters
  - walking patters

- brain patterns
  - measuring current flow
  - muse

- security threats
- components of biometrics
  - how do we build a biometric system?

- how do we authenticate using biometrics
  - machine learning

## What is Biometrics and Its History?

- meaning and uses
  - the word biometrics is derived from two greek works 
    - 1 bios means life
    - 2 metricos means measure
  - automatic recognition on their physical, behavioral, or neurological characteristics
  - confirm or establish the identity of individuals

- History
  - mid 19th century - paris police use body measurements to identify criminals
  - late 19th - fingerprints
  - current - huge growth with technology

## Taxonomy of Biometrics

- authentication
  - something a user knows
    - knowledge based authentication
      - password
  - something a user has
    - object based authentication
      - a token
  - something a user is
    - biometrics
    - physiological
      - fingerprint
      - face
    - behavioral
      - keystroke
      - gait
    - neurological
       - brain-computer interface
       - NeuroSky, muse, fMRI

## What Qualifies as a Biometric?

- Needed
  - Universality
  - Uniqueness or distinctiveness
  - permanence
  - collectability
- Desired
  - acceptability
    - willingness of user to accept the biometric system
  - performance
  - circumvention

From "An Introduction to Biometric Recognition" A Jain, Ross, and S Prabhakar IEEE Jan 2004

## Various Biometrics

&darr; universality
<br>
&darr; uniqueness
<br>
&darr; distinctiveness
<br>
&darr; permanence
<br>
&darr; collectibility
<hr>
&darr; acceptability A
<br>
&darr; performance P
<br>
&darr; circumvention C

- DNA
  - Deoxyribonucleic acid
  - universality, uniqueness, unique, collect
- Ear
- Face
- Facial
- Fingerprint
- Gait
  - video or mobile phone
- Hand and Finger geometry
- Iris
- Keystroke
- Odor
- Palm print
- retinal scan
- signature
- voice
- Brain signals

## Areas and Applications of Biometric Systems

### Areas Include

- sensing
  - measure features
- machine learning
- pattern recognition
- image processing
- data mining
- statistics
- psychology
- decision science

### Applications of Biometric Systems
- Commercial
  - compliance
  - atm cards
  - banking
- Government
  - national id card
  - passports
- Forensics
  - Corpse Identification
  - criminal investigation
    - fingerprint, dna, voice recording

## Limitations of Unimodal Biometrics and Multimodal Biometrics

### Limitations on Unimodal Biometrics
- noise in sensed data
  - fingerprint sensor might be bad
- infra-class variation
  - psychological behavior
- distinctiveness
  - might extract the wrong features
- nonuniversality
  - poor quality of fingerprint ridges
  - Failure to Enroll - FTE ~4%
- spoof attacks
  - 

### Multimodal Biometric Systems

- Multiple sensors
  - information from difference sensors for the same biometric, such as optical, solid-state, and ultrasound sensors for fingerprint capture
- multiple biometrics
  - combination of multiple biometrics, such as fingerprint, face, and retina scan, etc
- multiple units of same biometric
  - from different units, such as fingerprints from different fingers
- multiple snapshots of the same biometric
  - more than one measurement of the same biometric - for example, voice at different points of time or several images of the same face may be combined
- multiple representation and matching algorithms for the same biometric
  - different features or different feature extraction and combination methods or different matching algorithms