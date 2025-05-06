How the Viola–Jones Algorithm Works
The Viola–Jones object detection framework is a machine learning-based approach used for real-time face detection. It was introduced by Paul Viola and Michael Jones in 2001 and is one of the earliest successful algorithms for face detection in images.

📌 Key Steps of the Algorithm:
Haar-like Features:

The algorithm uses simple rectangular features similar to Haar wavelets (like edge, line, and center-surround patterns).

These features are used instead of raw pixel values to make detection faster.

Integral Image:

An intermediate representation of the image that allows fast computation of Haar features at any scale or location in constant time.

AdaBoost (Learning Algorithm):

A boosting algorithm is used to select the most important features from thousands of Haar features.

It combines several weak classifiers into a strong classifier for more accurate detection.

Cascade of Classifiers:

Instead of applying all features to every window, the algorithm uses a cascade structure.

Early stages quickly reject non-face regions, while later stages focus only on promising face-like areas.

This makes the detection both fast and efficient.

⚙️ Advantages:
Very fast and suitable for real-time applications.

Works well for frontal face detection.

⚠️ Limitations:
Not robust to large rotations or extreme lighting conditions.

Less accurate compared to modern deep learning-based methods.
