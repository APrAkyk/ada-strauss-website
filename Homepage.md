---
layout: homepage
title: Strauss project
---

# Introduction

As reported by the [New York Times Magazine](https://www.nytimes.com/2017/08/03/magazine/for-the-new-far-right-youtube-has-become-the-new-talk-radio.htm) in 2017, YouTube has become "the new Conservative talk radio" for the far right. Moreover, in 2019, [Kevin Roose depicted ](https://www.nytimes.com/interactive/2019/06/08/technology/youtube-radical.html) "countless" stories of young men, looking for direction or distraction on YouTube, ending up "seduced by a community of far-right creators". The existence of a radicalization pipeline on Youtube was strongly suggested by the study [“Auditing Radicalization Pathways on Youtube”, by Ribeiro et al. (2020)](https://dlab.epfl.ch/people/west/pub/HortaRibeiro-Ottoni-West-Almeida-Meira_FAT-20.pdf). 
From there, we would like to enlarge the scope of this research by studying the toxicity of the comments and the co-commenting activities in far right channel videos. 

Doing so, we would like to see if these channels generate more toxic behavior and isolate users. Finally, this project could help find suitable solutions in order to reduce toxicity and attenuate far-right radicalization.

To study far-right wing channels on Youtube, our study will be based on the data and the results coming from Ribeiro et al. (2020) study. The studied channels are broadly classified into four types: Media (the control group), the Alt-lite, the Intellectual Dark Web (I.D.W) and the Alt-right. 

<p align="center">
    <img width="500" src="assets/img/graph_intro.png" >
</p>

<p align="center">
    <a href="https://medium.com/2key/thegraph-how-to-build-our-subgraph-on-thegraph-hosted-solution-2360938c0323"><i>Is it me or is it hot in here?</i></a>
</p>

Our goal in this part is to compute how tight knit the extreme communities Alt-lite, IDW and Alt-right are. To this end, we’ll define a graph where the nodes represent youtube channels (not necessarily associated to extreme communities) and edges represent their influence on each other. We’ll then compute cluster coefficient to quantify the influence of the channels on each other.

<p align="center" style="color :BurlyWood; ">
    <i>“The wise man doesn't give the right answers, he poses the right questions”<i>

<p align="right " style="color :cadetblue; ">
    - Claude Levi-Strauss
</p>

# Acknowledgement 

We would like to thank [Manoel Ribeiro](https://manoelhortaribeiro.github.io/) for helping  his helpful remarks. We were able to successfully complete this project with his guidance and the data that he kindly shared with us. <br>  
His paper was also very helpful to understand the data we were working on. 
[YouNiverse: Large-Scale Channel and Video Metadatafrom English-Speaking YouTub](https://ojs.aaai.org/index.php/ICWSM/article/view/18125/17928)

# Credential

YouNiverse dataset : [Youniverse](https://zenodo.org/record/4650046#.Y3eNQceZO3-)

Paper of Ribeiro was very helpful to understand the data we were working on : 
[YouNiverse: Large-Scale Channel and Video Metadatafrom English-Speaking YouTub](https://ojs.aaai.org/index.php/ICWSM/article/view/18125/17928)

Paper used to calculate the local clustering coefficient computing for the clustering : 
[Directed clustering in weighted networks: A new perspective](https://www.sciencedirect.com/science/article/abs/pii/S096007791730509X?via%3Dihub)

We use a server to be able compute of the large amount of data from the YouNiverse dataset : [Server](https://www.vultr.com/)

Machine learning model which rates the toxicity : [Detoxify](https://github.com/unitaryai/detoxify)



