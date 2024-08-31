# -shuaishuai notes
 ---------------------------------------------------------------------------------------
模型代码
 ---------------------------------------------------------------------------------------

# facebookresearch
**Meta Research**

**1.segment-anything**
- 代码：https://github.com/facebookresearch/segment-anything
- 数据集：https://ai.meta.com/datasets/segment-anything-downloads/
- 网址：https://segment-anything.com/
- online demo：https://segment-anything.com/demo
- 知乎：https://zhuanlan.zhihu.com/p/717082584
- 该存储库已由所有者于 2024 年 7 月 1 日存档。现在为只读。
- 该存储库提供使用 SegmentAnything 模型 (SAM) 运行推理的代码、用于下载训练后的模型检查点的链接以及展示如何使用该模型的示例笔记本。
<img width="1206" alt="model_diagram" src="https://github.com/user-attachments/assets/0747c177-ae99-4364-abac-e54eebcd2824">
 <img src="https://github.com/sshuaichai/shuaishuai-notes/blob/main/assets/minidemo.gif" width="500"/>

![image](https://github.com/user-attachments/assets/98b33e8e-0649-434a-8555-1dfa0eff6073)

![image](https://github.com/user-attachments/assets/728a8ff2-6520-4afb-a35c-880f6049eee5)

自从sam模型发布以来，基于sam的二次应用及衍生项目越来越多，将其应用于各种任务，比如图像修复( image inpainting)、图像编辑（ image editing）、目标检测（objects detection）、图像标注（Image Caption）、视频跟踪(object tracking)、3d检测等等。
参考知乎：https://zhuanlan.zhihu.com/p/630529550
- 收集一些 Transformer 与计算机视觉（CV）的论文：https://github.com/dk-liang/Awesome-Visual-Transformer
- 对视觉及其他领域 Segment Anything 模型的全面调查的论文：https://github.com/liliu-avril/Awesome-Segment-Anything?tab=readme-ov-file
- 针对任何事物的通用 AI 方法的精选列表：https://github.com/VainF/Awesome-Anything?tab=readme-ov-file
- Segment Anything 推动了计算机视觉（CV）领域的新突破，本仓库将持续跟踪和总结 Segment Anything 在各个领域的研究进展，包括论文/项目等：https://github.com/Hedlen/awesome-segment-anything
- SAM 和相关研究的项目、论文和源代码的集合☆:https://github.com/Vision-Intelligence-and-Robots-Group/Awesome-Segment-Anything?tab=readme-ov-file
- 超棒的分割任何内容扩展☆：https://github.com/JerryX1110/awesome-segment-anything-extensions?tab=readme-ov-file
![232959211-6ee84ad5-a02d-44ca-91d2-17d12b978fb2](https://github.com/user-attachments/assets/b9ffed3b-5558-435a-a3e3-01d82d5b0e6c)
















 
 ---------------------------------------------------------------------------------------
 论文：
 ---------------------------------------------------------------------------------------

 1.Segment anything in medical images
 - 论文：https://www.nature.com/articles/s41467-024-44824-z  、  https://arxiv.org/pdf/2304.12306
-  代码：https://github.com/bowang-lab/MedSAM
-  知乎：https://zhuanlan.zhihu.com/p/717053976
![image](https://github.com/user-attachments/assets/3e8b0a14-fbd3-496e-84e9-db76b7da2b4c)





---------------------------------------------------------------------------------------
 数据集
---------------------------------------------------------------------------------------

# 2022-2023年

1.腹部CT-1K
作者：https://github.com/JunMa11
我们通过在现有的单一器官数据集 [1-6] 中添加四个腹部器官（包括肝脏、肾脏、脾脏和胰腺），收集了包含 1000 多张 CT 扫描的大型且多样化的腹部 CT 器官分割数据集。
- 代码：https://github.com/JunMa11/AbdomenCT-1K?tab=readme-ov-file
- 2022大挑战：https://flare22.grand-challenge.org/  快速、低资源半监督 CT 腹部器官分割（FLARE 2022）
- FLARE 2022 数据集介绍：FLARE 2022 数据集介绍 - 知乎  https://zhuanlan.zhihu.com/p/657611778

基于 nnU-Net 的 MICCAI FLARE22 挑战赛冠军解决方案：
- 让 nnU-Net 更快还能半监督学习：MICCAI FLARE 2022 挑战赛冠军方案介绍 
- 代码： https://github.com/Ziyan-Huang/FLARE22
- 冠军方案 paper：SpringerLink
- 冠军方案知乎：https://zhuanlan.zhihu.com/p/657611778
![advertise_tj8gutu x15](https://github.com/user-attachments/assets/a42ec72e-5616-44a8-95dc-40708c16ba03)

2023大挑战：https://codalab.lisn.upsaclay.fr/competitions/12239#learn_the_details-dataset
![FLARE23-Dataset](https://github.com/user-attachments/assets/2d037f47-9d28-4e94-b418-0628905e9272)
训练集：2200 份带部分标签的 CT 扫描和 1800 份不带标签的 CT 扫描
验证集：100 张不同类型癌症的 CT 扫描结果
测试集：400 张不同类型癌症的 CT 扫描图
- 下载数据集：  https://forms.gle/UMifAi8qufDga86Z6 
- 下载伪标签 https://drive.google.com/drive/folders/1sQ89xJsTeplXF6FFVwT7E5p8w0FUiyeP?usp=sharing
 这些伪标签可用于模型训练。请注意，不允许手动选择高质量的伪标签进行模型训练。（其他预训练模型和数据集也不允许。）

773例带有假肿瘤标签的病例
（下载：百度网盘 https://pan.baidu.com/s/17FJfxAR6MVnYRiT-_dRNgA?pwd=2021 、
Google Drive https://drive.google.com/file/d/12AINDARYZDrdc66v891YT6VDxW9NsfjR/view?usp=sharing）
更新：我们添加了 110 个病例的标签。现在，它包含 773 个带有伪肿瘤标签的病例。相应的图像位于整个数据集中Case_00001-00773。
![TumorDemo](https://github.com/user-attachments/assets/35db6d66-8def-4a24-be80-71544274fd59)
仅使用单相 CT 扫描很难做出明确而准确的诊断，因为识别（恶性）肿瘤通常需要病理检查。作为替代方案，我们通过注释所有可能的肿瘤提供了 663 例伪肿瘤标签，可用于噪声标签学习。

2.
