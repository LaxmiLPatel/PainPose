# PainPose

## Android App for Pain Position Image Classification based on TensorFlow v2

This is an Android app for classifying pain position in an image stream, using a classifer model, built by using TensorFlow v2, MobileNet pre-built model, and some images grouped by pain positions.

It can continuously classify image frames received by the Android device's back camera. Inference is performed using the TensorFlow Lite Java API.

It allows the user to choose between a floating point or quantized model, select the thread count, and decide whether to run on CPU or GPU.

## Requirements

- A computer with Android Studio 3 or greater

- Android phone or tablet with Android 4 or greater

## Method of Building the App

- On a computer, in some folder X, crate PainImages folder.

- In the PainImages folder, create subfolders named: Abdomen pain, Back pain, Chest pain, Chin pain, Ear pain, Elbow pain, Eye pain, Fingers pain, Foot pain, Hand pain, Head pain, Hip pain, Knee pain, Leg pain, Mouth pain, Neck pain, Nose pain, Thigh pain, Thumb pain, Toe pain, Wrist pain, Zero pain.

- In each of these subfolders, place some images corresponding to the subfolder name.

- From TensorFlow examples GitHub repository, download make_image_classifier.py file into folder X.

- Open Windows Command Prompt, and move to folder X.

- Run the following code:

- python make_image_classifier.py --image_dir PainImages --tfhub_module https://tfhub.dev/google/tf2-preview/mobilenet_v2/feature_vector/4 --saved_model_dir model --labels_output_file labels.txt --tflite_output_file model.tflite  --train_epochs 10

- This will generate labels.txt and model.tflite files in folder X.

- In Android Studio, create PainPose app.

- Use the above labels.txt and model.tflite files as assets in the Android app.

- Make necessary chnages in the app.

## References

- [TensorFlow Lite image classification overview](https://www.tensorflow.org/lite/models/image_classification/overview)

- [TensorFlow Lite image classification Android app example](https://www.tensorflow.org/lite/models/image_classification/android)

- [TensorFlow examples GitHub repository](git clone https://github.com/tensorflow/examples)

- [Android device in developer mode](https://developer.android.com/studio/debug/dev-options)
