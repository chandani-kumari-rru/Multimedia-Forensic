# Multimedia Forenisc
- in multimedia forensic covers `Audio`, `Video`, `Image`, `Text` Forensic.
- Video Lecture
  - Audio Forensic: vid[1.1](https://youtu.be/QsopUPy5nvs?si=ENvUMMDLWUopGU4E),[vid2](https://youtu.be/qQhB5uDQQCU?si=Q8PHxLQMLOVsj9xO)
  - Image Forensic: [1.2](https://youtu.be/iz-xPlradnU?si=io7LjWE4k-zUJWZb),[1.3](https://youtu.be/Ljn2A6MfCW4?si=r0SHfx9AvWPoOUxw),[1.4](https://youtu.be/K2hyRz9IYQs?si=MuSwezlE-qoiSKIz),[1.5](https://youtu.be/3VTfU0LTUy4?si=1YC7wIvn6-WlVwQr)

## 📑 Table of Contents

- [Audio Forensic](#audio-forensic)
  - [Mechanism of Voice Generation](#mechanism-of-voice-generation)
  - [Production of Speech](#production-of-speech)
  - [Challenge in Audio Processing](#challenge-in-audio-processing)
  - [Analysing Audio as a Investigator](#analysing-audio-as-a-investigator)
    - [Authentication](#audio-authentication)
    - [Enhancement](#Enhancement)
    - [Interpretation](#Interpretation)
    - [Critical Listening](#Critical-Listening)
    - [Visual Inspection](#Visual-Inspection)
    - [Analyzing Metadata](#Analyzing-Metadata)
  - [Audio Evidence in Investigation Laboratory](#Audio-Evidence-in-Investigation-Laboratory)
  - [Speaker Recognition](#speaker-identification/recognition)
  - [Method of Speaker Identification](#methods-of-speaker-identification)
  - [Audio Examination Tools](#audio-examination-tools)
  - [Common facing Forensic Audio Cases](#Common-facing-Forensic-Audio-Cases)
- [Video Forensic](#video-forensic)
- [Image Forensic](#Image-Forensic)
  - [Method of Image Authentication](#Method-of-Image-Authentication)
  - [Image Manipulation Technique](#Image-Manipulation-Technique)
    - [Pixel-based](#Pixel-based-method)
    - [Camera-based](#Camera-based-method)
    - [Physical-based](#Physical-based-method)
    - [Format-based](#Format-based-method)
  - [Camera Ballistics](#Camera-Ballistics)
  - [Digital Camera Structure](#Digital-Camera-Structure)
  - [Lens Radial Distortion](#Lens-Radial-Distortion)
  - [Sensor Defect Noise](#Sensor-Defect-Noise)
  - [Illumination Inconsistences](#Illumination-Inconsistences)
  - [Error Level Analysis](#Error-Level-Analysis)
- [Text Forensic](#Text-Forensic)
---

# Audio Forensic
- Sound can be visualized in waveform. waveform can be seen with tools like `Audacity`.
<img width="1789" height="796" alt="image" src="img/waveform.png" /> 

- Parameter of Audio Signals: Frequency, Amplitude, Phase, Intensity, pitch, Loudness, etc
- 2 types of Audio Signals: Analog & Digital
<img width="1699" height="852" alt="image" src="img/waveforms.png" />

| ADC | DAC |
|---|---|
|<img width="1046" height="411" alt="image" src="https://github.com/user-attachments/assets/3930ebe7-3806-4a48-9b69-f00f3e674b65" />|<img width="1046" height="447" alt="image" src="https://github.com/user-attachments/assets/9ed51748-9c0a-4692-b0d5-398f9710665c" />|


### Mechanism of Voice Generation
<img width="838" height="341" alt="image" src="https://github.com/user-attachments/assets/d047bf53-f3e2-4478-ade9-a4397f5dd99a" />

| SEPEAKER | LISTENER |  
|---|---|  
| `Production of vibrational energy` by `articulation` after brain instructs to perform | `Eardrums` convert this vibrational energy into signals that travel along nerves to the brain, which `interprets` them as `voices`, `music`, `noise`, etc. |

### Production of Speech
<p align="center"><img width="696" height="445" alt="image" src="https://github.com/user-attachments/assets/0ba76e42-fa72-4be7-948b-7ebd0414878a" /></p>

- The basic responsible function for production of speech are: `Generation of air pressure`, `regulation of vibration`, and `control of resonators`.
- Larynx sometimes called `voice box` is the most important  organ among Lung, Vocal code, pharynx, Tongue, Teeth & Lip etc. Tongue is also the valuable articulatory organ.

Place of Articulation
| | |  
|---|---| 
|1. Exo-labial, 2. Endo-labial, 3. Dental, 4. Alveolar, 5. Post-alveolar, 6. Pre-palatal, 7. Palatal, 8. Velar, 9. Uvular, 10. Pharyngeal, 11. Glottal, 12. Epiglottal, 13. Radical, 14. Postero-dorsal, 15. Antero-dorsal, 16. Laminal, 17. Apical, 18. Sub-apical|<img width="626" height="783" alt="image" src="https://github.com/user-attachments/assets/3e64776a-3a4e-4f50-a149-a8a6d39a775c" />|

Why animal can’t produce speech
- because they don’t have `co-articulation system`

Why person to person different in voice ?
- As  `vocal tracks` are differ in `shape`, `size` and `length` and the tension of the vocal folds, the voice production is also different to person to person
<p align="center"><img width="603" height="377" alt="image" src="https://github.com/user-attachments/assets/2b67f08b-f928-4a41-bb0c-93b82f15c97b" /></p>




### Challenges in Audio Processing
- `Noise`: Unwanted sound makes extraction and analysis harder.
- `Aliasing & Quantization Errors`: Bad sampling/poor bit depth reduces fidelity.
- `Loss of Information`: Compression and downsampling can discard important details.
- `Subjectivity in Loudness/Pitch Perception`: Variability in human listeners means technical measurements don't always match perception.

### Analysing Audio as a Investigator
- Authenticity
- Enhancement
- Interpretation
- Critical Listening
- Visual Inspection
- Analyzing Metadata

### Audio Authentication
- The primary step in the analysis of an audio recording is to establish the authenticity of the recording. The forensic examiner verifies whether any alterations, such as additions, substitutions, or deletions, have been made to the recording.
<img width="560" height="191" alt="image" src="https://github.com/user-attachments/assets/0416d5eb-579f-481f-8c6e-9d543c18c17f" />

### Enhancement
- The quality of the audio evidence is not always good. Many times it is really difficult to recognize the speech in the recording due to the background noise and to resolve this issue, to understand what is being said, the enhancement of the audio recording is done.

### Interpretation
- After authentication and enhancement, the evaluation of the audio recording is done in order to understand and interpret the relevance of the audio to the investigation. It includes recognition of the speech (`speech recognition`), recognition of the speaker (`speaker identification`), and interpretation of background noise that can indicate the environment in which the audio was recorded

### Critical Listening
- If an edit is discovered during the critical listening phase, they are usually in the form of abrupt changes. Detecting these changes is not easy and comes with experience.
- Critical listening must be the first step to become familiar with the audio evidence.

### Visual Inspection
- Visually inspecting the audio wave form and spectrogram is the next step in authenticating the audio. This goes hand in hand with the electronic measurement as the forensic expert analyzes the physical wave properties and frequency information.
<img width="1047" height="342" alt="image" src="https://github.com/user-attachments/assets/ccdba13a-48bb-4fa3-8fe7-6af7f61f2989" />

### Analyzing Metadata
- Digital audio recordings contain metadata which reveals information about how the recording was made and the type of equipment that created the recording.
<img width="1466" height="417" alt="image" src="https://github.com/user-attachments/assets/1418c9bb-00e0-42d2-8d1d-b65e3f15b453" />

### Audio Evidence in Investigation Laboratory 
- Pre-Examination Assesment
  - Always request the `original recording` or `original device`.
    - If unavailable, request details of recording device: make, model, serial number; date, time of copying; details of copying process.
  - For telephone recordings, request `Call Detail Records` (CDR) for data verification like length of the recording, time, date and etc.
  - Maintain and check `Chain Of Custody` Documents (COD).
- Laboratory Examination
  - Judge Source i.e Direct or Telephonic Recording ?? 

| Factor | Telephonic Recording | Direct Recording | 
|---|---|---|
|Sampling Rate|8000 Hz|23000 Hz or more|
|Background Noise|Low|High|
|Metadata/Hex|[md5](https://md5file.com/calculator)||
<img width="1369" height="506" alt="image" src="https://github.com/user-attachments/assets/c964587d-ffbd-41a2-a85b-f6156151df97" />

### Speaker Identification/Recognition
<p align="center"><img src="img/SpeakerIdentification.png"></p>
- The process of automatically recognizing who is speaking on the basis of individual’s speech signals information.
- It is divided into two categories:
  - `Speaker Identification`: The task of determining an unknown speaker’s identity. (Speaker identification determines which registered speaker provides a given utterance from amongst a set of known speakers.)
  - `Speaker Verification`: With certain identity the voice is used to verify (Speaker verification accepts or rejects the identity claim of a speaker - is the speaker the person they say they are? )
> In forensic applications, it is suggested to first perform a speaker identification process to create a list of "best matches" and then perform a series of verification processes to determine a conclusive match

Why Speaker Identification ?
- Speaker Identification is essential for several criminal offences, such as making hoax calls to the police, ambulance or fire brigade, making threatening or harassing telephone calls, blackmail or extortion demands, or taking part in criminal conspiracies such as those involving the importation, trafficking or manufacture of illegal drugs etc.

What's Possibilities in Speaker Identification?
- Determine the speaker identity
- Selection b/w a set of known voices
- The user doesn't claim an identity
- `closed set identification`: the task of identifying an unidentified speaker within a known database.
  - Assume that all speakers are known to the system
- `Open set identification`: the task of identifying a known speaker within the unknown database.
  - Possibility that speaker is not among the speakers known to the system

Problems in Forensic speaker examination
- Recorded Samples
  - Noisy (SNR 5-6db or less)
  - Distorted/Damped & short duration
  - Non-contemporary
  - Disguised
  - Different texts
- Mode of Recording: Telephone, Cellular phone, Tape recorder, ....etc
> Noise ARE THE ENEMY OF THE SPEECH SAMPLE!

### Methods for Speaker Identification
- Auditory/Aural examination Method
- Spectrographic visual analysis method via
  - Computerized Speech Laboratory (CSL)
  - Multi-Speech
- Automatic Speaker identification System via
  - Text Independent Speaker Identification System (SPID)
  - Language Independent Speaker Identification System (LISIS)

### Audio Examination Tools
- Audio High-End Professional System
- Digitization Tools
  - Professional Audio System
- Pre analysis tools
  - Audacity, Adobe Audition, Praat, Hash Calc, Sonic Visualizer etc.
- Analysis Software
  - Computerized speech Lab, Multispeech etc.
  - Semi Automatic SPID

### Common facing Forensic Audio Cases
- Kidnapping for ransom
- Anonymous calls, threatening calls
- Obscene calls
- Drug peddling
- Sharing of vital information across the border
- Bribery
- Match fixing .... etc

### Visual Inspection Method
`Waveform Analysis`
- Visual comparison to spot discontinuities, sharp cuts, or faces that don’t match up.
- Difficult to detect if edits are made with technical precision (phase-aligned cutting).
- Human vs. synthesized/AI voice detection:
  - Human speech naturally exhibits variation; synthesized or programmatic voice segments show near-identical waveforms repeatedly.
<img width="1019" height="874" alt="image" src="https://github.com/user-attachments/assets/bf1eddff-c843-44b1-96e7-f6e0af07b3ce" />

`Spectrographical Analysis`
- Visualizes frequency content over time.
- Look for abrupt frequency changes or repeated patterns
- Sudden start/stop bands suggest edits or synthetic content
<img width="1158" height="828" alt="image" src="https://github.com/user-attachments/assets/0b6ba19f-e3db-4962-97db-d3f3c8b5c889" />

`Spectrogram Analysis`
<img width="1576" height="744" alt="image" src="https://github.com/user-attachments/assets/199516ad-faa0-418d-9a84-cd88b125cf45" />

`DC Shift Analysis`
- Measures whether the center line of the waveform is offset from zero.
- Large DC offset = improper recording or editing
<img width="1776" height="587" alt="image" src="https://github.com/user-attachments/assets/2df5d887-5855-4c80-b75b-362c6b6c32a2" />

`Statistical Parameters`
- Skewness, Kurtosis: indicate amplitude distribution shape
- SNR (Signal-to-Noise Ratio): higher = clearer audio

`Silence/Zero Discontinuity Detection`
- Checks for unnatural silences or zero blocks.
- Natural speech pauses differ from hard cuts or inserted silences

`LPC (Linear Predictive Coding) Discontinuity`
- Analyzes prediction changes over time.
- Discontinuities = possible splicing
- 'No discontinuity found' = likely original audio

`ENF (Electric Network Frequency) Variation`
- Checks continuity of 50Hz power line hum.
- Absence or sudden change may suggest manipulation

`Sampling Frequency Detection`
- Confirms audio sampling rate (e.g., 44.1kHz).
- Mismatch may indicate resampling or re-encoding
<img width="1588" height="625" alt="image" src="https://github.com/user-attachments/assets/0dd854f5-7120-4ff4-85ed-323c3be114fb" />

Specific Scenarios for Authentication & Appropriate Techniques
|Audio File Scenario|Techniques|Outcome|
|---|---|---|
|Original file on original device like mobile phone|Metadata, Hash|Conclusive authentication possible|
|File copied to another device, but original available like cd or pendrive with souce|Metadata, Hash, Auditory, waveform form, Spectrograph|String opinion possible|
|file only CD/drive, not social media processed|Metadata, Auditory, waveform-form, spectrography|continuity only|
|File from social media but present in device|Mostly Auditory, waveform form, Spectrograph|Only continuity possible|


## Video Forensic

[Check Fake/Real News](https://toolbox.google.com/factcheck/explorer)


## Image Forensic

Tools: Exif Metadata

### Image Editing Methods
- Compression
- Enhancing
- Re-touching
- Panoramas
- Inpainting
- Morphing
- Copy-Paste
- Copy-Move

### Image Foregery
- Aim: Fantasy/Fiction
- They fabricate an image to deceive the recipient into believing it's authentic, allowing them to secure payment and personal benefit.
- They produce an image intended to trick the recipient into believing it's genuine, enabling them to gain payment and fame.
- Three types of forgery can be distinguished:
  - An image created using graphic design software.
  - An image where the content has been altered
  - An image where the context has been altered
### Verification of Image Authenticity
- Image authentication involves maintaining the integrity of an image and verifying its original content.
- It is commonly used to establish and confirm the copyright ownership of the image.
- There are generally two main techniques.
  - Watermarking
  - Digital Signature
### How to Authenticate an Image
- Visual Inspection
- File Analysis
  - File Format & Structures
  - Metadata (EXIF)
  - Compression parameters (Quantization Tables)
- Global Analysis
  - Pixel & compressed data statistics
- Local Analysis
  - Finding inconsistencies of pixel statistics across the image

### Method of Image Authentication
<img width="892" height="467" alt="image" src="https://github.com/user-attachments/assets/f12c829e-0858-4ae9-a37b-711b628f8365" />

Watermark
<img width="1296" height="452" alt="image" src="https://github.com/user-attachments/assets/8a9637ea-1093-48af-8c21-cee397da419d" />

Digital Signature using Hashing Function
<img width="901" height="410" alt="image" src="https://github.com/user-attachments/assets/40568301-f2f4-4f0b-954f-856ea14c0232" />

### Image Manipulation Technique
- The methods for extracting image-related features can be divided into four categories:
  - `Pixel-based`
  - `Camera-based`
  - `Physical-based`
  - `Format-based`
<img width="718" height="393" alt="image" src="https://github.com/user-attachments/assets/3c6339c6-d5c2-49bd-9c51-233ae1a63f05" />

### Pixel based Method
- To examine pixel-level correlations from a particular type of tampering.
  - Duplicate regions detection
  - Resampling detection
- `Copy-Move Manipulation`
  - Algorithms have been created to identify cloned regions in images.
  <img width="816" height="517" alt="image" src="https://github.com/user-attachments/assets/caf40acb-c1d2-45d9-8318-c243ec4f6e03" />

  - DCT (Discrete Cosine Transformation)
    - in copy-move forgery, the copied region may be rotated and/or scaled to fit the scene better. it is used in DCT.
      <img width="777" height="385" alt="image" src="https://github.com/user-attachments/assets/d251cf62-7ff5-4cf6-a53a-26ac66ad4d28" />

  - PCA (Principle Component Analysis)
      <img width="1227" height="252" alt="image" src="https://github.com/user-attachments/assets/240d573e-e2f3-49bb-82b5-57f79eb8e79f" />

  - SIFT (Scale-Invariant Feature Transform)
    <img width="1035" height="613" alt="image" src="https://github.com/user-attachments/assets/690ac4d1-e6b0-43bc-97e0-7a72507fecd5" />
- `Image Splicing`:
  - a common technique in photographic manipulation involves digitally merging multiple images to create a single composite.
  - if splicing is performed, it will disrupt higher-order statistics, indicating signs of tampering.
    <img width="605" height="330" alt="image" src="https://github.com/user-attachments/assets/d7984073-9a18-41af-9e32-9fe48f635a34" />

  - an example of image splicing (A) and (B) the genuine images (C) the resulted.
- `Resampling`:
  - To create a composite, it is often necessary to resize, rotate or stretch parts of an image.
  - resampling introduces distinct periodic correlations b/w neighboring pixels.
  - this specific type of correlation can be easily identified.
    <img width="625" height="802" alt="image" src="https://github.com/user-attachments/assets/4e7b5b78-5c4f-469e-9edb-8c87c9152de2" />

    - Bilinear interpolation
    - Bayer Pattern
  - a tampered image often exhibits discrepacies in second-order differences along the horizontal direction.
    <img width="775" height="490" alt="image" src="https://github.com/user-attachments/assets/80895af5-01ae-4412-8b10-9d7aa8a9af82" />

### Image Analysis
- Multilevel wavelet decomposition consists of the following: (a) single level components specification, (b) two-level components specification, (c) discrete wavelet transform (DWT) single level, and (d) DWT two-level decomposition. LH-vertical; HL-horizontal; HH-diagonal detail.
<img width="433" height="465" alt="image" src="https://github.com/user-attachments/assets/f1a26677-b432-43c5-881a-7a28dc1b372f" />



### Camera Ballistics
- Which device has created this picture ?
- example: Forensic analysis of a smartphone: which pictures have been generated on the device and which ones have been generated by other devices and sent by messaging application or saved from the internet.
- we can identify:
  - Type of Devices
  - Maker & Moodel
  - Specific exemplar
    - Source Identification
    - Manipulation Detection
- DIGITAL FINGERPRINTS of Camera
  - `In-camera fingerprints`: Every part of the device that captures the image, such as the lens, color sensor, and camera software, leaves its own unique imprint on the final image.
  - `Out-camera fingerprints`: Any processing applied to the digital media after it's captured, like editing or compression, changes its characteristics (e.g., statistical or geometric features), leaving distinct traces.
  - `Scene (geometric) fingerprints`: Real-world elements in the image, like lighting conditions or reflections, have specific features that help describe the scene, such as the direction of light or reflections in the eyes.
- Utilization of DIGITAL FINGERPRINTS
  - for source identification
    - Digital fingerprints are extracted from the media and matched against a database of fingerprints unique to each type, brand, or model of device used to capture the content.
  - for forgery detection
    - Identify inconsistencies or missing fingerprints in the media, which may indicate tampering.
    - Look for fingerprints that reveal specific edits or post-processing applied to the content.
- Features Derived from Camera
  - Methods for modeling and estimating various camera artifacts.
    - Every camera component imparts its unique characteristics to the resulting image.
    - These characteristics can be used as evidence to determine the source camera.
    - Discrepancies can serve as evidence of tampering.

### Camera Architecture
- this necessitates an understanding of the image formation process in a digital camera.
- the fundamental design of a digital camera.
<img width="1180" height="400" alt="image" src="https://github.com/user-attachments/assets/29e5e157-2770-4e34-8ce3-929c4a6077ab" />

### Digital Camera Structure
- The camera lens directs light onto a flat surface made up of tiny, light-sensitive points known as a “CCD” or “CMOS” sensor.
- The tiny sensors are struck by light particles (photons) and turn them into electrical signals. These signals are then processed by an A/D converter, which transforms them into digital data.
- Before the light hits the sensor, it goes through a Colour Filter Array (CFA), which splits the light into different colors, such as red, green, and blue, allowing the camera to capture color details.
<img width="1432" height="314" alt="Screenshot 2026-10-05 195619" src="https://github.com/user-attachments/assets/0d8bf18c-0ad2-472d-88d2-453f82fbab9c" />

Features Derived from Camera
- Lens aberrations
  - the camera's lenses introduce various aberrations into the resulting image.
- Sensor pattern noise
  - pixel-to-pixel variations when the sensor array is not exposed to light.

### Lens Radial Distortion
- Radial lens distortion correction using cascaded one-parameter division model
  - Corrected results of ours and the results using the method in [1]: Images in the first column are source images. The middle column are rectified results using the method in [1]. The images depicted in the last column are our automatically corrected results.
<img width="696" height="615" alt="image" src="https://github.com/user-attachments/assets/1218a5ee-398e-4faa-ab5c-be7105aaa7a0" />
- Background of Lens Radial Distortion
<img width="1222" height="492" alt="image" src="https://github.com/user-attachments/assets/470876ad-b8a5-4c43-88f2-6b33b84ebad4" />
- Analysis of Lens Radial Distortion at Different Camera
<img width="567" height="272" alt="image" src="https://github.com/user-attachments/assets/e8683966-693a-40ee-b2b4-cd6357be4697" />

<img width="1263" height="841" alt="image" src="https://github.com/user-attachments/assets/bdd075aa-732d-452e-bedd-dd16d1e794d2" />

<img width="1368" height="848" alt="image" src="https://github.com/user-attachments/assets/334e1c9c-3465-4b35-a649-b24bbb74c3e1" />

- Behaviour of lens radial distortion parameter k1 across the image for various cameras at different zoom levels.
<img width="688" height="782" alt="image" src="https://github.com/user-attachments/assets/d3cc8ef6-a3e0-4e1f-8fa9-43d991db76e7" />

### Sensor Defect Noise
<img width="710" height="190" alt="image" src="https://github.com/user-attachments/assets/3dc13965-c214-427c-8bd2-7ef16a893c1e" />

- Sensor noise consists of two primary components:
  - Fixed Pattern Noise (FPN) refers to
    - Variations b/w pixels when in low-light conditions.
    - Added noise that affects the image.
  - Photo-Response Non-Uniformity (PRNU) is
    - the primary source of pattern noise.
    - Variability in pixel response to light, resulting in multiplicative noise.

Photo Response Non-Uniform (PRNU) Sound
- The PRNU of the source camera can be regarded as the device's unique identifier, similar to a human fingerprint.
- PRNU analysis is most commonly employed to determine the source of a digital image.
- The PRNU pattern can also reveal if a digital image has been altered.
<img width="1897" height="507" alt="image" src="https://github.com/user-attachments/assets/0ef81e5d-8d26-459c-9288-8ff06bf7aa00" />

Sensor Anomaly: FPN
- Fixed Pattern Noise (FPN) refers to the variations between pixels when the sensor is in darkness and not receiving any light.
- In many digital cameras, this variation is corrected by subtracting a dark frame (mask) from the captured image.
<img width="1042" height="298" alt="image" src="https://github.com/user-attachments/assets/94ea77f2-8173-406f-8b9e-36aef4af4207" />

Sensor Defect: PRNU
- A digital camera usually contains a 2D grid of millions of CCDs, with each CCD dedicated to capturing data for one individual pixel.
- A CCD is often likened to a bucket that gathers rain (photons) until it fills to a specific level, representing the pixel value.
- In an ideal situation, when even light illuminates a camera sensor, every pixel should produce the same output value.
- In practice, slight differences in cell size and the materials used for the substrate lead to minor variations in output values.
<img width="1172" height="277" alt="image" src="https://github.com/user-attachments/assets/0c87b923-93a4-4946-b399-c6f4608b8f12" />

### Illumination Inconsistences
- The amount of light striking a surface is proportional to the angle between the surface normal and the direction of the light source.
- By knowing the 3D surface normals, the direction of the light source can be estimated.
- This method relies on intensity gradients across the surface of an object.
- The gradient distribution can reveal the light sources in the image.
- Illumination inconsistencies can be used for revealing traces of digital tampering.
<img width="947" height="720" alt="image" src="https://github.com/user-attachments/assets/f46b7158-863d-4bcb-94c1-f336c7100ab5" />

### Format-based Method
- As JPEG is the most widely used image format
  - The technique for detecting tampering addresses the JPEG Lossy compression s
  - The distinct characteristics of lossy compression can be leveraged for forensic analysis scheme.
  - The JPEG image encoding (compression) process involves three fundamental steps.
  - Discrete cosine transform (DCT): An image is initially divided into 8x8 blocks, and each block is transformed into the frequency domain using a 2D DCT.
  - Quantization: The DCT coefficients are divided by a quantization table and then rounded to the nearest integer.
  - Entropy coding: Lossless entropy coding of the quantized DCT coefficients (e.g., Huffman coding).

### Error Level Analysis
- ELA highlights differences in the JPEG compression rate.
- It helps to detect regions within the image that have been compressed at different levels, which might indicate editing or manipulation
- Normally, a JPEG image should have a uniform compression level, as errors are spread evenly across the image.
- ELA works by calculating the average differences in the quantization tables of pixel blocks throughout the image, highlighting areas that deviate from the expected compression pattern.
<img width="631" height="792" alt="image" src="https://github.com/user-attachments/assets/80cc5f7e-3d2e-427e-8d7d-7b6f3cc7d7a1" />




## Text Forensic





