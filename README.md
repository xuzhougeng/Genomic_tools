# 基因组学工具合集

整理了一些我所知道的和基因组学相关的工具，可能不全面，欢迎补充

PS: 有中文评论才是我用过的

## 基因组Survey

- [GenomeScop2.0](https://github.com/tbenavi1/genomescope2.0) : Reference-free profiling of polyploid genomes
- [smudgeplot](https://github.com/KamilSJaron/smudgeplot): Inference of ploidy and heterozygosity structure using whole genome sequencing data

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
- [HINGE](https://github.com/HingeAssembler/HINGE)
- [MECAT](https://github.com/xiaochuanle/MECAT): 高效的三代组装工具
- [MECAT2](https://github.com/xiaochuanle/MECAT2): PacBio专用组装工具
- [NECAT](https://github.com/xiaochuanle/NECAT): Nanopore专用组装工具
- [NextDenovo](https://github.com/Nextomics/NextDenovo): 可用于Nanopore的组装工具
- [FLYE](https://github.com/fenderglass/Flye)
- [SMARTdenovo](https://github.com/ruanjue/smartdenovo)       
- [WTDBG2](https://github.com/ruanjue/wtdbg2): 不对原始数据纠错,快速的组装工具
- [Shasta](https://github.com/chanzuckerberg/shasta): Nanopore组装工具

## GFA相关

GFA是目前组装比较认可的格式

- [GFA格式声明](http://gfa-spec.github.io/GFA-spec/GFA1.html)        
- [Gfakluge](https://github.com/edawson/gfakluge): GFA操作工具         
- [Bandage](https://github.com/rrwick/Bandage): 全平台GUI可视化工具
- [GfaViz](https://github.com/ggonnella/gfaviz): 命令行的可视化        
- [AGB](https://github.com/almiheenko/AGB): Linux分析，网页展示
          

##  三代组装polish

- Pilon: 利用二代进行polish
- Racon: 利用三代进行polish
- NextPolish: 利用二代进行polish
- Medaka: 利用三代对nanpore进行polish(建议先用Racon Polish至少一次)

## 去除冗余序列

- [HaploMerger2](https://github.com/mapleforest/HaploMerger2)
- [Redundans](https://github.com/lpryszcz/redundans)
- [purge_haplotigs](https://bitbucket.org/mroachawri/purge_haplotigs)
- [purge_dups](https://github.com/dfguan/purge_dups): 借鉴了purge_haplotigs，但是更快更自动化，智能确定阈值

##  辅助组装

使用遗传图谱，光学图谱，Hi-C和物种间共线性对contig进行scaffold, 或者是基于已有参考基因组进行辅助组装。

### HiC

- [SALSA](https://github.com/marbl/SALSA): 高效率，能纠错使用GFA信息
- [HiCAssembler](https://github.com/maxplanck-ie/HiCAssembler): 借鉴了3D-DNA
- [3D-DNA](https://github.com/theaidenlab/3d-dna): 搭配JuicerBox效果极佳（但是速度有点慢） 
- [ALLHiC](https://github.com/tangerzhang/ALLHiC): 多倍体HiC组装             
- LACHESIS: 古老的工具，已不再维护

### 光学图谱

- [Bionano Solve](https://bionanogenomics.com/support/software-downloads/): BioNano提供的一系列分析脚本工具
- [BIONANO ACCESS](https://bionanogenomics.com/support/software-downloads/): BioNano提供的网页工具
- [OMSV](http://yiplab.cse.cuhk.edu.hk/omsv/): 基于光学图谱鉴定SV
- [OMTools](https://github.com/TF-Chan-Lab/OMTools): 光学图谱数据处理，分析和可视化

## 基于已有基因组

- [chromosomer](https://github.com/gtamazian/chromosomer)
- [RaGoo](https://github.com/malonge/RaGOO)
- [Ragout](https://github.com/fenderglass/Ragout)

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

- 三代注释工具
  - [FLAIR](https://github.com/BrooksLabUCSC/flair): 用于nanopore cDNA, native RNA, PacBio的纠错,鉴定isoform,可变剪切分析
  - [SQANTI](https://bitbucket.org/ConesaLab/sqanti/src/master/): 新转录本的结构和质量注释
  - [PINISH](https://github.com/nanoporetech/pinfish): 构建注释信息

- 注释流程
  - [Braker2](https://github.com/Gaius-Augustus/BRAKER)
  - [MAKER](https://www.yandell-lab.org/software/maker.html)
  - [LoReAn](https://github.com/lfaino/LoReAn): 整合三代测序的基因组注释流程
             

## WGD分析

- [wgdi](https://github.com/SunPengChuan/wgdi/): 比较基因组学分析的瑞士军刀
- [wgd](https://github.com/arzwa/wgd)

## 全基因组比对软件

- LAST
- LASTZ
- MUMMER
- minimap2

## 共线性可视化

- [D-Genies](http://dgenies.toulouse.inra.fr/): 非常好用的网页工具
- [dotPlotly](https://github.com/tpoorten/dotPlotly)         

## 群体结构

- STRUTURE
- [Admixture](http://software.genetics.ucla.edu/admixture/)
- [lostruct](https://github.com/petrelharp/local_pca)
          
