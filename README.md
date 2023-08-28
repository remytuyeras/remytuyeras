<p align="center">
  <img width="300px" src="img/logo.png" />
</p>

## Hello there!
On this github you will find projects related to my research as well as some very old school projects that I put here for storage purposes.

## What I currently focus on

### [HaploDynamics](https://github.com/remytuyeras/HaploDynamics)
This is a cloud-native software framework for fast generation of genomic data simulations. One of the features I am currently working on is to make this project composable with the user's models for specific mutation profiles or genetic positioning. 

$$\begin{array}{ccccccc}
\mathsf{User}&&\mathop{\longrightarrow}\limits^{\fbox{1}}&&(x_{1},x_{2},\dots,x_{n})&&\\
^{\fbox{2}}\downarrow&&&&\downarrow&&\\
(x_{1},x_{2},\dots,x_{n}) &\longrightarrow& \fbox{$\mathsf{UserModel}$} &\longrightarrow& \fbox{$\mathsf{HaploDXModel}$}& \longrightarrow &\fbox{$\mathsf{VCFData}$}\\
\end{array}$$

So far, users have control on:
- mutation rates
- lengths of LD blocks
- genetic position values

### [Pedigrad](https://github.com/remytuyeras/pedigrad-library)
This is a software I have been working on for the last five years. I intend to publish a new version soon, with some semigroup linear algebra features that you can use to find combinatorial genetic effects from variant call and phenotype data. On the long term, the ```Pedigrad``` library will complete the simulations of the ```HaploDynamics``` library with phenotype simulations.

### Homomorphic Encryption
I intend to add a project on a new model for Homomorphic Encryption. More to come later this year.


