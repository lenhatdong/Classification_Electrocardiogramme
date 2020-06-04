# Classification_Electrocardiogramme
(C'est un des premiers pas pour la Science de données)

(Télécharger les données sur ce [lien](https://drive.google.com/drive/folders/17CUab46-Syxx8zvjhIpCBnpf-5QpDaCz?usp=sharing)

Inspriré de la [recherche](https://arxiv.org/pdf/1805.00794.pdf) **"ECG Heartbeat Classification: A Deep TransferableRepresentationMohammad Kachuee, Shayan Fazeli, Majid SarrafzadehUniversity of California, Los Angeles"**, qui utilise les réseau de neurones pour prédire 5 classes d'ECG, détaillées dans le tableau suivant. Le jeu de données est constitué de 87554 electrocardiogrammes échantillonés à la fréquence de 125hz,c’est-à-dire une valeur toutes les 0,008 secondes. On a donc pour chacun des signaux 187 valeurs sur 1,488s.


| Category(data)        |  Category(Paper)     | Annotations  |
| ------------- |:-------------:| -----:|
|0|N| <ul><li>Normal</li><li>Left/Right bundle branch block</li><li>Arial escape</li><li>Nodal escape</li></ul>  |
|1|S| <ul><li>Atrial premature</li><li>Aberrant atrial premature</li><li>Nodal premature</li><li>Supra-ventricular premature</li></ul> |
|2|V| <ul><li>Premature ventricular contraction</li><li>Ventricular escape</li></ul> |
|3|F| <ul><li>Fusion of ventricular and normal</li></ul> |
|4|Q| <ul><li>Paced</li><li>Fusion of paced and normal</li><li>Unclassifiable</li></ul> |

Pourtant, la classe **N** bien domine les autres classes (plus de 80% de données). Donc le modèle a la tendance de prédire les autres classes dans la classe **N**

Dans ce projet, nous essayons de mettre en pratique nos connaissances en apprentissage statistique pour faire la prévision de la catégorie des battements cardiaques. Pour ce faire, nous augmentons des données pour équilibrer les classes et pour mieux apprendre. Ensuite, les analyses axploratoires par l'ACP et l'AFD avant de passer en modélisation. Nous utilisons les méthodes classiques (Logit, Arbre de décision, Random forest, XGB, SVM et réseau de neurones) pour prédire et comparer leur précision. C'est aussi 2eme but de projet: famialiser et comparer des méthodes de classification, et construire des réseaux de neurones.

Nous avons 2 pistes pour exploiter des données:
1. Utiliser des caractéristiques des signaux (moyenne, variance, min, max, entropie,...)
2. Utiliser des ondelettes (avec seuillage ou non)

