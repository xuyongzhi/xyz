# Yongzhi
Computer vision researcher and engineer with 5 years’ academic and 4 years’ industry experience. I have
developed several popular products on TikTok and CapCut at ByteDance. I am currently working on 3D
reconstruction and scene understanding as the team lead of mixed reality (MR) group in Tencent XR AU-Lab.
I love coding and have been programming using C++ and python for around 9 years. I am passionate on
pursuing excellence, embracing challenges, enjoying work with others, learning new things along the way.

# 3D scene generation using panoramic RGBD diffusion models
<p align="center">
<img src=resources/scene_gen/scene_gen_overview.png width=800 />
</p>

## Two stage coarse-to-fine panorama generation
<p align="center">
<img src=resources/scene_gen/panorama_gen.png width=800 />
</p>

|  Prompt | Panorama RGB | 
| :-----| :----: |
|  For_Honor, The image is a 360-degree panoramic view of a fantasy-themed village, featuring various buildings and structures. The village appears to be located near a body of water, possibly a river or a lake. There are also some trees visible in the background, adding to the overall atmosphere of the scene. |   <img src="resources/scene_gen/For_Honor,_The_image_is_a_360-degree_panoramic_vie1.png" width="5000" />  |
| genshin, The image is a 360-degree panoramic view of a cobblestone street with buildings and a windmill in the background. It appears to be a computer-generated or animated scene, possibly from a video game or virtual world. | <img src="resources/scene_gen/genshin,_The_image_is_a_360-degree_panoramic_view_1.png" width="5000" /> |
|Ghost_Recon, The image is a 360-degree panoramic view of a mountainous landscape with a lake in the foreground. There are several trees and bushes visible in the scene. The image appears to be a digital or computer-generated representation of the landscape, rather than an actual photograph.|<img src="resources/scene_gen/Ghost_Recon,_The_image_is_a_360-degree_panoramic_v0.png" width="5000" />|
|The image is a 360-degree panoramic view of a bedroom, featuring a large bed, a television, and a window with a view of the city. The room is decorated in a modern style, with wooden floors and white walls. There is also a chair and a lamp in the room. The panoramic view provides an immersive experience, allowing the viewer to take in the entire room and its surroundings.|<img src="resources/scene_gen/The_image_is_a_360-degree_panoramic_view_of_a_bedr2.png" width="5000" />|
|The image is a 360-degree panoramic view of a city street, with buildings and cars visible in the foreground. It appears to be taken from a high vantage point, providing a bird's-eye view of the urban environment.|<img src="resources/scene_gen/The_image_is_a_360-degree_panoramic_view_of_a_city0.png" width="5000" />|

## RGBD diffusion 
<p align="center">
<img src="resources/scene_gen/RGBD_diffusion.png" width="1200" />
<img src="resources/scene_gen/depth_compare.png" width="1200" />
</p>


## Panorama inpainting: Masked image conditional UNet + Manifold constraint training

<p align="center">
<img src="resources/scene_gen/Inpainting_method.png" width="1200" />
</p>

- Vanilla FT inpainting: Finetune inpainting models using Lora.  
- Our MCT inpainting:  inpainting model trained with Lora and manifold constraint loss.  

   
<img src="resources/scene_gen/inpaint0.png" width="1200" />
<img src="resources/scene_gen/inpaint1.png" width="1200" />
<img src="resources/scene_gen/inpaint2.png" width="1200" />
<img src="resources/scene_gen/inpaint3.png" width="1200" />
<img src="resources/scene_gen/inpaint4.png" width="1200" />
<img src="resources/scene_gen/inpaint5.png" width="1200" />
<img src="resources/scene_gen/inpaint6.png" width="1200" />
<img src="resources/scene_gen/inpaint7.png" width="1200" />


# Dense 3D reconstruction and scene understanding for VR headset 
**Tencent， Canberra Australia**  
**Senior researcher in computer vision, Team lead of Mixed Reality (MR) group**

- Roadmap of MR: I have designed the first roadmap of MR for Tencent XR AU-Lab based on a
comprehensive evaluation of SOTA methods in stereo depth, multi-view stereo(MVS) and depth fusion. 
- I proposed a pyramid and structural-aware plane-sweep MVS approach, based on SimpleRecon, that achieves a speed improvement from 75ms to 25ms.

| <img width = 600/> SimpleRecon | <img width = 600/> Structure-aware virtual camera locations | 
| :-----| :----: |
| <img width = 600/> ![MVS_AULab](resources/MVS/Simplerecon.png)  | <img width = 600/>  ![MVS_AULab](resources/MVS/MVS-Virtual_cameras.png)   |

- 3D scene understanding: I am leading the development of a 3D scene understanding system similar to
Apple’s RoomPlan for MR, which detects 3D objects real-time from RGB-D images.

