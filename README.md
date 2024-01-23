<p align="center">
  <img width="300px" src="img/logo.png" />
  <h1 align="center">Welcome!</a></h1>
</p>

This GitHub page contains projects related to my research, as well as some older projects that I have archived for reference.

[![Website](https://img.shields.io/website?up_color=olivegreen&url=https%3A%2F%2Fwww.normalesup.org%2F~tuyeras%2F&style=for-the-badge&label=Webpage)](https://www.normalesup.org/~tuyeras/)
[![Twitter Follow](https://img.shields.io/twitter/follow/Rtuyeras?label=%40Rtuyeras&style=for-the-badge&logo=X&labelColor=black&color=grey)](https://twitter.com/rtuyeras?lang=en)
[![Website](https://img.shields.io/website?up_message=%20&up_color=dodgerblue&url=https%3A%2F%2Fhub.docker.com%2Fu%2Frtuyeras&style=for-the-badge&logo=Docker&label=Docker)
](https://hub.docker.com/u/rtuyeras)

![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=remytuyeras\&rank_icon=github)](https://github.com/anuraghazra/github-readme-stats)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=remytuyeras&layout=compact)
<br>

<p align="center">
  <h1 align="center">What I currently work on</h1>
</p>

I strongly believe that the future of genomics will depend on our ability to go beyond traditional approaches and adopt a more holistic view of complex problems. 
Current challenges include the **privacy of genomic data** and the lack of flexible tools for studying **complex genetic effects**. To address these challenges, I have developed several Python libraries that allow researchers to simulate realistic variant call data and study complex genetic effects using novel analytical techniques from post-modern algebra.

<br>

<p align="center">
  <img width="130px" src="img/haplo-logo.png"/>
  <h2 align="center"><a href="https://github.com/remytuyeras/HaploDynamics">HaploDynamics</a></h2>
</p>

![GitHub issues](https://img.shields.io/github/issues-raw/remytuyeras/HaploDynamics?style=for-the-badge&logo=Github&color=purple)
![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/remytuyeras/HaploDynamics?style=for-the-badge&logo=Github&color=purple)

This is a cloud-native software framework for fast generation of genomic data simulations. One of the features I am currently working on is to make this project composable with the user's models for specific mutation profiles or genetic positioning. 

$$\begin{array}{ccccccc}
\mathsf{User}&&\mathop{\longrightarrow}\limits^{\fbox{1}}&&(x_{1},x_{2},\dots,x_{n})&&\\
^{\fbox{2}}\downarrow&&&&\downarrow&&\\
(x_{1},x_{2},\dots,x_{n}) &\longrightarrow& \fbox{$\mathsf{UserModel}$} &\longrightarrow& \fbox{$\mathsf{HaploDXModel}$}& \longrightarrow &\fbox{$\mathsf{VCFData}$}\\
\end{array}$$

So far, users have control on:
  1. population-specific LD decay profiles
  2. bottleneck parameters
  3. allele frequency spectra (and/or mutation rate profiles)
  4. LD block lengths
  5. genetic position values

In the near future, the ```HaploDynamics.Framework``` module will include an arithmetic to manipulate the generated VCF files (or in fact any VCF file).

<br>

<p align="center">
  <img width="150px" src="img/logo.png"/>
  <h2 align="center"><a href="https://github.com/remytuyeras/pedigrad-library">Pedigrad Library</a></h2>
</p>

![GitHub issues](https://img.shields.io/github/issues-raw/remytuyeras/pedigrad-library?style=for-the-badge&logo=Github&color=purple)
![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/remytuyeras/pedigrad-library?style=for-the-badge&logo=Github&color=purple)

I have been working on this software for the last five years to fully implement the framework developed in <a href="https://arxiv.org/abs/1708.05255">CTG</a>, <a href="https://arxiv.org/abs/1805.07002">CTGI</a> \& <a href="https://arxiv.org/abs/1805.07004">CTGII</a> . I intend to publish a new version of this framework **soon**, inclduing new semigroup-based linear algebra features to find combinatorial genetic effects from variant call and phenotype data. Overall,  the ```Pedigrad``` library will provide a new paradigm for doing machine learning on genomic data and learn combinatorial relationships.

$$\begin{array}{c|c|c|c}
\textbf{A pedigrad} & \textbf{A segment} & \to & \textbf{A semigroup of haplotypes}\\
\hline
\textit{the framework provided} & \textit{where learning events occur} & \to & \textit{where algebraic operations are used}\\
\textit{by the library} & \textit{to find genetic interactions} & \to & \textit{to guide the learning}\\
\hline
&&&\\
P:&(\bullet\bullet\dots\bullet\bullet)\dots(\bullet\bullet\dots\bullet\bullet) & \mapsto & \lbrace\sum_i x_i = \sum_i y_i~|~x_i,y_i\textrm{ haplotypes}\rbrace\\
&&&\\
\end{array}$$

On the long term, the ```Pedigrad``` library will also be used to complete the simulations of the ```HaploDynamics``` library with complex genomic architecture generations (e.g. variant interactions, complex phenotypes, environment modeling etc.).

<br>

<p align="center">
  <img width="110px" src="img/logo-fhe.png"/>
  <h2 align="center"><a href="https://github.com/remytuyeras/aces">ACES (FHE scheme)</a>a></h2>
</p>

This project constains the code developed for a paper detailing the design of a fully homomorphic encryption scheme. The outcomes of this work bear significance in the domains of machine learning and privacy computing.


