---
title: "Undergraduate Thesis Research (BUET)"
excerpt: "Developed an efficient computational tool on CPLM-2.0 database proposing a prediction scheme
based on evolutionary conserved information of protein sequences. The study explored the efficacy of
protein sequence based features and protein secondary structure for predicting Lysine Succinylation
sites using machine learning techniques. *(Click on the title for a brief overview)*
<br/>"
collection: projects
---
[Draft](https://joyantabasak13.github.io/files/Lys_Suc_Draft.pdf) of the article we wrote based on our thesis work.
* Supervised by [Dr.Md Sohel Rahman](https://cse.buet.ac.bd/faculty/facdetail.php?id=msrahman), Professor, CSE, BUET.

A Brief Note
------------
For details read the [draft article](https://joyantabasak13.github.io/files/Lys_Suc_Draft.pdf). <br>
For a quick overview, abstract is given in the following section. <br>
<em> Update: </em> I have later worked on far larger PLMD database. I will post it in future. <br>
<br>
The target of the research was to find an robust and efficient binary classifier to predict a lysine site (a amino acid in protein) have undergone succinylation or not. Succinylation is a posttranslational modification where a succinyl group (-CO-CH2-CH2-CO2H) is added to a lysine residue of a protein molecule.
<br>
Here I would mention the questions I tried to find answer to while we were conducting the research.

<dl>
  <dt><em>Why Some Features Perform Better?</em> </dt>
  <dd>There is no consensus in the literature on any particular feature or feature type to use. Prior researches explored many features including physico-chemical features, various positional encoding, protein primary & secondary structures. Although some features (protein structures) showed better discriminatory performance, why they perform better is not clear (yet). We noticed almost all of the recently explored better performing feature types are directly or indirectly dependent to the sequence. To gain better insight, we used simple features (n-gram, n-gapped-n-gram, position specific n-gram) extracted from the sequence directly. Our work shows some features (some certain gapped-bi-grams) are particularly better at discriminating the Lysine succinylation sites. It may help to explain the efficacy of some complex features in future. </dd>

  <dt><em>Is There Any Species-wise Difference?</em> </dt>
  <dd> Succinylation is spotted in variety of animal, plants and prokaryote species. As this PTM was discovered relatively recently (2010), investigations on different species are still going on. However, the current state-of-the-art predictors do not take account of any species specific variation which is probably due to low amount of per species samples. These works are based on CPLM 2.0 database which contains 893 unique proteins from 12 species. Later published PLMD database (2017) expanded the number of sequenced unique proteins to 6378 from 14 species. In my later work (not yet complete), I experimented with this dataset and tried to find out how the lysine site descriptions varied across species. </dd>

  <dt><em>How the Models Behave?</em></dt>
  <dd>Like any other ML task, finding out a better performing model is crucial. Succinylation prediction is relatively new problem and related field is still progressing. Hence an explainable model offering valuable insights might be more preferred to a slightly better performing black-box implementation. This compelled us to try ML algorithms that offer better monitoring capability. As more data becomes available, explainable deep learning techniques (for ex., attention mechanism) can be adopted.</dd>

</dl>

Abstract
---------
Post-translational modification (PTM) is a biological mechanism that expands protein functionality.
Among the PTMs, lysine succinylation substantially alter the structural and functional properties of
cellular proteins. This PTM is suspected to be implicated in numerous diseases regarding heart and
blood circulation. Recent proteomic studies spotted it in wide variety of both prokaryotic and eukaryotic
organisms. In reality, little is known about this particular PTM and its implications. The experimental
detection of lysine succinylation is expensive, time consuming and labor extensive. Which is why fast and
robust computational tools are absolutely necessary to process rapidly increasing number of sequenced
proteins and correctly categorize the concealed lysine residues. In this paper, we propose an efficient
model that optimizes different sequence based representations to approximate discriminating function.
This model reflects the efficacy of sequence information by **achieving 87.3% accuracy, 94.9% sensitivity,
81.1% specificity, 0.76 Matthews correlation coefficient, 0.94 AUROC and 0.91 AUPR**, which is comparable
performance to state-of-the-art predictors in lysine succinylated site prediction.
