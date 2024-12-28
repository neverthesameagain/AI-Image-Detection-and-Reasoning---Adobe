# How to test Task 2 solution
## Overview of Testing Methods
* **Automatic pipeleline** : A pipeline has been implemented that will save all images classified as fake to a directory and automatically generates the explanations 
* **Script based** : By running a script on a directory containing fake images so that explanations can be generated on it.
## Prerequisites
Install required python modules by running the below code in the terminal.

```
pip install -r requirements.txt
```
## How to perform Script based testing
1. Prepare the image directory
    * Place all the images you want in a single directory
    * Images of all formats are supported
2. Update the script
    * In the test script replace the image_dir variable with the directory location of which you want to generate explainations.
        ```python
        image_dir = "path_to_your_image_directory"
        ```
3. Run the script
4. View the results
    * The explainations will be saved in "testing_fake.json" in the same directory as the script
    * Each image analysis will include
      * Image name (without extension)
      * The detected artifacts and the corresponding explanations

    * Results will be saved in the json file in the following format format
        ```json
        [{"index": 2,
        "explanation":
        {"<artefact name 1>": "<explanation>",
        "<artefact name 2>": "<explanation>", ...},
        ...]
        ```