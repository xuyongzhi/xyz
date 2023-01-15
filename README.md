## Yongzhi Xu

# Dense 3D reconstruction using mobile phone

| <img width = 600/> Input video | <img width = 600/> Multi-view stereo reconstruction | <img width = 600/> 3D scene understanding |
| :-----| :----: | :----: |
| <img width = 600/> ![MVS_AULab](resources/MVS/office.gif)  | <img width = 600/>  ![MVS_AULab](resources/MVS/AU_Lab_Office_mesh.gif)   | <img width = 300/>  ![RoomPlan](resources/MVS/roomplan_aulab.gif)  |


# AR (Augmented reality) Cloud 

Similar with:   
![AR_SNap](resources/SnapAR.gif)

## Structure from motion (SFM) of 3D line map

Key contributions:
1. A novel 3D mapping pipeline.   
2. Multi-view triangulation using Plucker representation.   
3. No Manhattan assumption

| <img width = 1000/> High-precision map for AR | <img width = 1000/> The pipeline of proposed 3D line mapping approach.|
| :-----| :----: |
|  ![AR_HR_Map](resources/AR_Map.PNG)  | <img width = 1000/>  ![BJF_3D_Lines](resources/line_mapping.jpg)  |
|![Tri](resources/LineSFM/Line_Tri.png) | ![Tri](resources/LineSFM/LineMat.png) |



| |<img width = 1000/>   |  <img width = 1000/> |
| ----------- |  ----------- | ----------- |
| 3D point cloud | ![BJF_Points1](resources/BJF_Points_1.gif) | ![BJF_Points2](resources/BJF_Points_2.gif)      |
| 3D line cloud |  ![BJF_3D_Lines](resources/BJF_LineSFM.gif) | ![BJF_3D_Lines](resources/BJF_3D_lines.gif)   |
| Reprojections | ![rep_lines_A](resources/project_lines_A.gif) | ![rep_lines_A](resources/project_lines_B.gif) | 


## Visual positioning system combining features of point and line  
Key contributions: 
- A novel geometric & descriptor fused line matching approach based on coarse VPS pose.

| <img width = 1000/> VPS (Visual Positioning Service) | <img width = 1000/> The pipeline of proposed line-based pose verification & refinement.|
| :-----| :----: |
| ![VPS](resources/VPS.gif) |![BJF_3D_Lines](resources/Poine_Line_VPS.png)|
|  |![JcASL_MAT](resources/NL_JcASL_Line.gif)|

![JcASL_MAdT](resources/SegJuncMat.gif)

## 3D surface detection from a single view  

Multiple 3D surfaces are detected from a single view.
- No Manhattan assumption
- Unknown camera models 
- 3D normal accuracy > 97% in real world images (around 60% accuracy achieved by SOTA learning and handcrafted methods.)
![Surface3D](resources/3D_surfaces.gif)

### Wrap virtual materials on the 3D surfaces:  

| | |
| :-----| :----: |
|<img width = 1000/> 1. Fully automated and real-time generation of multiple 3D planes from a single view. <br> 2. The layout of multiple planes are optimized based on the scores and distribution of 3D planes.  | <img width = 1000/> ![Surface3D](resources/Cyberpunk.gif)|


## Scan-to-BIM  
- Input: registered point cloud
- Output: building information models (BIM), which are 3D objects with semantic and structural information.
![BIM](resources/BIM/scan_to_BIM.png)

### FloorDet  

| <img width = 1000/> | <img width = 1000/> |
| :-----| :----: |
| ![](resources/BIM/FloorDet_1.png) | ![](resources/BIM/FloorDet_2.png)  |
| ![](resources/BIM/FloorDet_res1.png) | ![](resources/BIM/FloorDet_res2.png)  |
| ![](resources/BIM/FloorDet_res3.png) | ![](resources/BIM/FloorDet_res4.png)  |

### CorDet  

| <img width = 1000/> | <img width = 1000/> |
| :-----| :----: |
| ![](resources/CorDet/CorDet_1.png) | ![](resources/CorDet/CorDet_2.png)  |
| ![](resources/CorDet/CorDet_res1.png) | ![](resources/CorDet/CorDet_res2.png)  |
| ![](resources/CorDet/CorDet_res3.png) | ![](resources/CorDet/CorDet_res4.png)  |
