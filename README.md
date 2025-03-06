# UnmannedRetail-PickReturn-Dataset
## **Overview**
UR-PRD is a dataset designed for action recognition in unmanned retail environments. It includes **2,103 labeled action instances** across three categories:

- **Item Pickup**: Actions where an item is successfully picked up.
- **Item Return**: Actions where an item is returned to the shelf.
- **Other Action**: Actions that do not fall into the above two categories.

These instances were extracted from recorded videos, with each instance spanning **1 to 10 seconds**, resulting in a total of **101,830 annotated frames**.

## **Data Format**
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
Our dataset is available at: [Insert Dataset Link Here]

## **Usage**
Researchers can leverage UR-PRD for **multi-modal action recognition** using both skeleton-based and vision-based models. The dataset is particularly useful for studying fine-grained hand-object interactions in retail environments.
![introduction](https://github.com/user-attachments/assets/a4a5073a-9734-4e2a-9dd2-fe23a0e57a62)

