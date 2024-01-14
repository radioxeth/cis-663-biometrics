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

## Security of Biometric Systems
- Types of Vulnerabilities and Attacks
  - admin
  - user
  - enrollment spoofing
  - bypass
  - corruption
  - tampering
  - brute force attack
  - replay
- consequences of attacks
  - privacy
  - privileges
  - financial and personal
  - various others

### Attack Levels
- sensor level
  - presenting a fake biometric
- transmission between sensor and feature extractor
  - replay of stored digital biometric signals
- feature extractor level
  - denial of feature extraction
- transmission of the extracted features
  - spoofing the biometric feature
- classifier level
  - attacking the matching module
- database
  - attacking the channel between the template database and matching module
- transmission of the template from the database
- decision level
  - attacking the final decision process

### Vulnerability of Biometric Systems

| Biometric | Vulnerability             | Possible Solutions |
|-----------|---------------------------|--------------------|
| Fingerprint | Synthetic or dismembered finger | To use thermal scanners to detect the temperature. Detection of a perspiration pattern over the fingertip skin can identify the vitality of a fingerprint |
| Voice | A tape recording of the authorized user | To use a text-dependent system (different for each trial) |
| Iris | Prosthetic eye | Infrared system for checking veins will look at flows of warm blood |
| Face | Face mask etc. | Facial tomography |

### Frog-Boiling Attacks

With the prediction set, users are clustered into four types of animals: Lamb, goat, wolf, and sheep, as described in [Doddington et al., 1998]

- **Lamb**: Lambs are the users who are vulnerable to imposter attack, their FRRs are higher than others.
- **Goat**: Goats are the users who find difficulty matching against their own template. Specifically, goats have higher FAR than other users.
- **Wolf**: Wolves can match well against other users, therefore, there are considered “strong attackers.”
- **Sheep**: Sheep are the users who do not belong to any of the above groups. They are the users who generally have good verification performance.


## Future of Biometric Systems
- physiological systems likely to stay
- cameras and videos are ubiquitous
  - facial, retinal, finger print to stay
- rise of brain-computer interfaces
- authentication biometrics
- biometrics of devices
- can change in color of face correlate with video

## Week 1 Live Session

### Requirements of Biometrics
- universality
- distinctiveness
- permanence
- collectability
- performance
- acceptability
- circumvention

### Verification vs Identification Mode

- Verification (Authentication): Given biometric input and supposed indentity validate that the biimetric input should come from identity. Returns a Boolean (T/F)
  - V(I,X_Q)=True if S(X_Q,X_I)>=t, false otherwise
- Identification (recognition): given biometric input return identity (or unkown flag) that owns said biometric.
  - Id(X_Q)= {I_k=max{S(X_Q,X_ik)}>=t, k=1,2,3...N}, I_n+1 if no match found

### Biometric Systems
1. Sensor Modules: Extracts biometric data from individual
2. Feature Extraction Module: Extracts Features from Biometric Data
3. Matcher Module: Compares extracted features against stored **templates**. Performs the actual decision (match, no match)
4. Database Module: Stores captured templates for known users
5. Enrollment Module: Enrolls users into the system. Involves ##1, ##2 and may perform quality analysis on sample. Extracts template from quality samples
6. Pattern Recognition/Machine Learning: Offline modules that adjusts internal values to improve system accuracy.

### Biometric System Errors

- Imposter Distribution: the distribution of S(X_Q,X_I) (scores) where X_Q ***does not*** come from individual I
- Genuine Distribution: the distribution of S(X_Q, X_I) (scores) where X_Q ***does*** come from individual I
- False Match: the system returning a match between two different people
- False Nonmatch: the system returning a nonmatch for a known user's input
- False Match rate: Rate of False Matches
- False Nonmatch Rate: Rate of False Nonmatches

### More Error Review

- H_0: input X_Q does not come from the same person as X_I (null hypothesis)
- H_1: Input X_Q does come from the same person as X_I
- D_0: person is not who she claims to be (system output)
- D_1: person is who she claims to be (system output)

- Type-I: false match (D_1 is decided when H_0 is true)
- Type-II: false nonmatch (D_0 is decided when H_1 is true) FNMR: P(D_0|H_1)
- conditional probability: $P(A|B)$=probability of A being true given we know (or assume) B is true:
  - $P(A|B)=\frac{P(A&&B)}{P(B)}$

FMR=\integral_t^infin p(S(X_Q,XI)|H_0)
FNMR=\integral_-infin^t p(S(X_Q,XI)|H_1)

### Enrollment

- FTC: Failure to capture rate. Occurs when a biometric sample of sufficient quality is not being extracted
- FTE: Failure to enroll rate. Occurs when the system rejects poor quality inputs during enrollment

### FMR and FNRM in Identification
- FNMR_N (N subscript because we assume there are N templates in the system to match against)
  - FNMR_N FNMR (false nonmatch rate in identification)
- FMR_N 1-(1-FMR)^N NFMR (False match rate in identification)
