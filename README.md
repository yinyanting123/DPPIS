# DPPIS
DPPIS is a repository of dynamic network datasets with structure information. Specifically， it is an enhanced protein interaction dataset built upon the dppin database, featuring temporal dynamics augmentation and AlphaFold-predicted structural data to empower dynamic network analysis and computational biology research.

The current release includes sample data primarily based on the Hazbun dataset.  

 # Key Features
🔥 Enhanced Temporal Dynamics  
- New interaction temporal labels (transient/persistent)
- Contain structure information
- Dynamic network evolution trajectories

# 主要特性
🔥 动态信息增强  
- 新增蛋白质相互作用的时间动态标签（瞬时/持续）
- 补充蛋白质的机构信息
- 添加动态网络演化轨迹数据


# Future Plans  
- 2026: Complete release of protein structural information for all 12 datasets  
- 2027: Provide feature mining and alignment schemes for protein structural/sequential/descriptive information  
- 2028: Launch an integrated framework for dynamic protein relationship prediction with variable time intervals  

# 未来计划
- 2026: 完整发布12个数据集对应的蛋白质结构信息以及学习方案
- 2027: 提供蛋白质结构信息、序列信息、描述信息等的特征挖掘以及特征对齐方案
- 2028: 推出不定时间间隔的蛋白质关系动态预测集成框架

# Quick Startpython
import pandas as pd
from biopandas.pdb import PandasPdb

# Load interaction data
df = pd.read_json('dataset/dynamic_network/interactions.json')

# Read structural data
ppdb = PandasPdb().read_pdb('dataset/structure/AF-P12345-F1.pdb')
atoms = ppdb.df'ATOMS'


# Acknowledgments
This project builds upon these foundational works:
- dppin Dynamic PPI Database 
- AlphaFold2 Protein Structure Prediction System
