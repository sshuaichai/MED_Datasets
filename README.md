# -此存储库用于索引感兴趣的数据集、论文、代码...
 
 ---------------------------------------------------------------------------------------
 论文：
 ---------------------------------------------------------------------------------------

 1.Segment anything in medical images
 论文：https://www.nature.com/articles/s41467-024-44824-z  、  https://arxiv.org/pdf/2304.12306
 代码：https://github.com/bowang-lab/MedSAM
 知乎：https://zhuanlan.zhihu.com/p/717053976
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
