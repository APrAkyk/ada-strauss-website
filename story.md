---
layout: cayman
---

# Introduction

As reported by the [New York Times Magazine](https://www.nytimes.com/2017/08/03/magazine/for-the-new-far-right-youtube-has-become-the-new-talk-radio.htm) in 2017, YouTube has become "the new Conservative talk radio" for the far right. Moreover, in 2019, [Kevin Roose depicted ](https://www.nytimes.com/interactive/2019/06/08/technology/youtube-radical.html) "countless" stories of young men, looking for direction or distraction on YouTube, ending up "seduced by a community of far-right creators". The existence of a radicalization pipeline on Youtube was strongly suggested by the study [“Auditing Radicalization Pathways on Youtube”, by Ribeiro et al. (2020)](https://dlab.epfl.ch/people/west/pub/HortaRibeiro-Ottoni-West-Almeida-Meira_FAT-20.pdf). 
From there, we would like to enlarge the scope of this research by studying the toxicity of the comments and the co-commenting activities in far right channel videos. 

Doing so, we would like to see if these channels generate more toxic behavior and isolate users. Finally, this project could help find suitable solutions in order to reduce toxicity and attenuate far-right radicalization.

To study far-right wing channels on Youtube, our study will be based on the data and the results coming from Ribeiro et al. (2020) study. The studied channels are broadly classified into four types: Media (the control group), the Alt-lite, the Intellectual Dark Web (I.D.W) and the Alt-right. 

# Toxicity
## How to measure toxicity ?

[_Detoxify_](https://github.com/unitaryai/detoxify) is a machine learning model which rates the toxicity of a comment on a scale from 0 to 1 (0 not at all, 1 very much). Furthermore, it detects if it fits into these subcategories of toxicity: **severe_toxicity**, **obscene**, **identity_attack**, **insult**, **threat**, **sexual_explicit**. A comment is rated 1 in toxicity if it is a very ‘hateful, aggressive, or disrespectful that is very likely to make you leave a discussion or give up on sharing your perspective’. 

[include example of application of Detoxify, see notebook in to delete/toxic_examples.ipynb . Either include the table, or it would be fun to include “un curseur où l’utilisateur peut choisir le degré de toxiticité”. ]

<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

    <label for="pet-select">Choose a pet:</label>

    <select name="pets" id="pet-select">
      <option value="">--Please choose an option--</option>
      <option value="dog">Dog</option>
      <option value="cat">Cat</option>
    </select>

    <img id="graphique-1" src="../assets/img/profilAriane.png" />

<script>
    const selectEl = document.getElementById("pet-select");
    selectEl.addEventListener("change", (ev) => {
    console.log("yoooo")
    switch (selectEl.value) {
        case "dog":
        document.getElementById("graphique-1").src = "../assets/img/favicon.png";
        break;
        case "cat":
        document.getElementById("graphique-1").src = "../assets/img/favicon.png";
        break;
        default:
        document.getElementById("graphique-1").src="assets/img/profilAriane.png";
        document.getElementById("graphique-1").src = "../assets/img/profilAriane.png";
        break;
    }
    })
</script>

## Process

![Stay toxic](https://www.selfies.com/wp-content/uploads/sites/5/2022/07/Mutausbrueche-TikTok-Stay-Toxic.jpg)(https://www.selfies.com/apps/instagram/stay-toxic-lustiger-social-media-trend-tiktok-insta-beziehungstipps-141719/)






