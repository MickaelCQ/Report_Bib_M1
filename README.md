# Résumé
Au CHU de Nîmes, l’arrivée du Séquençage Haut Débit (SHD) a produit une ava-
lanche de données, augmentant considérablement l’efficacité diagnostique de la Sclérose
Latérale Amyotrophique (SLA). Cette évolution reste insuffisante pour identifier une
éventuelle cause génétique chez de nombreux patients. Pour tenter d’y remédier, il est
intéressant d’élargir le spectre d’analyse en s’intéressant à l’Acide RiboNucléique (ARN).
Cette approche dite ’multiomique’ permettrait de d’identifier d’éventuelles anomalies qui
affectent l’épissage. Ces événements génétiques altérant l’ARN sont fréquents, selon la
Human Gene Mutation Database (HGMD), 8 % des événements mutationnels documen-
tés affectent l’épissage, toutes maladies génétiques confondues. [2]. Cette donnée vient
consolider la volonté du laboratoire d’étendre son activité au RNA-Seq. In fine, cette évo-
lution implique l’élaboration d’un pipeline de d’analyse bioinformatique.
Ce travail traite d’une de ses étapes, la normalisation. Son intérêt réside dans la cor-
rection des biais inhérents à l’expérience. Elle permet de rendre les résultats des patients
comparables entre eux, ce qui facilite la caractérisation d’une différence d’expression pour
un gène particulier, qui pourrait se traduire, par exemple, par une haploinsuffisance et
donc permettre de statuer sur la causalité génétique de la maladie. Cette étude s’attarde
sur les concepts statistiques et leur mise en oeuvre. Nous nous concentrons sur les fonc-
tions proposées par la bibliothèque edgeR, bien qu’il en existe d’autres. Dans certains
cas, nous proposons des formulations en langage R pour examiner plus en détail les effets.
Enfin nous parlons d’un outil qui compile différentes méthodes de normalisation, Normseq.
La normalisation des données RNA-Seq peut se faire sur divers paramètres d’entrée
tels que la taille des gènes, la composition de la bibliothèque et le nombre de comptages.
La diversité des méthodes présentées dans ce travail peut paraître déroutante , car comme
souvent en bioinformatique, il n’existe pas de consensus sur la stratégie à adopter. Les
outils dépendent fortement des caractéristiques du jeu de données et de la problématique
biologique. Par ailleurs, ce rapport peut être considéré comme une étude méthodologique
pour être exploité au sein du CHU de Nîmes sur un jeu de données réel. Une stratégie
envisageable serait une étude comparative avec les données spécifiques du panel de gènes
SLA
