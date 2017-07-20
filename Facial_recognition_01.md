# How facial recognition works

## What is facial recognition

**A face recognition system is a computer application capable of identifying or verifying a person from a digital image or a video frame from different sources.**
One of the ways to do this is by comparing selected facial features from the image and a face database.

It is typically used in robotics and in security systems and can be compared to other biometrics such as fingerprint or eye iris recognition systems.
It has also become popular as a commercial identification and marketing tool.

## The process of facial recognition

The process of facial recognition has three main phases:

* **Face detection and face representation**: Find the face or faces in the photo, and create a representation (also known as face signature).

* **Model training**: convert several examples of a person's face into a single model.

* **Recognition**: compare a face representation to the models of a list of candidate identities.

### Face detection

Many confuses this with face recognition.
**Detection** is the process of finding the face, recognition is the process of finding whom the face belongs to.
Face detection involves passing a sliding window of various sizes across the image, each time trying to answer the question "is there a face at this size at this position".
This step involves an initial quick filtering stage, that will result in a fairly large number of candidate faces, and a following step that will run a test on each candidate face to confirm it's a face.

Once a face is detected, the system needs to extract a face signature.
Facial recognition systems are aligning the faces before extracting the face signature as it makes the face signature better.
**Aligning** is the process of rotating and scaling the face in order to bring all of the key features into the same places (eyes, nose, mouth etc).

**Representing the face is probably the most important step in facial recognition**.
The face is represented as a vector of floating point numbers, where the meaning of each number depends on the representation itself.
The best representation can be generated using a neural network.

### Model training

Model training is the process of taking several face representations belonging to the same person, and creating a classifier that can recognize more examples of face representation from the same person.
The most popular approach is to use a linear SVM.

### Recognition

Given a new face representation and a list of candidate identities, recognition will compare the face models of the identities with the new face representation and will generate a score for each one.
The score if passing a certain threshold is an indication of a recognition.
This is a fast operation, and depending on the size of the representation - recognition systems can obtain scores for millions of candidates per second.

(Source: [Wikipedia](https://en.wikipedia.org/wiki/Facial_recognition_system), [Quora](https://www.quora.com/How-does-the-facial-recognition-technology-work))

adding an extra paragraph
