# Yongzhi
Computer vision researcher and engineer with 5 years’ academic and 4 years’ industry experience. I have
developed several popular products on TikTok and CapCut at ByteDance. I am currently working on 3D
reconstruction and scene understanding as the team lead of mixed reality (MR) group in Tencent XR AU-Lab.
I love coding and have been programming using C++ and python for around 9 years. I am passionate on
pursuing excellence, embracing challenges, enjoying work with others, learning new things along the way.

# Dense 3D reconstruction and scene understanding for VR headset 
**Tencent， Canberra Australia**  
**Senior researcher in computer vision, Team lead of Mixed Reality (MR) group**

- Roadmap of MR: I have designed the first roadmap of MR for Tencent XR AU-Lab based on a
comprehensive evaluation of SOTA methods in stereo depth, multi-view stereo(MVS) and depth fusion. I
proposed a pyramid and structural-aware plane sweep MVS approach, which achieves 40FPS and is 3 times
faster than the SOTA method SimpleRecon.

<p align="center">
<img src="resources/MVS/Simplerecon.png" width="600" height="300" >
</p>

- 3D scene understanding: I am leading the development of a 3D scene understanding system similar to
Apple’s RoomPlan for MR, which detects 3D objects real-time from RGB-D images.

<p align="center">
<img src="resources/MR/M2BEV.png" width="700" >
</p>

| <img width = 600/> Input video | <img width = 600/> Multi-view stereo reconstruction | <img width = 600/> 3D scene understanding |
| :-----| :----: | :----: |
| <img width = 600/> ![MVS_AULab](resources/MVS/office.gif)  | <img width = 600/>  ![MVS_AULab](resources/MVS/AU_Lab_Office_mesh.gif)   | <img width = 300/>  ![RoomPlan](resources/MVS/roomplan_aulab.gif)  |

## General plan detection

| <img width = 400/> Input point cloud | <img width = 400/> Plane detection | <img width = 400/> Input point cloud | <img width = 400/> Plane detection |
| :-----| :----: | :----: | :----: |
| <img width = 400/> ![MVS_AULab](resources/plane_det/cor_pcd.gif)  | <img width = 400/>  ![MVS_AULab](resources/plane_det/Cor_Planes.gif)   | <img width = 300/>  ![RoomPlan](resources/plane_det/office_pcd.gif)  | <img width = 300/>  ![RoomPlan](resources/plane_det/planes_indoor.gif)  |

## BEV room layout detection
| <img width = 600/> Input point cloud | <img width = 600/> Plane detection | 
| :-----| :----: | 
| <img width = 600/> ![RoomPlan_Garage](resources/roomplan/Garage_20Dec_sold2_img_d_recording.gif)  | <img width = 600/>  ![RoomPlan_Corridor](resources/roomplan/Corridor_19Dec_sold2_img_d_recording.gif)   | 



# AR (Augmented reality) Cloud 


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
