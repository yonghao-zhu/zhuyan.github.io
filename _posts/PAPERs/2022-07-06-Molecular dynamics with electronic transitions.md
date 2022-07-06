---
layout: post
toc: true
title: "Molecular dynamics with electronic transitions"
categories: Papers
tags: [NA-MD]
author:
  - John C. Tully
---

<img src="https://yonghao-zhu.github.io/zhuyan.github.io/imags/library/person/John C. Tully.jpg" width="40%">
[John C. Tully](https://chem.yale.edu/faculty/john-tully "John C. Tully") 

[J. Chem. Phys. 93, 1061(1990)](https://doi.org/10.1063.1.459170 "Molecular dynamics with electronic transitions")

# ABSTRACT

&emsp; A method is proposed for carrying out molecular dynamics simulations of processes that involve electronic transitions. The time dependent electronic Schrödinger equation is solved self-consistently with the classical mechanical equations of motion of the atoms. At each integration time step a decision is made whether to switch electronic states, according to probabilistic ‘‘fewest switches’’ algorithm. If a switch occurs, the component of velocity in the direction of the nonadiabatic coupling vector is adjusted to conserve energy. The procedure allows electronic transitions to occur anywhere among any number of coupled states, governed by the quantum mechanical probabilities. The method is tested against accurate quantal calculations for three one-dimensional, two-state models, two of which have been specifically designed to challenge any such mixed classical–quantal dynamical theory. Although there are some discrepancies, initial indications are encouraging. The model should be applicable to a wide variety of gas-phase and condensed-phase phenomena occurring even down to thermal energies.

# INTRODUCTION
&emsp; The molecular dynamics technique has proved to be a very powerful tool for elucidating gas-phase and codensed-phase dynamical processes. The method is founded on the assumption that atomic motions are governed by classical mechanics subject to some appropriate multidimensional force field. Limitations of the method are well known. There may be practical difficuties with constructing accurate force fields, including large mumbers of atoms, integrating for long times, or achieving accurate statistical sampings. There are also fundamental limitations that result from the basic assumptions of the method; quantum mechanical behavior is neglected and a single potential energy surface governs the motion. Quantal effects such as tunneling, interference and level quantization can be significant, particularly in low-energy processes involving hydrogen atom motion. Of at least comparable importance is the restriction to motion on a single potential energy surface. To each nondegenerate electronic state of a many atom system there corresponds a distinct Born-Oppenheimer potential energy surface. When a transition between electronic states occurs, the forces experienced by the atoms therefore change, often drastically. Proper incorporation of these effects can be crucial for describing a host of dynamical processes, including carrier recombination at surfaces or in condensed phases, photochemistry, radiationless transitions, laser or electron induced chemistry, dynamics at metal surfaces, and electron transfer in molecular, biological, interfacial, or electrochemical systems. In addition, the same considerations apply to other mixed quantal-classical situations not involving electronic transitions, e.g., vibrational relaxation in liquids.

&emsp; The objective of this paper is to introduce a practical molecular dynamics method that accurately incorporates the effects of electronic transitions. The greatest advantage of the molecular dynamics approach is its ability to treat complicated many atom systems in full dimensionality. This practicality arises from the assumption that atoms obey classical mechanical equations of motion. We demand that this advantage be retained in the extended approach. Thus we require that atomic motions be described by classical-like trajectories. We make no attempt at incorporating quantum effects such as tunneling or zero-point motion, since current methods for doing this, even for motion on a single potential energy surface, require an enormous increase in computational effort over standard molecular dynamics. On the other hand, electronic transitions are inherently quantum mechanical and must be treated as such. Since the atomic trajectories determine the probabilities of electronic transitions and electronic transitions, in turn, strongly influence the forces governing the trajectories, the theory must treat self-consistently the classical and quantal degrees of freedom.

&emsp; The treatment of nonadiabatic effects in molecular dynamics has a long history, with development of a host of classical, semiclassical, and quantum mechanical approaches. [ref: 1-39] The most widely applied method and that which is most closely related to the current approach is the "surface-hopping" method with its many variants. [ref: 7-10, 23-28] However, with the method proposed in this paper transitions can occur anywhere, not just at localized avoided crossings. Furthermore, any number of coupled electronic states can be included, and quantum coherences between different "state switches" are maintained.

&emsp; The objective of this work, to incorporate one kind of quantum effect (electronic transitions) while ignoring others (tunneling, zero-point motion, etc.) may appear inconsistent. But, to the extent that the Born-Oppenheimer separation of electronic and atomic motions is valid, the prominence of the two kinds of quantum effects are controlled by independent "small parameters" and there is no inconsistency in addressing either separately. The importance of tunneling and level quantization effects depends on the ratio of the atomic wavelength to the characteristic range of the potential. Thus these quantum effects are diminished in systems involving large atomic masses and large velocities. On the other hand, electronic transitions are controlled primarily by the separation between electronic energy levels, a property that is independent of atomic masses. For example, for a simple two-state avoided crossing**, electronic transitions are probable if the so-called Massey parameter $\zeta$ is of order unity

$$\zeta=\left|\frac{\hbar \mathbf{\dot{\mathrm{z}}} \cdot \mathbf{\mathrm{d}_{12}}} {V_{1}-V_{2}}\right| \gtrsim 1    (1) $$                

where $V_1$ and $V_1$ are the energies of the two adiabatic states at the position of the avoided crossing, $\mathbf{\dot{\mathrm{z}}}$ is the atomic velocity vector, and $\mathbf{d_{12}}$ is the nonadiabatic coupling vector to be defined below. Mass does not appear in this expression, and transitions are more probable at high velocities $\mathbf{\dot{\mathrm{z}}}$ in contrast to the other quantum effects. Thus, it is proper to construct a theory which treats atomic motion in the short wavelength (classical) limit, while retaining effects of electronic transitions. Of course, any theory which attempts to combine quantal and classical degrees of freedom will ultimately encounter limits in which it fails. Our hope is to develop a method for which the range of useful accuracy will encompass most realistic systems of interest.

&emsp; In the next section we present a list of attributes that are desireable, if not essential, for any approach that incorporates electronic transitions into molecular dynamics. We then propose a specific method, possibly the simplest that displays most of these attributes. In Sec. IV we test the proposed method against accurate quantum mechanical solutions of three model problems. We discuss the promise and limitations of the method in the final section.

[剩下的就不copy了，直接到我的notion中查看吧！](https://yonghaozhu.notion.site/1-John-C-Tully-Molecular-dynamics-with-electronic-transitions-3f6168acbee54c0db447617b404632ed "My Notion")
