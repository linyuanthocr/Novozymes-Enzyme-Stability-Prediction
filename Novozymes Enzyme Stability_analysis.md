# Novozymes Enzyme Stability

https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction

- Protein fold
    
    **Protein fold**（蛋白质折叠）是指蛋白质分子通过其氨基酸序列（一级结构）的非共价相互作用形成的特定三维结构。蛋白质折叠是蛋白质从线性链状结构到功能性三维形态的物理过程，是其发挥生物学功能的关键。
    
    ### 核心概念：
    
    1. **一级结构**：氨基酸序列。
    2. **二级结构**：由氢键驱动形成的局部结构，例如 α-螺旋和 β-折叠片。
    3. **三级结构**：通过疏水作用、离子键、氢键和范德华力等作用力，使二级结构折叠成一个完整的三维形态。
    4. **四级结构**：多个肽链（亚基）通过非共价作用或二硫键组装成功能性复合体。
    
    ---
    
    ### 关键要点：
    
    - **热力学假说**：蛋白质折叠的最终结构是自由能最低的构象，即所谓的"本征结构"。
    - **分子伴侣**：某些蛋白质需要分子伴侣（chaperone）辅助折叠，防止错误折叠或聚集。
    - **错误折叠与疾病**：错误折叠的蛋白质可能导致疾病，例如阿尔茨海默病、亨廷顿病和朊病毒相关疾病。
    
    ---
    
    ### 蛋白质折叠的研究：
    
    - **实验方法**：核磁共振（NMR）、X射线晶体学和冷冻电镜（Cryo-EM）是研究蛋白质折叠和三维结构的重要工具。
    - **计算模拟**：借助分子动力学模拟和人工智能（如AlphaFold）可以预测蛋白质的折叠和结构。
    
    蛋白质折叠是生物学与结构生物学的核心领域，直接影响对生命现象的理解和药物研发等实际应用。如果有具体问题可以深入探讨！ 😊
    
- Alphafold2
    
    **AlphaFold2** 是由 DeepMind 开发的一种人工智能系统，用于 **蛋白质结构预测**。它是 AlphaFold 系列的第二代产品，于 2020 年在 **CASP14（蛋白质结构预测的国际评估竞赛）** 中取得了革命性的成功，显著提高了蛋白质三维结构预测的准确性。
    
    ---
    
    ### **AlphaFold2 的核心功能：**
    
    AlphaFold2 的目标是根据蛋白质的 **氨基酸序列** 精确预测其 **三维结构**。蛋白质的三维结构决定其功能，但实验确定结构（如 X 射线晶体学、核磁共振、冷冻电镜）通常耗时、昂贵且具有挑战性。AlphaFold2 提供了一种快速、高效的替代方法。
    
    ---
    
    ### **AlphaFold2 的原理：**
    
    1. **输入**：
        - 蛋白质的氨基酸序列。
        - 来自同源序列数据库的多序列比对（MSA）。
        - 空间中残基之间的几何约束。
    2. **核心技术**：
        - 使用深度学习方法，结合注意力机制（transformer architecture），来处理氨基酸序列和其进化信息。
        - 通过迭代优化，生成蛋白质折叠路径并预测最终的三维结构。
    3. **输出**：
        - 高精度的蛋白质三维结构（包括主链和侧链位置）。
        - 预测可信度分数（pLDDT），用于评估结构的可靠性。
    
    ---
    
    ### **AlphaFold2 的优势：**
    
    1. **高精度**：其预测精度与实验结果接近，甚至在某些简单蛋白质的情况下可以媲美实验数据。
    2. **快速性**：相比实验方法，AlphaFold2 大幅缩短了时间成本（数小时到数天）。
    3. **广泛应用**：
        - **基础研究**：理解蛋白质功能和生物过程。
        - **药物研发**：加速靶标蛋白的识别和结构分析。
        - **生物工程**：设计新型蛋白质和功能性分子。
    
    ---
    
    ### **应用实例：**
    
    1. **生物医学**：
        - 预测疾病相关蛋白的结构，例如癌症相关蛋白或病毒蛋白（如新冠病毒的刺突蛋白）。
    2. **合成生物学**：
        - 帮助设计功能性酶和合成分子。
    3. **大规模结构预测**：
        - AlphaFold 数据库已公开超过 2 亿个蛋白质的预测结构，为生命科学研究提供了巨大的资源。
    
    ---
    
    AlphaFold2 是生命科学领域的一次变革，不仅解决了长期的科学难题，还为生物学、医学和药物研发开辟了新的可能性。如果你对其实现细节或具体应用有兴趣，可以进一步讨论！ 😊
    
