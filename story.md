---
layout: cayman
title: Strauss project
---

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

<img id="graphique-1" src="assets/img/profilAriane.png" />

<script>
    const selectEl = document.getElementById("pet-select");
    selectEl.addEventListener("change", (ev) => {
    switch (selectEl.value) {
        case "dog":
        document.getElementById("graphique-1").src = "assets/img/favicon.png";
        break;
        case "cat":
        document.getElementById("graphique-1").src = "assets/img/favicon.png";
        break;
        default:
        document.getElementById("graphique-1").src="assets/img/profilAriane.png";
        document.getElementById("graphique-1").src = "assets/img/profilAriane.png";
        break;
    }
    })
</script>

## Process

<p align="center">
    <img width="500" src="https://www.selfies.com/wp-content/uploads/sites/5/2022/07/Mutausbrueche-TikTok-Stay-Toxic.jpg" >
</p>
<p align="center">
    <a href="https://www.selfies.com/apps/instagram/
stay-toxic-lustiger-social-media-trend-tiktok-insta-beziehungstipps-141719/">Source</a>
</p>

<p align="center">
    <img width="300" src="http://img.picturequotes.com/2/428/427713/have-you-been-playing-in-toxic-waste-lately-quote-1.jpg" >
</p>

<p align="center">
    <a href="http://www.picturequotes.com/have-you-been-playing-in-toxic-waste-lately-quote-427713">Source</a>
</p>

<p align="center">
    <img width="500" src="assets/img/toxic_behaviour.png" >
</p>

<p align="center">
    <a href="https://www.pinterest.fr/pin/551761391849970879/">Source</a>
</p>

## Introduction

Some extreme communities are well known for making toxic comments. Taking Trump for example:

<p align="center">
    <img width="500" src="assets/img/trump.png" >
</p>

<p align="center">
    <a href="https://twitter.com/realDonaldTrump/status/332308211321425920">Twitter</a>
</p>


But how toxic is that tweet? Thankfully, we’re using a Machine Learning model called Detoxify to compute how toxic a sentence is and how severe-toxic, obscene, threatening, sexually explicit, identity attacking  and threatening it is. It rates it on a scale from 0 to 1 (0 not at all, 1 very). To get an idea, a comment is considered to have a toxicity of 1 if if it is a very ‘hateful, aggressive, or disrespectful that is very likely to make you leave a discussion or give up on sharing your perspective’. 
For example Trump’s tweet had a score of :

| Toxicity        | Severe toxicity  | Obscene  | Identity attack |  Insult  | Threat   | Sexual explicit |
|:----------------|:-----------------|:---------|:----------------|:---------|:-------- |:----------------|
|    0.994145     |     0.000396     | 0.004639 |     0.004734    | 0.988292 | 0.000295 |     0.000622    |

It has a toxicity of ~0.994 and is very insulting (insult~0.988). To get a better idea of what toxicity score is associated with what type of sentence, we’re introducing the monkey scale:
(scale of the monkey sequences and the corresponding monkey sentences)

<details open="open">
<summary>Toxicity of 'The monkey makes jokes' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.080424</th>
    <th>0.000012</th>
    <th>0.000631</th>
    <th>0.001699</th>
    <th>0.045562</th>
    <th>0.000297</th>
    <th>0.000416</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The mean monkey makes means jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.158876</th>
    <th>0.000014</th>
    <th>0.000780</th>
    <th>0.002192</th>
    <th>0.123876</th>
    <th>0.000231</th>
    <th>0.000387</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The annoying monkey makes annoying jokes about means'</summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.197954</th>
    <th>0.000018</th>
    <th>0.001104</th>
    <th>0.002104</th>
    <th>0.139986</th>
    <th>0.000289</th>
    <th>0.000623</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The vile monkey makes vile jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.319232</th>
    <th>0.000017</th>
    <th>0.000790</th>
    <th>0.002627</th>
    <th>0.259821</th>
    <th>0.000322</th>
    <th>0.000463</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The malevolent monkey makes malevolent jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.462587</th>
    <th>0.000031</th>
    <th>0.001146</th>
    <th>0.003987</th>
    <th>0.397109</th>
    <th>0.000386</th>
    <th>0.000831</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The nasty monkey makes nasty jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.615834</th>
    <th>0.000024</th>
    <th>0.000813</th>
    <th>0.002809</th>
    <th>0.556885</th>
    <th>0.000381</th>
    <th>0.000466</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The despicable monkey makes despicable jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.707401</th>
    <th>0.000016</th>
    <th>0.000449</th>
    <th>0.001647</th>
    <th>0.657305</th>
    <th>0.000226</th>
    <th>0.000282</th>
  </tr>
</table>
</details>

<details>
<summary>Toxicity of 'The despicable monkey makes despicable jokes about means' </summary>

<table class="tb" id="members">
  <tr>
    <th>Toxicity</th>
    <th>Severe toxicity</th>
    <th>Obscene</th>
    <th>Identity attack</th>
    <th>Insult</th>
    <th>Threat</th>
    <th>Sexual explicit</th>
  </tr>
  <tr>
    <th>0.995640</th>
    <th>0.032880</th>
    <th>0.883254</th>
    <th>0.030733</th>
    <th>0.975668</th>
    <th>0.000906</th>
    <th>0.028742</th>
  </tr>
</table>
</details>


Therefore we wondered if being toxic was one of the characteristic features of extreme communities. Just as in the study [“Auditing Radicalization Pathways on Youtube”, by Ribeiro et al. (2020)](https://dlab.epfl.ch/people/west/pub/HortaRibeiro-Ottoni-West-Almeida-Meira_FAT-20.pdf), we decided to study the extreme communities ‘Alt-right’, ‘Alt-left’ and ‘Intellectual Dark Web’ aka I.D.W and use medias as our control group. And hopefully twitter isn’t the only place where you can be toxic, there is also the comment section of youtube videos. 

<details>
  <summary id="mysummary"
           style="background: lightblue; outline: none;padding: 15px; 
                  border-radius: 50px;">Order 4A801</summary>
  <p>You sold 125 shares of MSFT at 11:29 AM</p>
  <p>You bought 200 shares of GOOG at 11:26 AM</p>
</details> 






