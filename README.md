# Dataset: PIGRGB-Weight

## Dataset Overview
This dataset consists of two parts: RGB_9579 and RGB_MASK_3394.
- The **RGB_9579** dataset contains RGB images of pigs' backs taken at a height of 1.88 meters in a free-ranging state.
- The **RGB_MASK_3394** dataset contains RGB images of pigs' backs taken at a height of 1.78 meters, along with corresponding manually labeled mask images.

## Complete data download address:
Link: https://pan.baidu.com/s/13uHbg-_B3-EaJFVanqYY9A?pwd=mawh
Password: mawh or https://drive.google.com/drive/folders/1DiVtsBbE9egLa4imoNzBLPDtUMKYHkJk?usp=sharing

Both datasets include weight annotations for the pigs, providing support for research on pig weight estimation. The **RGB_9579** dataset is used for image feature extraction and weight prediction model training, while the **RGB_MASK_3394** dataset is useful for studies involving mask image processing.

## Dataset Structure
**PigRGB-Weight**
PigRGB-Weight/
    ├── RGB_9579/
    │   └── fold1/
    │       └── 73.36_124/
    │           └── 73.36kg_1.png
    ├── RGB_MASK_3394/
    │   ├── MASK_3394/
    │   │   └── 33.1_34/
    │   │       └── 33.1kg_1.png
    │   └── RGB_3394/
    │       └── 33.1_34/
    │           └── 33.1kg_1.png


- **RGB_9579**: Contains 9579 RGB images taken at 1.88 meters in height, with weight annotations in PNG format.
- **RGB_MASK_3394**: Contains RGB images and corresponding mask images, taken at 1.78 meters in height. The image naming convention includes weight information (e.g., "33.1kg" indicates the pig's weight is 33.1kg).

### Directory Structure Explanation
- **RGB_9579**: This subdirectory contains a total of 9579 RGB images.
- **fold1**: A subset of the dataset, used for cross-validation or other purposes.
- **73.36_124**: This subset indicates the weight range (e.g., 73.36kg to 124kg) and dataset numbering.
- **33.1_34**: This subset indicates the weight range (e.g., 33.1kg to 34kg) and dataset numbering.
- **Mask images**: Each image has a corresponding mask image in the MASK_3394 directory, matching the RGB image filenames and containing the areas of interest (such as the pig's back and contour).

## Dataset Contents
- **RGB images**: Each PNG image corresponds to a pig's back image, captured when the pig is freely active.
- **Mask images**: Each RGB image has a corresponding manually labeled mask image, indicating the region of interest.

## Behavioral States
The dataset includes the following pig behavioral states:
- **Stand Upright**: The pig is standing upright, supporting its body with all four limbs, maintaining an upright posture.
- **Feeding**: The pig is feeding, typically observed foraging or eating from a food trough.
- **Walking**: The pig is walking, moving within an activity area with limbs alternating in a regular, rhythmic pattern.
- **Drinking**: The pig is drinking water, shown by the pig lowering its head toward a water source.
- **Standing Abnormally**: The pig is standing in an abnormal posture, with its body twisted or in an irregular stance.
- **Standing with Head Down**: The pig is standing while lowering its head, with its body still standing but its head lowered.
- **Partially Obscured Multiple**: Multiple pigs are present in the image, but parts of their bodies are obscured or incomplete due to the viewing angle or obstruction from other pigs or objects.
- **Fully Visible Multiple**: Multiple pigs are fully visible in the image, with no occlusion or distortion.

## Usage Instructions
1. After downloading the dataset, you can directly load these PNG images.
2. Each image’s weight data is provided in the image's annotation, with weight in kilograms (kg).
3. This dataset can be used for pig weight estimation tasks, including machine learning model training and testing.

## License
This dataset is publicly shared for research purposes in machine learning and image processing. Please cite the relevant research when using this dataset.

## Notes
1. The images in this dataset are all RGB images, and the filenames include weight annotations.
2. Users can choose different subsets for training and validation based on their needs.
3. The pigs' weight range in the dataset is from 33.1kg to 192kg.
