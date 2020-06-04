# Classification_Electrocardiogramme
Inspriré de la recherche "ECG Heartbeat Classification: A Deep TransferableRepresentationMohammad Kachuee, Shayan Fazeli, Majid SarrafzadehUniversity of California, Los Angeles" [ici](https://arxiv.org/pdf/1805.00794.pdf), qui utilise les réseau de neurones pour prédire 5 classes d'ECG



Dans l'article expliquant tout ce processus  [ici](https://arxiv.org/pdf/1805.00794.pdf) nous trouvons la signification suivantes des différents labels ou catégories :


| Category(data)        |  Category(Paper)     | Annotations  |
| ------------- |:-------------:| -----:|
|0|N| <ul><li>Normal</li><li>Left/Right bundle branch block</li><li>Arial escape</li><li>Nodal escape</li></ul>  |
|1|S| <ul><li>Atrial premature</li><li>Aberrant atrial premature</li><li>Nodal premature</li><li>Supra-ventricular premature</li></ul> |
|2|V| <ul><li>Premature ventricular contraction</li><li>Ventricular escape</li></ul> |
|3|F| <ul><li>Fusion of ventricular and normal</li></ul> |
|4|Q| <ul><li>Paced</li><li>Fusion of paced and normal</li><li>Unclassifiable</li></ul> |

