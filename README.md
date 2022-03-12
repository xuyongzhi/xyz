## Yongzhi Xu

## Structure from motion (SFM) of 3D line map

| <img width = 1000/> Key contributions | <img width = 1000/> The pipeline of proposed 3D line mapping approach.|
| :-----| :----: |
|   1. A novel 3D mapping pipeline. <br> 2. Multi-view triangulation using Plucker representation. <br> 3. No Manhattan assumption | <img width = 1000/>  ![BJF_3D_Lines](resources/line_mapping.jpg)  |


| |<img width = 1000/>   |  <img width = 1000/> |
| ----------- |  ----------- | ----------- |
| 3D point cloud | ![BJF_Points1](resources/BJF_Points_1.gif) | ![BJF_Points2](resources/BJF_Points_2.gif)      |
| 3D line cloud |  ![BJF_3D_Lines](resources/BJF_LineSFM.gif) | ![BJF_3D_Lines](resources/BJF_3D_lines.gif)   |
| Reprojections | ![rep_lines_A](resources/reprojected_3D_lines/rep_lines_A.gif) | ![rep_lines_A](resources/reprojected_3D_lines/rep_lines_B.gif) |

## Visual positioning system combining features of point and line  

| <img width = 1000/> Key contributions | <img width = 1000/> The pipeline of proposed line-based pose verification & refinement.|
| :-----| :----: |
|A novel geometric & descriptor fused line matching approach based on coarse VPS pose. |![BJF_3D_Lines](resources/Poine_Line_VPS.png)|

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
