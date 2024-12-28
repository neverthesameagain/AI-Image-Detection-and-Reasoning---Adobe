# **Adobe Mid Prep Problem Statement**

### Image Classification and Artifact Identification

---

###### Task 1 - Image Classification

1. Go to the sub folder task1 .

```
cd 41_code_m3_adobe/task1/binary_deepfake_detection-main
```

2. Install the Requirements

```
!pip install requirements.txt
```

3. Place the location of test dataset at:
   configs/results_cifake_T_unfrozen.cfg

   `cifake_path: final_test`
4. If you want to check wether the images are real or fake , place all your test images (Both real and fake regardless of being fake or real) in `final_test/test/REAL`
5. Run the test script:

```
 python3 test.py 
```