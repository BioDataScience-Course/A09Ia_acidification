# Croissance d'un foraminifère en présence d’acidification et d’augmentation de la température

Doo et al. (2020) ont étudié les effets d'une acidification et d'une augmentation de la température sur le foraminifère vertèbre *Marginopora vertebralis* Quoy & Gaimard 1830. Ils ont également étudié en parallèle ces effets lorsque *M. vertebralis* est en présence de l'un de ses hôtes, l'algue rouge *Laurencia intricata* J.V.Lamouroux 1813.

Les auteurs ont publié les données de cette étude (Doo et al. 2021). L'article correspondant est disponible dans le sous-dossier `bibliography`. Vous utiliserez une partie de ces données pour appliquer l'analyse de variance à un facteur et le test de Kruskal-Wallis. Les données
originales se trouvent dans le dossier `data/raw`, mais vous utiliserez les données remaniées `growth.rds` qui se trouvent dans le dossier `data`. Ce projet correspond au template <https://github.com/BioDataScience-Course/A09Ia_acidification>.

## Objectifs

Ce projet est individuel et cadré. Il permet de démontrer que vous avez acquis les compétences suivantes :

- représenter graphiquement de la manière la plus appropriée les données à étudier avec une ANOVA
- formuler les hypothèses de l'ANOVA à un facteur
- réaliser une ANOVA à un facteur et l'interpréter sur des données biologiques

## Consignes

Complétez le document `vertebralis_notebook.qmd`. Le jeu de données à disposition `data/growth.rds` contient les variables suivantes (les conditions exactes utilisées sont précisées dans la Table 1 de Doo et al. 2020) :

- **Name :** un identifiant unique de chaque individu étudié,
- **pH :** une variable facteur indiquant le traitement effectué relatif au pH, soit `"amb"` pour ambiant (= non modifié) ou `"low"` pour des conditions simulées d'acidification de l'eau (pH bas par rapport au pH habituel de l'eau de mer),
- **Temp :** une variable facteur indiquant le traitement effectué relatif à la température, soit `"amb"` pour ambiant (= non modifié) et `"high"` pour des conditions simulées d'augmentation de la température,
- **Association :** une variable facteur indiquant si l'individu a été associé à l'algue rouge *Laurencia intricata* (`"Yes"`) ou non (`"No"`),
- **Wet_Weight :** le pourcentage de variation journalière de la masse observé durant l'expérience,
- **Condition :** une variable facteur à quatre niveaux reprenant à la fois le traitement pH et le traitement température, avec `"n"` conditions normales (référence), `"p"` pH bas uniquement, `"t"` température élevée uniquement et `"tp"` à la fois pH bas et température élevée.

N'oubliez pas d'effectuer un “Rendu” du document en HTML à la fin de votre travail pour vérifier que tout fonctionne bien, et corrigez les erreurs éventuelles rencontrées à ce stade (très important ! Sans quoi il ne sera pas possible de donner des points à votre travail) Vous avez une batterie de tests à votre disposition pour des vérifications plus poussées de vos résultats (onglet "Construire" -> bouton "Construire tout"). Vérifiez également que votre
dernier commit a bien été pushé sur GitHub avant la deadline.

# Références

Doo, Steve S., Aero Leplastrier, Alexia Graba-Landry, Januar Harianto, Ross A. Coleman, et Maria Byrne. 2020. « Amelioration of ocean acidification and warming effects through physiological buffering of a macroalgae ». *Ecology and Evolution* 10 (15): 8465‑75. <https://doi.org/10.1002/ece3.6552>.

Doo, Steve S., Aero Leplastrier, Alexia Graba-Landry, Januar Harianto, Ross Coleman, et Maria Byrne. 2021. « Data from: Amelioration of ocean acidification and warming effects through physiological buffering of a macroalgae ». Dryad. <https://doi.org/10.5061/dryad.qv9s4mwbw>.
