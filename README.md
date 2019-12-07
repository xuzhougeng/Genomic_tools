# 基因组学工具合集

整理了一些我所知道的和基因组学相关的工具，可能不全面，欢迎补充

## 一代组装

- [Celera Assembler](http://wgs-assembler.sourceforge.net/): 最具代表性的工具
          
## 二代组装

- Minia
- SPAdes: 细菌基因组常用
- ALLPaths-LG
- SOAPdenovo: 华大出品

## 三代contig组装

- [falcon](https://github.com/PacificBiosciences/pb-assembly): PacBio专用组装工具        
- [Canu](https://canu.readthedocs.io/en/latest/): 老牌工具，资源消耗大
- [MECAT](https://github.com/xiaochuanle/MECAT): 高效的三代组装工具
- [MECAT2](https://github.com/xiaochuanle/MECAT2): PacBio专用组装工具
- [NECAT](https://github.com/xiaochuanle/NECAT): Nanopore专用组装工具
- [NextDenovo](https://github.com/Nextomics/NextDenovo): 可用于Nanopore的组装工具
- [FLYE](https://github.com/fenderglass/Flye)
- [SMARTdenovo](https://github.com/ruanjue/smartdenovo)       
- [WTDBG2](https://github.com/ruanjue/wtdbg2)

## GFA相关

GFA是目前组装比较认可的格式

- [GFA格式声明](http://gfa-spec.github.io/GFA-spec/GFA1.html​)        
- [Gfakluge](https://github.com/edawson/gfakluge): GFA操作工具         
- [Bandage](https://github.com/rrwick/Bandage): 全平台GUI可视化工具
- [GfaViz](https://github.com/ggonnella/gfaviz): 命令行的可视化        
- [AGB](https://github.com/almiheenko/AGB): Linux分析，网页展示
          

##  三代组装polish

- Pilon: 利用二代进行polish
- Racon: 利用三代进行polish
- NextPolish: 利用二代进行polish
- Medaka: 利用三代对nanpore进行polish

## 去除冗余序列

- [purge_haplotigs](https://bitbucket.org/mroachawri/purge_haplotigs)
- [HaploMerger2](https://github.com/mapleforest/HaploMerger2)
- [Redundans](https://github.com/lpryszcz/redundans)

##  辅助组装

使用遗传图谱，光学图谱，Hi-C和物种间共线性对contig进行scaffold的工具

### HiC

- [SALSA](https://github.com/marbl/SALSA): 高效率，能纠错使用GFA信息
- [HiCAssembler](https://github.com/maxplanck-ie/HiCAssembler): 借鉴了3D-DNA
- [3D-DNA](https://github.com/theaidenlab/3d-dna): 搭配JuicerBox效果极佳（但是速度有点慢） 
- [ALLHiC](https://github.com/tangerzhang/ALLHiC): 多倍体HiC组装             
- LACHESIS: 古老的工具，已不再维护

### BioNano

### 遗传图谱

### 整合工具

- [ALLMAPS](https://github.com/tanghaibao/jcvi/): 可以整合多张图谱做一套比较好的染色体组装

## 组装质量评估

- [BUSCO](https://busco.ezlab.org/)
- [CEGMA](http://korflab.ucdavis.edu/datasets/cegma/)
- [LAI](https://github.com/oushujun/LTR_retriever)

## 重复序列注释

- RepeatModeler
- RepeatMasker
- [EDTA](https://github.com/oushujun/EDTA)
- [LTRpred](https://hajkd.github.io/LTRpred/)
          

## 基因注释

- 从头预测
  - AUGUSTUS
  - SNAP
  - GeneMark

- 注释流程
  - [Braker2](https://github.com/Gaius-Augustus/BRAKER)
  - [MAKER](https://www.yandell-lab.org/software/maker.html)
             

## WGD分析

- [wgd](https://github.com/arzwa/wgd)

## 全基因组比对软件

- LAST
- LASTZ
- MUMMER
- minimap2

## 共线性可视化

- [dotPlotly](https://github.com/tpoorten/dotPlotly)         

## 群体结构

- STRUTURE
- [Admixture](http://software.genetics.ucla.edu/admixture/)
- [lostruct](https://github.com/petrelharp/local_pca)
          
