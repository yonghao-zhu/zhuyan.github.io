---
layout: post
toc: true
title: "Computational Methods in Solid State Physics: Perface"
categories: Library
tags: [electronic-structure, Computational Methods in Solid State Physics]
author:
  - Nemoshkalenko V V, Antonov N V
---

Computational Methods in Solid State Physics

<img src="https://yonghao-zhu.github.io/zhuyan.github.io)/imags/library/CMSSP/0-CMSSP.jpg" width="60%">

## Perface

&emsp; 金属物理学 是 基于量子力学的，然而，在量子力学建立之前，在金属中重要的电子传导特性是利用自由电子模型（free-electron mode）来研究的。在1928年，Sommerfeld阐述了量子力学的自由电子模型，他表示电子传导是量子系统自然的属性，遵守费米统计。在同一年，Bloch证明电子是在周期性势场中运动的，这个定理允许我们通过布里渊区的波矢***k***来分辨电子态。

&emsp; 在1931年，Wilson展示了Bloch定理的物理形式，可以把晶体分为金属，半导体，和绝缘体。基于此，能带结构的概念在固体物理中被广泛接受。

&emsp; Winger和Seitz（1934年）首先获得了关于金属Na基态的数值结果。基于cellular方法，他们使用实验上关于原子势的数据计算了导带底的能量。

&emsp; 在计算能带结构中，关键的问题是选择原子势。在Hartree-Fock近似下，原子势必须自洽获得。然而，交换相互作用导致了非局域势，这使计算变得困难。为了规避这种困难，Slater（1934年）提出了一种简单的表达式，在自由电子气模型中（电子密度是常数）是可行的。Slater表明在非统一的电子密度下，局域势的表达式相同。随后（1965年），Slater引入了一个无量纲的参数α计算局域势，参数可以通过与一个原子的总能量（在Hartree-Fock近似下获得的）对比获得。这种方法称为$X_{\alpha}$方法，被广泛应用了几十年了。在密度方法理论（DFT）框架下，一个关于电子关联能的合适的解释称为可能。Hohenberg和Kohn（1964年）证明：多电子体系的所有基态特性可以只被密度的泛函描述。Kohn和Sham（1965年和1966年）表明：单粒子波函数是一个类似于薛定谔方程的解，这些单电子波函数决定了电子密度，势能是外势和有效局域交换关联势的总和。

&emsp; 事实证明，在很多实际应用中，交换关联势可以近似在均匀电子气中电子-电子相互作用的能量中得到，$ \varepsilon_{XC} $（局域密度近似，LDA）。如果$ \varepsilon_{XC} $被带入到Hartree-Fock交换能中，$ \varepsilon_X $，由此产生的势能是当α=2/3时的$ X_{\alpha} $势。由此DFT为由Hartree，Fock，和Slater提出的自洽场技术提供了必要的理论背景。

&emsp; 密度泛函理论描述基态的理论。当考虑激发态时，体系产生了电子-空穴对，需要考虑两粒子的关联效应。Landau发现激发谱的一个普遍特征，原激发（elementary excitations）表现准粒子行为的系统是多费米子系统。

&emsp; 在Landau理论中，费米液体具有准粒子的色散法则（dispresion law）特征，该法则被定义为总能量对分布函数的变分倒数，关联函数解释为准粒子的相互作用，如果这种相互作用很小，单粒子方法是可行的。一般来说，为了获得多粒子系统的原激发谱就必须要确定Green函数的极（poles），Green函数满足Dyson方程，它包含一个非局域的自能算符来描述交换-关联效应。Hedin和Laundqvist（1971年）表示在价带中自能算符的能量依赖可以忽略。

&emsp; 在这种情况下，Dyson方程可以简化为一个简单的方程，通过DFT可以求解，他们有相同的交换关联势$V_{XC}$。换句话来说，很多情况下，Landau关联函数可以设置为0，准粒子之间的相互作用可以被忽略。如果能带比较宽并且相同位置的电子相互作用不太强，此时单粒子方法是可行的。

&emsp; 能带理论的发展经历了三个阶段：第一阶段，从十九世纪三十年代中期到五十年代中期，发展了能带理论的基本理论，cellular方法（Wigner和Seitz，1934年），APW方法（augmented plane wave，Slater，1937），OPW方法（orthogonalized plane waves，Herring，1940）在产生赝势的概念和KKR方法（or the Green函数方法；Korringa，1947；Kohn和Rostocker，1940）中扮演了重要的角色，在这里时期，没有现实晶体能带结构的数值计算方法。第二阶段，持续到十九世纪七十年代中期，精心设计的计算机代码被开发出来，开展了大量的能带结构模拟。此外，不同方法的数学关系被评估了。第三阶段，由线性理论（linear methods）概念的出现而开启（Andersen，1975年），在很短的时间内，出现了很多方法，包括：LMTO（linear method of MT-orbitals，Andersen，1975年），linear APW（Andersen，ref-15，1975年；Koelling和Arbman，1975年；Takeda和Kubler，1979年），ASW（augmented spherical waves，Williams，Kubler，Gillat，1979年），linear KKR（Pettifor，1972年；Wonn等人，1974年），TB-LMTO（Anderson和Jepsen，1984年），和LASO（linear method of augmented Slater orbitals，Davenport，1984年）。这些方法使计算速度提高了100倍。

&emsp; 为了对复杂材料的物理性质获得深入的理解，建立电子结构和多变的物理效应之间的关系是必要的。使用能带理论的线性方法可以解决这个问题。

&emsp; 需要注意的是，在很长的时间里，固体物理的发展独立于能带结构的模拟。一般来说，为了描述电子系统，必须要引入一个有效的哈密顿量，在该哈密顿量中包含一些列需要拟合的参数，这就暗示了为了描述一个特定物质的性质需要选取一系列的参数，比如说，在离子晶体的铁磁理论中有Heisenberg哈密顿量，轻掺杂磁性合金中有Adersen哈密顿量，在超导理论中有BCS哈密顿量。第一个例子中的有效哈密顿量是由交换积分决定的，在第二个例子的哈密顿量中，两个反平行自旋电子的库伦排斥能是参数，他们占据在相同的d轨道，在局域d态和导带态之间有相同的矩阵元，BCS有效哈密顿量是由费米能级的态密度和电子-电子相互作用决定的。近年来，构建有效的哈密顿量和能带方法之间的差距缩小了。由于多体理论的进步，我们期待可以构建一个更加精确的有效晶格有效势。另一方面，在很多工作中，晶体的能带结构模拟被用来获得有效哈密顿量中的参数。除此之外，能带结构模拟对理解实验也是非常必要的。比如，能带计算在解释晶体的光学吸收和光子发射是必不可少的，当然也包括电磁场存在下，由费米面上电子的行为决定的其他性质。

&emsp; 今天，能带理论在物理世界中占有稳固的位置。然而，在掌握这一理论上存在技术上的问题。这本书就是为了降低学习该理论的难度。

[微信公众号](https://mp.weixin.qq.com/s/-iQy2ahAFiZrYZTQvrFW7A "Computational Methods in Solid State Physics: Perface")

## Reference
- Nemoshkalenko V V, Antonov N V. Computational methods in solid state physics[M]. CRC Press, 1999.
