# UnmannedRetail-PickReturn-Dataset
## **Overview**
![scenarios](https://github.com/user-attachments/assets/0165e490-f787-40f6-a5d2-921704f4a38b)
UR-PRD is a dataset designed for action recognition in unmanned retail environments. It includes **2,103 labeled action instances** across three categories:

- **Item Pickup**: Actions where an item is successfully picked up.
- **Item Return**: Actions where an item is returned to the shelf.
- **Other Action**: Actions that do not fall into the above two categories.

These instances were extracted from recorded videos, with each instance spanning **1 to 10 seconds**, resulting in a total of **101,830 annotated frames**.

To protect privacy, only **Skeleton Data** and **Hand Images** are publicly available.
Each sample in the dataset is stored in **HDF5 (`.h5`) format**, containing:

- **Skeleton Data**: Keypoint coordinates extracted from human body joints.
- **Hand Images**: Cropped hand images corresponding to item pickup and return actions.

## **Scenarios**
UR-PRD is designed to capture real-world challenges in unmanned retail through five scenarios:

1. **Normal**: Includes all actions with minimal occlusion, varying lighting, and different viewpoints.
2. **Occlusion**: Cases where hands or items are partially blocked.
3. **Small Items**: Features smaller, harder-to-detect items.
4. **Err-Pickup**: Instances where a user attempts a pickup but does not successfully hold the item.
5. **Err-Return**: Instances where a user attempts to return an item while still holding it.

## **Train-Test Split**
To ensure robust evaluation, the dataset is divided as follows:

- **Normal, Occlusion, and Small Items**: 80% for training, 20% for testing.
- **Err-Pickup and Err-Return**: Exclusively allocated to the test set to rigorously assess generalization.

## **Dataset Link**
train_data.h5
link：https://pan.baidu.com/s/1s48FTeJt8MaHBmIYFCW06w?pwd=ky17 
extraction code：ky17

test_data.h5
link：https://pan.baidu.com/s/1INdDQg7sD6_kKNN51W7dLA?pwd=ky17 
extraction code：ky17


## **Usage**
Researchers can leverage UR-PRD for **multi-modal action recognition** using both skeleton-based and vision-based models. The dataset is particularly useful for studying fine-grained hand-object interactions in retail environments.