| <img width = 600/> Input video | <img width = 600/> Multi-view stereo reconstruction | <img width = 600/> 3D scene understanding |
| :-----| :----: | :----: |
| <img width = 600/> ![MVS_AULab](resources/MVS/office.gif)  | <img width = 600/>  ![MVS_AULab](resources/MVS/AU_Lab_Office_mesh.gif)   | <img width = 300/>  ![RoomPlan](resources/MVS/roomplan_aulab.gif)  |



## General plan detection

| <img width = 400/> Input point cloud | <img width = 400/> Plane detection | <img width = 400/> Input point cloud | <img width = 400/> Plane detection |
| :-----| :----: | :----: | :----: |
| <img width = 400/> ![MVS_AULab](resources/plane_det/cor_pcd.gif)  | <img width = 400/>  ![MVS_AULab](resources/plane_det/Cor_planes.gif)   | <img width = 300/>  ![RoomPlan](resources/plane_det/office_pcd.gif)  | <img width = 300/>  ![RoomPlan](resources/plane_det/planes_indoor.gif)  |




# AR (Augmented reality) Cloud 


## Structure from motion (SFM) of 3D line map

Key contributions:
1. A novel 3D mapping pipeline.   
2. Multi-view triangulation using Plucker representation.   
3. No Manhattan assumption

| <img width = 1000/> High-precision map for AR | <img width = 1000/> The pipeline of proposed 3D line mapping approach.|
| :-----| :----: |
|  ![AR_HR_Map](resources/BT_AR/AR_Map.PNG)  | <img width = 1000/>  ![line_mapping](resources/SFM/line_mapping.jpg)  |
|![Tri](resources/SFM/Line_Tri.png) | ![Tri](resources/SFM/LineMat.png) |



| |<img width = 1000/>   |  <img width = 1000/> |
| ----------- |  ----------- | ----------- |
| 3D point cloud | ![BJF_Points1](resources/SFM/BJF_Points_1.gif) | ![BJF_Points2](resources/SFM/BJF_Points_2.gif)      |
| 3D line cloud |  ![BJF_line_sfm](resources/SFM/BJF_LineSFM.gif) | ![BJF_line_cloud](resources/SFM/BJF_3D_lines.gif)   |
| Reprojections | ![rep_lines_A](resources/SFM/project_lines_A.gif) | ![rep_lines_A](resources/SFM/project_lines_B.gif) | 


## Visual positioning system combining features of point and line  
Key contributions: 
- A novel geometric & descriptor fused line matching approach based on coarse VPS pose.

| <img width = 1000/> VPS (Visual Positioning Service) | <img width = 1000/> The pipeline of proposed line-based pose verification & refinement.|
| :-----| :----: |
| ![VPS](resources/VPS/VPS.gif) |![point_line_vps](resources/VPS/Poine_Line_VPS.png)|
| I proposed a new approach of pose refinement by combing deep features of points and lines. The 1st contribution is a structure-aware line detector \& descriptor network, which jointly matches lines and junctions locally. The 2nd one is a fused PnPL-based pose estimator combing line-matching, junction-matching and vanishing points. The localization accuracy (within 1m) has been improved from 91\% to 96\% compared with using points only.  |![JcASL_MAT](resources/VPS/NL_JcASL_Line.gif)|


## SuperPoint
I improved the open implementation of SuperPoint which achieve similar performance of the official model.
The recall of MagicLeap can achieve 0.42. However, the recalls of pretrained model of TF_SP and PyTorch_SP are both around 0.145.  I have improved the recall of PyTorch_SP to 0.41.

- Holography augmentation using Thesesus  (https://github.com/facebookresearch/theseus)
- Small rotation (15 to 30 degree)
- Using pseudo GT generated by MagicLeap-SP, instead of MagicPoint in Pytorch_SP 
- An implementation of homograph adaptation based on the original paper, combing within-scale and across-scale.
- Use the Recall to evaluate the performance following "An Evaluation of Feature Matchers for Fundamental Matrix Estimation".


## 3D surface detection from a single view  

Multiple 3D surfaces are detected from a single view.
- No Manhattan assumption
- Unknown camera models 
- 3D normal accuracy > 97% in real world images (around 60% accuracy achieved by SOTA learning and handcrafted methods.)
![Surface3D](resources/BT_AR/3D_surfaces.gif)

### Wrap virtual materials on the 3D surfaces:  
- Fully automated and real-time generation of multiple 3D planes from a single view.  
- The layout of multiple planes are optimized based on the scores and distribution of 3D planes.  

| | |
| :-----| :----: |  
| <img width = 600/> ![Surface3D](resources/BT_AR/Cyberpunk.gif) |  <img width = 600/>  ![AR_Chinese](resources/BT_AR/AR_ChineseNewYear.gif) |


## Intelligent advertisement placement

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
