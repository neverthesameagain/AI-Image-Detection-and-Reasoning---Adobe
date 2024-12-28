# General Approach for PS
## Task 1
Inorder to classify the images into "real" and "fake" we train a custom model made originally to detect deepfakes. We retrain it on real and fake datasets which contain random perturbations on a fixed amount of images. These images are randomly chosen from the initial dataset.

The steps to test this methodology is available in the "README.md" file in the "Task1" directory.
___
## Task 2
Our approach to generate explainations on fake images is initially the images are passed through a filter that utilizes clip toretreive the type of artifacts present in the image.Then we use a VLM (Qwen2-VL-7B) and pass prompts specifically tailored to thetype of artifacts detected in the image so that appropriate explainations are generated.

The steps for testing this method is available in the "README.md" file in the "Task2" directory.
___