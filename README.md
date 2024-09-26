# Brain-CT-image-hemorrhage-segmentation-XN-Project
The Zeta Surgical company was started by a team of Harvard graduates and academics. The mission is to democratize access to accurate, safe, and fast image guidance, to unlock the use of image guidance directly at the point of care, and to enable new treatments in cases such as emergencies and bedside procedures.


In this project, the company provides us with a dataset consisting of various brain CT scan slices, each of which has a hemorrhage (bleeding) within it. The hemorrhages have been labeled in some of the images. These hemorrhages are divided into different types:  intraparenchymal, intraventricular, subarachnoid, subdural, epidural, and category for images with multiple sources of bleeding. We will use techniques in machine learning, computer vision, user interface, and data analytics to classify, regression, and segment these CT images.

Deliverable:  We will develop mathematical models, apply machine learning and artificial neural network techniques, and develop a program using Python and TensorFlow to investigate the labeled dataset.  The goal of the project is to complete the machine learning model with Python scripts for classification, regression, and, more importantly, the segmentation of brain hemorrhage in CT images.

Data: Here are the data except for the original CT images. 

https://northeastern-my.sharepoint.com/:f:/g/personal/he_wang_northeastern_edu/EodLanXAcDxImt-4t2qjkJIBxdO0zzBDr7ONcvVduPSu7wLinks to an external site. 

The dataset itself consists of various brain CT scan slices, each of which has a hemorrhage (bleeding) within it. These hemorrhages are divided into different types, as according to the table below: (some of the slices contain multiple hemorrhages in them, and we have a 6th category for images with multiple sources of bleeding. ) 

![image](https://github.com/user-attachments/assets/238f9dc6-ec6b-4746-a553-3ded2a02802b)

Data is saved in the following folders:
dcms/
    hemorrhage-labels.csv
    renders/
        epidural/
            ...
        intraparenchymal/
            ...
        intraventricular/
            ...
        multi/
            ...
        normal/
            ...
        subarachnoid/
            ...
        subdural/
            ...
Where each of the bottommost level directories has 4 subdirectories within (brain_bone_window, bone_window, max_contrast_window, subdural_window) for the different rendering types for each hemorrhage. CT windowing allows us to render the CT scan using different values of density, and some window methods make it easier to see a hemorrhage than others do.   The raw dicom files for the CT scans into the dcms/ subfolder. The normal/ folder contains images without any hemorrhaging, while the multi/ folder contains images with multiple hemorrhages.


