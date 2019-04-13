
3D bounding box visualization using open3D
=====
#### This repository is the visualization of 3D Bounding Box in Point Clouds using open3D library.

- Install open3D Library
```
pip install open3d-python
``` 

- Please first run [view_point_experiment.py](https://github.com/kangningLi/visualization/blob/master/view_point_experiment%20.py "view_point_experiment.py") to adjust your view point based on your monitor and preference. This file will generate a json file to represent the view parameter, please replace the json file in [video_generator.py](https://github.com/kangningLi/visualization/edit/master/video_generator.py "video_generator.py").

- In order to direct use this code, please change your label file to the same format of KITTI dataset. Or modifiy the function in [helper_functions.py](https://github.com/kangningLi/visualization/blob/master/helper_functions.py "helper_functions.py") and [vis_utils.py](https://github.com/kangningLi/visualization/blob/master/vis_utils.py "vis_utils.py").

- Run [vis_train_val.py](https://github.com/kangningLi/visualization/blob/master/vis_train_val.py "vis_train_val.py") to get your required output. Need to set the correct path in the code.
1. image_with_gt_2d_bbox： Draw 2d ground truth bounding box into images
2. image_with_3d_bbox : Draw 3d bounding box into images
3. image_for_point_cloud_wo_bbox : Raw point cloud images
4. image_for_lidar_with_3d_bbox : Draw bounding box into 2d bird eye view images
5. image_for_point_cloud : Point Cloud with 3d bounding box

- [Parameter.py](https://github.com/kangningLi/visualization/edit/master/parameter.py "Parameter.py") contains all the necessary parameters when generating output images.

- Example output video please see:  https://youtu.be/7IUUmFAFa-A
