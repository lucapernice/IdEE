---
layout: post
title: "Everything You Need to Know About Superconductivity."
author: thomas
categories: [ physics, science ]
image: assets/images/foto superconduttore bloccato.png
beforetoc: "In the realm of physics, few phenomena captivate scientists and engineers like superconductivity. This fascinating property, discovered over a century ago, continues to intrigue researchers for its revolutionary potential in technologies ranging from power transmission to medical imaging. Superconductivity defies conventional understanding by allowing certain materials to conduct electricity with zero resistance at extremely low temperatures. As we delve deeper into the mechanisms behind superconductivity and its applications, new frontiers emerge in our quest for efficient and sustainable technologies. This article explores the principles of this fascinating phenomenon, aiming to explain it in a simple yet comprehensive and exhaustive manner."
toc: true
---

## What is a Superconductor?

Superconductors are materials that, under certain conditions of temperature, can conduct electric current with zero resistance. This property is monumental in physics and technology because it eliminates the *Joule effect, where power dissipation (P*) in a conductor is given by the following formula:

$$P = RI^2$$

When resistance (*R*) approaches zero, power dissipation also becomes negligible. This breakthrough could revolutionize scientific research and technology, particularly in energy-saving applications for ecological transitions.

However, widespread adoption of superconductors faces challenges. These materials are typically expensive to produce, and their superconducting behavior occurs only at extremely low temperatures. Each superconductor has a *critical temperature* (*T~c~*), below which it exhibits superconductivity. In this paper we'll explore later on why this low-temperature requirement is crucial.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/grafico con resistance drop.jpeg" alt="Resistence_Drop" width="70%">
</div>

## Main known Superconductors

The first superconductive element, mercury (Hg), was discovered by  Heike Kamerlingh Onnes in 1911, and it was noticed that it had a critical temperature of approximately 4.2 K. Over time, researchers identified more materials with higher critical temperatures, making them easier to use practically. Notably, materials like YBa<sub>2</sub>Cu<sub>3</sub>O<sub>7</sub> exhibit superconductivity at temperatures above the boiling point of liquid nitrogen (77.2 K), enabling more accessible cooling methods. It's pretty funny noticing that actually YBa~2~Cu~3~O~7~ is an insulator at ambient temperature (as usual for ceramic materials), but it becomes superconductive below a certain temperature.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/tabella superconduttori con loro tc.png" alt="Tabella_Superconduttori" width="70%">
</div>

Today, various superconductors with unique properties, including perovskites, are known (link futuro articolo perovskiti). The ultimate goal remains discovering a material that exhibits superconductivity at ambient temperatures, which would be a game-changer in materials science.
This is what actually humanity thought she did during the summer of 2023, when some South Koreans scientists announced the discovery of an ambient temperature superconductor: the LK99. It was then found out that this discovery wasn't actually true (link al futuro articolo dell'LK99).

## The Physical Principles Behind Superconductivity

### The BCS Theory
BCS stands for "Bardeen Cooper Schrieffer", the three physicists who proposed this model, which earned them the Nobel prize for physics in 1972.
This theory can explain why superconductors have null electrical resistance. Later on we'll see few more physic phenomena related to superconductivity.

#### Cooper pairs
In the world of condensed matter physics, we can think of a conductor microscopically as a lattice of positive ions immersed in a sea of electrons that are free to move from one point to another. The efficiency of electron transport, or conductivity, depends on how frequently electrons collide with ions.

Achieving R=0 (zero resistance) implies no collisions between ions and electrons. This remarkable behavior is explained by the concept of *Cooper pairs* introduced by the BCS theory.

The BCS theory proposes that there can be an attractive interaction between two electrons in a superconducting lattice. This may seem counterintuitive, as we typically expect particles with the same negative charge to repel each other.

Consider one electron (*Electron #1) traveling through a conductive lattice along a certain path. Due to its negative charge, Electron #1 attracts the positive ions surrounding it, creating a region within the crystal lattice with a higher density of positive charge. This localized positive charge density then attracts more electrons in the same direction of movement. Each itinerant electron can thus be associated with a following electron (Electron #2*).

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/immagince electron1 e electron2.jpeg" alt="elettroni" width="70%">
</div>

These pairs of electrons, where one electron effectively trails another, are known as *Cooper pairs*. This cooperative pairing mechanism, facilitated by lattice distortions and attractive interactions between electrons, is fundamental to understanding superconductivity.

#### The effect of temperature
Of course, it's only possible to observe this effect when the electromagnetic interaction between electrons and ions is the dominant force acting within the crystal. This requires that the thermal energy be lower than a certain threshold, below which the vibrations of the ions have a negligible effect compared to the interaction of Cooper pairs.

Given that the average kinetic energy is proportional to Boltzmann's constant (*k~B~) times the temperature, the critical level (E~c~*) at which superconductivity occurs can be expressed as:

$$E_c \propto k_B T_c$$

Here, \(T~c~) represents the critical temperature discussed earlier.

The BCS theory also provides a formula to calculate the critical temperature:

$$T_c = T_D \exp \left[ -\frac{1}{n(0)V} \right]$$

Where:
1. T~D~is the Debye temperature,
2. n(0) is the density of states at the Fermi level,
3. V is the coupling energy between phonons and electrons.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/foto penetrazione campo magnetico.jpeg" alt="penetrazione" width="70%">
</div>

### Type I and Type II Superconductors
Superconductors can be divided in two types, based on their reaction to a magnetic field. More specifically they can expel the magnetic field in two different ways.

#### Type I superconductors
This category is formed by those superconductors which give Meissner effect just exactly how we described it before: they just expel every type of magnetic field flux. This means that:

$$Mμ_{0}+B_{ext}=B_{int}=0 $$ 

$$⟹B_{ext}=-Mμ_{0}$$

where of course M is the magnetization field. 
It' clear that there's a linear dependence between M and B.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/plot M-B.jpeg" alt="plot" width="70%">
</div>

Actually I can see that, after a critical value of the external magnetic field (*B~c~*), the superconductor is no more able to contrast it, so from here on it can start flowing through the sample undisturbed.

#### Type II  superconductors

In type II superconductors, we can distinguish three different regimes based on the value of the magnetic field to which the superconductor is exposed, separated by two critical values (*B~c1~* and *B~c2~*).

1.  *At 0 < B < B~c1~*: The behavior of the sample is similar to that of type I superconductors, exhibiting the classic Meissner effect where the magnetic field is simply repelled.
    
2.  *At B~c1~ < B < B~c2~: The system enters a **mixed phase*, where the magnetization of the sample partially opposes the external magnetic field, allowing part of the field to penetrate the material (we will discuss this further later).
    
3.  *At B > B~c2~*: The magnetization of the superconductor is no longer present, and the external magnetic field passes through the sample undisturbed.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/grafico tre regimi.png" alt="regimi" width="70%">
</div>

We can observe that in the mixed phase, there is no linear dependence between the magnetic field B and the magnetization M. 
When the sample is in this regime, magnetic fields concentrate in tubes, leading to the formation of vortex currents.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/foto tubi di flusso.png" alt="tubi" width="70%">
</div>

This causes the superconductive sample to lock its orientation in space when subjected to an appropriate magnetic field.

<div style="text-align:center">
  <img src="{{ site.baseurl }}/assets/images/foto superconduttore bloccato.png" alt="bloccato" width="70%">
</div>

Since part of the magnetic field can penetrate inside the material in the mixed phase, the superconductor repels less magnetic field compared to the case where all the field is expelled. This is why type II superconductors typically have a higher critical magnetic field value (B~c2~) compared to type I superconductors.
