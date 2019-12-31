# PainPose

## Pain Position IMage Classification Android App

This is an Android app for classifying pain position in an image stream, using a classifer model,
built by using TensorFlow v2, MobileNet pre-built model, and some images grouped by pain positions.

It can continuously classify image frames received by the Android device's back camera.
Inference is performed using the TensorFlow Lite Java API.

It allows the user to choose between a floating point or quantized model,
select the thread count, and decide whether to run on CPU or GPU.

## Requirements

- A computer with Android Studio 3 or greater

- Android phone or tablet with Android 4 or greater

## Method of Building the App

...

## References

- [TensorFlow Lite image classification overview](https://www.tensorflow.org/lite/models/image_classification/overview)

- [TensorFlow Lite image classification Android app example](https://www.tensorflow.org/lite/models/image_classification/android)

- [TensorFlow examples GitHub repository](git clone https://github.com/tensorflow/examples)

- [Android device in developer mode](https://developer.android.com/studio/debug/dev-options)