some random extra text I added

## Techniques for face acquisition

### Traditional

Face recognition algorithms identify facial features by extracting landmarks, or features, from an image of the subject's face.
For example, an algorithm may analyze the relative position, size, and/or shape of the eyes, nose, cheekbones, and jaw.

![Facial recognition markers (picture: Extreme Tech)](/assets/pictures/01_markers.jpg)

*Facial recognition markers*

These features are then used to search for other images with matching features.
Other algorithms normalize a gallery of face images and then compress the face data, only saving the data in the image that is useful for face recognition.
A probe image is then compared with the face data.
One of the earliest successful systems is based on template matching techniques applied to a set of salient facial features, providing a sort of compressed face representation.

Recognition algorithms can be divided into two main approaches:

1. **geometric**, which looks at distinguishing features, and

2. **photometric**, which is a statistical approach that distills an image into values and compares the values with templates to eliminate variances.

Popular recognition algorithms include principal component analysis using eigenfaces, linear discriminant analysis, elastic bunch graph matching using the Fisherface algorithm, the hidden Markov model, the multilinear subspace learning using tensor representation, and the neuronal motivated dynamic link matching.

### 3-dimensional recognition

A newly emerging trend, claimed to achieve improved accuracy, is three-dimensional face recognition.
**This technique uses 3D sensors to capture information about the shape of a face.**
This information is then used to identify distinctive features on the surface of a face, such as the contour of the eye sockets, nose, and chin.

![Biometric facial recognition (picture: Quora)](/assets/pictures/02_biometric.jpg)

*Biometric facial recognition*

One advantage of 3D face recognition is that it is not affected by changes in lighting like other techniques.
It can also identify a face from a range of viewing angles, including a profile view.
Three-dimensional data points from a face vastly improve the precision of face recognition.
3D research is enhanced by the development of sophisticated sensors that do a better job of capturing 3D face imagery.
The sensors work by projecting structured light onto the face.
Up to a dozen or more of these image sensors can be placed on the same CMOS chip, each sensor captures a different part of the spectrum.

Even a perfect 3D matching technique could be sensitive to expressions.
For that goal Teal Robotics applied tools from metric geometry to treat expressions as isometries.

A new method is to introduce a way to capture a 3D picture by using three tracking cameras that point at different angles; one camera will be pointing at the front of the subject, second one to the side, and third one at an angle.
All these cameras will work together so it can track a subject's face in real time and be able to face detect and recognize.


(Source: [Wikipedia](https://en.wikipedia.org/wiki/Facial_recognition_system), [Extreme Tech](https://www.extremetech.com/extreme/178777-facebooks-facial-recognition-software-is-now-as-accurate-as-the-human-brain-but-what-now) - 1st picture, [Quora](https://www.quora.com/How-does-the-facial-recognition-technology-work) - 2nd picture)