- pdb files
    
    **.pdb 文件** 是一种用于存储 **蛋白质三维结构** 的文件格式，全称为 **Protein Data Bank file**。它是由 **PDB（蛋白质数据银行）** 定义的标准格式，广泛用于分子生物学和结构生物学领域，用于描述蛋白质、核酸以及小分子复合物的三维结构。
    
    ---
    
    ### **.pdb 文件的主要内容：**
    
    1. **三维坐标**：描述了蛋白质中每个原子的空间坐标（x, y, z）。
    2. **原子信息**：
        - 原子编号、原子名称、残基名称。
        - 残基编号、链标识符。
    3. **拓扑结构**：包括二级结构的信息（如 α-螺旋、β-折叠片）。
    4. **连接信息**：描述化学键和配体结合。
    5. **注释**：蛋白质功能、来源、实验方法（如 X 射线晶体学、NMR）等元数据。
    
    ---
    
    ### **.pdb 文件的基本格式示例：**
    
    ```
    ATOM      1  N   GLY A   1      11.104  13.207  12.411  1.00 21.46           N
    ATOM      2  CA  GLY A   1      11.806  13.098  11.100  1.00 20.94           C
    ATOM      3  C   GLY A   1      12.709  14.261  10.728  1.00 20.13           C
    ATOM      4  O   GLY A   1      12.825  15.170  11.569  1.00 19.99           O
    HETATM   23  O   HOH A   5       8.108   8.545   9.123  1.00 18.33           O
    
    ```
    
    ### **字段含义**：
    
    - `ATOM`：原子信息记录。
    - `N/CA/C/O`：原子名称。
    - `GLY`：氨基酸名称（甘氨酸）。
    - `A`：链 ID。
    - 坐标信息：`11.104 13.207 12.411` 是原子在空间中的 x, y, z 坐标。
    - `1.00` 和 `21.46`：占有率和 B 因子（结构的热运动指标）。
    
    ---
    
    ### **.pdb 文件的用途：**
    
    1. **结构可视化**：通过分子可视化软件（如 PyMOL、Chimera、VMD）展示蛋白质的三维结构。
    2. **分子模拟**：作为输入文件用于分子动力学模拟或对接实验。
    3. **功能研究**：分析蛋白质的活性位点、配体结合、分子间相互作用等。
    4. **数据库存储**：蛋白质结构数据（如 PDB 数据库）以 .pdb 格式为主。
    
    ---
    
    ### **如何获取 .pdb 文件？**
    
    - **PDB 数据库**：[Protein Data Bank (RCSB PDB)](https://www.rcsb.org/)
        - 提供数百万蛋白质和核酸的三维结构，支持按 PDB ID 检索和下载。
    
    ---
    
- Dataset Description
    
    In this competition, you are asked to develop models that can predict the r**anking of protein thermostability (as measured by melting point, `tm`) after single-point amino acid mutation and deletion.**
    
    For the training set, the protein thermostability (experimental melting temperature) data includes natural sequences, as well as engineered sequences with single or multiple mutations upon the natural sequences. The data are mainly from different sources of published studies such as [Meltome atlas—thermal proteome stability across the tree of life](https://doi.org/10.1038/s41592-020-0801-4). Many other public datasets exist for protein stability; please see the competition [Rule 7C](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction/rules) for external data usage requirements. There are also other publicly available methods which can predict protein stabilities such as [ESM](https://doi.org/10.1073/pnas.2016239118), [EVE](https://doi.org/10.1038/s41586-021-04043-8) and [Rosetta](https://doi.org/10.1016/B978-0-12-381270-4.00019-6) etc., without using the provided training set. These methods may also be used as part of the competition.
    
    The test set contains experimental melting temperature of over 2,413 single-mutation variant of an enzyme (GenBank: KOC15878.1), obtained by Novozymes A/S. The amino acid sequence of the wild type is:
    
    `VPVNPEPDATSVENVALKTGSGDSQSDPIKADLEVKGQSALPFDVDCWAILCKGAPNVLQRVNEKTKNSNRDRSGANKGPFKDPQKWGIKALPPKNPSWSAQDFKSPEEYAFASSLQGGTNAILAPVNLASQNSQGGVLNGFYSANKVAQFDPSKPQQTKGTWFQITKFTGAAGPYCKALGSNDKSVCDKNKNIAGDWGFDPAKWAYQYDEKNNKFNYVGK`
    
    ![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image.png)
    

***Learning to Rank - Developed a 3D CNN-based ranking model using voxelized
protein structures and biochemical features, leveraging Rosetta for mutation
modeling and an ensemble of models for stability prediction***

**Dataprepare: data+single mutation→alphafold→pdb files**

DataSet:

compiles together 8 datasets and generates voxel features that can later be used to train 3D CNN models for protein stability detection. The following source databases were used to generate the resulting dataset:

- [ThermoMutDB](http://biosig.unimelb.edu.au/thermomutdb)
- [iStable2.0](http://ncblab.nchu.edu.tw/iStable2/)
- [dt-xgboost-5000-mutations-200-pdb-files-lb-0-40](https://www.kaggle.com/code/cdeotte/xgboost-5000-mutations-200-pdb-files-lb-0-40)
- [S1626](https://aip.scitation.org/doi/suppl/10.1063/1.4947493)
- [S140](http://marid.bioc.cam.ac.uk/sdm2/data)
- [S2648](http://marid.bioc.cam.ac.uk/sdm2/data)
- [Q3214, Q1744](https://github.com/gersteinlab/ThermoNet/tree/master/data/datasets)
- [Q3421](https://github.com/gersteinlab/ThermoNet/tree/master/data/datasets)
- [FireProtDB (6713 mutations)](https://loschmidt.chemi.muni.cz/fireprotdb/)

There is a significant overlap between datasets above. Unique mutations can be described with the following unique triplets `(fasta_sequence, pdb_mutation_position, mutant_residue)`. The final dataset generated by this notebook contains 14656 such unique triplets. AFAIK at the time of publishing (26.10) this is the largest published NESP dataset by number of unique single mutations!

https://www.kaggle.com/code/vslaykovsky/14656-unique-mutations-voxel-features-pdbs?scriptVersionId=109568406

Evaluation Matric:

The competition metric is `Spearman Correlation Coefficient` which is a ranking metric. only **order** matters.

[**How To Use Kaggle's Train Data**](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction/discussion/358320)

1. The test data contains 2413 rows and all 2413 rows come from the same one wild type protein. The rows of test data are 1 mutation applied to a certain known one.
2. 

Prediction

paper:

Predicting changes in protein thermodynamic stability upon point mutation with deep 3D
convolutional neural networks

https://journals.plos.org/ploscompbiol/article/file?id=10.1371/journal.pcbi.1008291&type=printable

![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%201.png)

![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%202.png)

The uploaded paper, titled **"Predicting changes in protein thermodynamic stability upon point mutation with deep 3D convolutional neural networks,"** introduces **ThermoNet**, a computational framework based on deep 3D-convolutional neural networks (3D-CNNs). Below is an overview of the key concepts and findings from the paper:

### Summary of the Paper:

1. **Objective**:
The study focuses on predicting mutation-induced changes in protein thermodynamic stability (ΔΔG) to address challenges in protein engineering and understanding disease-causing mutations.
2. **ThermoNet Overview**:
    - ThermoNet treats protein structures as multi-channel 3D images to predict ΔΔG values for point mutations.
    - Inputs to the model are voxel grids representing the biophysical properties of atoms in the protein structure.
3. **Model Architecture**:
    - Utilizes 3D-CNNs to process the voxel grids.
    - Incorporates local biochemical interactions and aggregates them hierarchically to predict complex, nonlinear effects of mutations on stability.
    - Includes data augmentation with anti-symmetry principles to balance predictions between stabilizing and destabilizing mutations.
4. **Data and Testing**:
    - The model was trained on a curated dataset of mutations with experimental ΔΔG values.
    - Rigorous homology reduction ensured no overlap between training and testing datasets, addressing biases common in previous models.
5. **Key Findings**:
    - ThermoNet achieved state-of-the-art performance, comparable to or exceeding existing ΔΔG predictors like DDGun and STRUM.
    - The model demonstrated reduced bias and higher accuracy for both stabilizing and destabilizing mutations.
    - Case studies on clinically relevant proteins (e.g., p53 and myoglobin) showcased its applicability in medical genetics.
6. **Challenges and Limitations**:
    - The reliance on 3D structural data limits its applicability to proteins without resolved or modeled structures (~70% of the proteome).
    - Training deep 3D-CNNs is resource-intensive and requires significant computational power.
7. **Applications**:
    - ThermoNet can be used for designing stable proteins, studying disease-causing mutations, and prioritizing candidate variants for experimental testing.

Useful Sources:

[**1st Place Public - Shakedown to 967th Place Private - Hahaha**](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction/discussion/376116)

1. PB first place

https://www.kaggle.com/code/cdeotte/public-lb-1st-place-solution

1. **ThermoNet v2**

https://www.kaggle.com/code/vslaykovsky/nesp-thermonet-v2?scriptVersionId=109617489

- Model highlight
    
    ![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%203.png)
    
    ![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%204.png)
    
    ![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%205.png)
    
    ![image.png](Novozymes%20Enzyme%20Stability%2017e71bdab3cf809881bddd4b585389e9/image%206.png)
    
1. https://www.kaggle.com/code/cdeotte/xgboost-5000-mutations-200-pdb-files-lb-0-410
2. https://www.kaggle.com/code/shlomoron/nesp-relaxed-rosetta-scores