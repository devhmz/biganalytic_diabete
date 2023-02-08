# biganalytic_diabete
On recherche l’hypothèse qu’un patient soit diabétique sur la base de certaines caractéristique (Grosses, glucose, tension, insuline, épaisseur de la peau, indice de la masse corporelle, âge et la fonction pedigree du diabète) 

# Objectif :


On recherche l’hypothèse qu’un patient soit diabétique sur la base de certaines caractéristique
(Grosses, glucose, tension, insuline, épaisseur de la peau, indice de la masse corporelle, âge et la
fonction pedigree du diabète)
Cet ensemble de données pourrait être utilisé pour former un modèle d'apprentissage automatique
capable de prédire la probabilité qu'un patient soit diabétique sur la base de ces caractéristiques. Le
modèle apprendra à partir des données fournies et utilisera cet apprentissage pour faire des
prédictions sur de nouvelles données non vues.


# Qu'est-ce que le diabète ?


Selon le NIH, "le diabète est une maladie qui survient lorsque votre glycémie, également appelée
sucre dans le sang, est trop élevée. Le glucose sanguin est votre principale source d'énergie et
provient des aliments que vous mangez. L'insuline, une hormone fabriquée par le pancréas, aide le
glucose contenu dans les aliments à pénétrer dans les cellules pour être utilisé comme source
d'énergie. Il arrive que l'organisme ne produise pas assez d'insuline - ou n'en produise pas du tout -
ou qu'il ne l'utilise pas bien. Le glucose reste alors dans votre sang et n'atteint pas vos cellules.
Avec le temps, un excès de glucose dans le sang peut entraîner des problèmes de santé. Bien
que le diabète soit incurable, vous pouvez prendre des mesures pour gérer votre diabète et rester en
bonne santé.
On appelle parfois le diabète "une touche de sucre" ou "diabète limite". Ces termes
suggèrent qu'une personne n'a pas vraiment de diabète ou que son cas est moins grave, mais chaque
cas de diabète est grave.

# Quels sont les différents types de diabète ? 

Les types de diabète les plus courants sont le
type 1, le type 2 et le diabète gestationnel.
Diabète de type 1 Si vous êtes atteint de diabète de type 1, votre organisme ne produit pas
d'insuline. Votre système immunitaire attaque et détruit les cellules de votre pancréas qui fabriquent
l'insuline. Le diabète de type 1 est généralement diagnostiqué chez les enfants et les jeunes adultes,
bien qu'il puisse apparaître à tout âge. Les personnes atteintes de diabète de type 1 doivent prendre
de l'insuline tous les jours pour rester en vie.
Diabète de type 2 Si vous êtes atteint de diabète de type 2, votre organisme ne fabrique pas
ou n'utilise pas bien l'insuline. Vous pouvez développer un diabète de type 2 à tout âge, même
pendant l'enfance. Toutefois, ce type de diabète survient le plus souvent chez les personnes d'âge
moyen et les personnes âgées. Le type 2 est le type de diabète le plus courant.
Le diabète gestationnel Le diabète gestationnel se développe chez certaines femmes
lorsqu'elles sont enceintes. La plupart du temps, ce type de diabète disparaît après la naissance du
bébé. Cependant, si vous avez eu un diabète gestationnel, vous avez plus de chances de développer
un diabète de type 2 plus tard dans votre vie. Parfois, le diabète diagnostiqué pendant la grossesse
est en fait un diabète de type 2.
Autres types de diabète Parmi les types moins courants, on trouve le diabète monogénique,
qui est une forme héréditaire de diabète, et le diabète lié à la mucoviscidose ."


#  Présentation des données :


L'ensemble de données contient des informations sur les patients telles que leurs :
Grossesses : nombre de fois où la patiente a été enceinte.
Glucose : concentration de glucose dans le plasma lors d'un test de tolérance au glucose oral.
Blood Pressure : pression sanguine diastolique (mm Hg).
Epaisseur de la peau : épaisseur du pli cutané du triceps (mm).
Insuline : insuline sérique à 2 heures (mu U/ml).
BMI : indice de masse corporelle (poids en kg/(taille en m)^2).
Diabetes Pedigree Function : fonction de pedigree du diabète.
Age : âge en années.
Résultat : 0 pour l'absence de diabète, 1 pour le diabète.

# Analyse ACP :


Dans le cas de cet ensemble de données, l'ACP a probablement été utilisée pour identifier les
caractéristiques les plus pertinentes pour prédire la probabilité de diabète chez un patient. Les
résultats de l'ACP peuvent être utilisés pour sélectionner un sous-ensemble de caractéristiques
les plus importantes pour la construction d'un modèle de prédiction de diabète. Il peut
également être utilisé pour visualiser les relations entre les variables et identifier des clusters
de patients similaires en termes de risque de diabète.


# Ecart type :

Dans le contexte de cette étude, l'écart type peut être utilisé pour évaluer la variabilité des
caractéristiques de patients diabétiques, comme leur âge, leur indice de masse corporelle, leur
pression artérielle, etc. Il peut également être utilisé pour évaluer la variabilité des résultats de
tests de laboratoire, tels que la glycémie ou l'insuline. En comparant l'écart type de différentes
caractéristiques ou résultats de test, on peut déterminer lesquels sont les plus variables et donc
les plus importants pour la prédiction du diabète

array([ 3.595 , 38.3846, 22.8394, 16.6625, 245.2066, 9.7377,
0.5865, 12.921 ])

Dans ce cas, l'écart type des données montre que la variable "insuline" a une plus grande
variabilité par rapport aux autres variables. Cela signifie que les valeurs de l'insuline varient
considérablement par rapport à la moyenne. Les autres variables ont des écarts types plus
faibles, ce qui signifie qu'elles ont moins de variation par rapport à la moyenne. Cela peut
aider à identifier les variables qui auront un impact plus important sur les résultats.

# L’obésité et le diabète :

L'obésité, évaluée par l'indice de masse corporelle (IMC), est intimement associée au diabète
et son impact sur le développement du DT2 a été largement décrit dans de grandes études
prospectives de cohorte (VAN GAAL et SCHEEN, 2015 ; WILDING, 2014 ; RUIZ-ALEJOS
et al, 2020). En effet, la plupart des individus atteints de DT2 sont en surpoids ou obèses 5.
Malgré le lien entre l'obésité et le DT2, tous les obèses ne développent pas le diabète et tous
les diabétiques ne sont pas des personnes obèses. Les personnes diabétiques maigres ont
probablement une composante génétique plus forte pour le DT2 que les personnes en surpoids
et obèses (WILDING, 2014). Selon Ruiz-Alejos et col (2020) "il n'y a pas de recommandation
spécifique sur l'utilisation d'une mesure anthropométrique comme marqueur pour la prédiction
du risque de DT2 en dehors de l'IMC et du tour de taille". Malheureusement, le tour de taille
est une mesure qui ne figure pas dans l'ensemble de données sur le diabète des Indiens Pima.
L'IMC est une méthode simple mais précise pour indiquer l'état nutritionnel des adultes
(comme on peut le voir dans le tableau ci-dessous). Il peut être calculé en divisant le poids de
l'individu (en kg) par le carré de sa taille (en mètres).

Figure 1

• 11 femmes n'ont pas d'information sur leur IMC. Seules 106 des 758 femmes ont un
poids normal. La plupart des femmes présentent un surpoids ou une obésité.

Figure 2

Figure 3

Les femmes diabétiques ont tendance à présenter des valeurs plus importantes pour l'âge,
l'IMC, l'insuline, l'épaisseur de la peau, la pression artérielle et les grossesses.
La caractéristique qui permet de voir 2 groupes distincts (diabétique et non diabétique) est le
glucose.


# Matrice de correlation :


A partir de cette matrice, nous pouvons constater qu'il existe plusieurs corrélations fortes entre
les variables. Par exemple, il existe une forte corrélation négative entre les grossesses et
l'épaisseur de la peau (-0,74), et une forte corrélation positive entre le glucose et l'insuline
(0,56). En outre, il existe une corrélation positive modérée entre le glucose et l'âge (0,64) et
entre la fonction du pedigree du diabète et l'âge (0,15).
La variable cible "diabète" est corrélée avec la plupart des variables indépendantes, en
particulier le glucose, l'IMC et l'âge. Le coefficient de corrélation entre le diabète et le glucose
est de 0,17.
Il est également important de noter que certaines variables ont une faible corrélation avec la
variable cible, comme les grossesses (-0,06) et la pression artérielle (-0,12).
‘’Diabète de grossesse’’ : plus t’es âgée plus t’as peut-être plus de grossesses, donc plus de
de diabète de grossesse donc risque d’être diabétique.
La variable "glucose" a une forte corrélation positive avec les variables "BloodPressure"
(0.12), "Insulin" (0.56) et "age" (0.64). Elle a une faible corrélation positive avec la variable
"pregnancies" (0.17) et une faible corrélation négative avec la variable "SkinThickness" (-
0.16).
En 2005, Les résultats d’une étude chez 2045 sujets révèlent que la prévalence de diabète
augmente significativement selon les grades d’hypertension artérielle (optimale, normale,
normale-élevée et franchement élevée) évalués au moyen de la tension artérielle de clinique.

Matrice de corrélation 1

https://sqha2.hypertension.qc.ca/lhypertension-arterielle-un-puissant-predicteur-dintolerance-
au-glucose-de-diabete-et-dhypercholesterolemie/

La variable "BloodPressure" a une faible corrélation positive avec les variables "pregnancies"
(0.01), "glucose" (0.12) et "age" (0.36). Elle a une faible corrélation négative avec les
variables "SkinThickness" (-0.16), "Insulin" (-0.07) et "BMI" (-0.46).
Une analyse multivariée tenant en compte le sexe, l’IMC, l’âge et le traitement
antihypertenseur a permis de mettre en évidence une corrélation positive entre les niveaux de
glycémie et de cholestérol total avec toutes les valeurs de tension artérielle
Les résultats de cette étude suggèrent donc que l’hypertension artérielle pourrait être le facteur
causal à la base d’une foule de perturbations métaboliques dont notamment l’intolérance au
glucose, le diabète et l’hypercholestérolémie.
La variable "SkinThickness" a une forte corrélation négative avec les variables "pregnancies"
(-0.74), "glucose" (-0.16), "Insulin" (0.48) et "BMI" (0.29). Elle a une faible corrélation
positive avec les variables "DiabetesPedigreeFuncion" (0.14) et "age" (0.12).
La variable "Insulin" a une forte corrélation négative avec les variables "pregnancies" (-0.51),
"SkinThickness" (-0.07) et "BMI" (-0.05). Elle a une forte corrélation positive avec les
variables "glucose" (0.56) et "age" (0.50).
C’est pour ça aujourd’hui on fait des test de hyperglycémie provoquée par voix orale qui sert
à confirmer le diagnostique de diabète
https://www.chumontreal.qc.ca/sites/default/files/2018-06/88-2-test-hyperglycemie-
provoquee.pdf
En analysant la matrice de corrélation, nous pouvons voir que certaines caractéristiques ont
une forte corrélation avec la probabilité d'être atteint de diabète, telles que la glycémie
(Glucose), l'IMC (BMI), l'âge, le diabète antérieur (DiabetesPedigreeFunction) et le nombre
de grossesses. D'autres caractéristiques comme la pression artérielle et l'épaisseur de la peau
ont une faible corrélation avec la probabilité de diabète. Il est important de noter que cette
matrice de corrélation montre seulement les relations linéaires entre les variables, il peut y
avoir d'autres relations non linéaires qui ne sont pas capturées par cette analyse

#  Résultat de l’inertie :

[34.23 30.38 19.16 12.83 7.44 4.52 3.03 0.42]
Si on remarque la quantité de données observées, on peut se baser sur 6
composantes qui peuvent couvrir le besoin de cette analyse.
On observe qu’on peut réduire le nombre de composantes à 6 car à partir de
la 6 ème composante on a un résultat de plus de 95 % ça peut nous permettre
de conclure sur un résultat si on fait encore une analyse plus approfondie
sur les composantes choisies.
A noté que dans notre cas la quantité compte mais aussi la qualité de données analysées est
bien plus importante.En terme de qualité on peut réduire à 5 car on juge que c’est suffisant
pour avancer l’analyse, sinon pour une quantité de données qui couvrent un peut plus que 95
% on peut réduire à 6 composantes.

# Cercle de corrélation :

Diagramme d'inertie 1
Sur le premier cercle de corrélation on peut constituer déjà un premier cluster (Insumin,
pregnancies et glycémie) qu’on peut définir comme du diabète du type 1 :
Dans le diabète de type 1, le pancréas ne fabrique plus d’insuline de façon suffisante. En son
absence, les cellules ne peuvent plus utiliser correctement le sucre qui circule dans le sang.
L’hyperglycémie apparaît rapidement, dès que le niveau d’insuline devient insuffisant
Sur le deuxième cercle de corrélation on peut constituer un deuxième cluster qui peut correspondre à un diabète de type 2 :

Cercle de corrélation 1

Cercle de corrélation 2

le diabète dit « de type 2 », dû à une mauvaise utilisation de l’insuline par les cellules de
l’organisme. Son développement se fait très progressivement, de façon insidieuse sur de
nombreuses années.

Cercle de corrélation 3

On peut former un troisième cluster (Pregnancies, glucose, Age) qui peut correspondre à un
diabète de grossesse car on a une forte correlation entre les pregnancies, glycose et diabète

# Relation entre les caractéristiques :

Corrélatoin en les caractéristique 1

Figure 4

Arbre de décision 1

Pour certaines méthodes d'ajustement, il existe des paramètres d'ajustement
intégrés au modèle qui compensent le nombre de prédicteurs ajoutés au modèle pendant
l'ajustement. Ces compensations empêchent le modèle de trop s'adapter aux données de
l'ensemble d'apprentissage et, d'une certaine manière, optimisent le compromis biais-
variance. Ces paramètres peuvent être ajustés en utilisant la validation croisée pour
permettre au modèle de mieux s'adapter à l'ensemble des données. Ainsi, il y a beaucoup
plus de travail à faire que de simplement faire passer les données par toutes les
méthodes d'apprentissage statistique par défaut.

# La matrice du nuage :

La matrice du nuage de points est utile
pour identifier les relations par paire
des caractéristiques de manière
préliminaire. Si les points sont
dispersés, cela signifie qu'il n'y a pas de
relation évidente, tandis que si les
points sont grossièrement disposés en
ligne droite, cela signifie qu'ils sont
linéairement liés. Si l'on se réfère à la
matrice du nuage de points de la figure
4, les caractéristiques les plus
étroitement corrélées/proportionnelles
sont [la grossesse et l'âge], [l'épaisseur
de la peau et l'IMC] et [le glucose et
l'insuline], car leurs diagrammes de
dispersion montrent tous une
corrélation positive.

Figure 6

Afin de rendre notre modèle clair et explicable, cette partie montre aux utilisateurs finaux
comment nous jugeons les caractéristiques importantes. Pour la sélection des caractéristiques
dans le cadre des expériences avec les modèles d'apprentissage automatique, cette recherche
effectue un clustering k-means, une analyse en composantes principales (ACP) et un
classement par importance sur l'ensemble de données.

Figure 5
Figure 7 1

En commençant par l'ACP, les groupements de caractéristiques ont été observés dans le
graphique de la figure 6, où les flèches qui sont proches les unes des autres représentent des
caractéristiques étroitement liées. On peut voir que les caractéristiques suivantes sont
étroitement liées :
• Grossesse et âge
• Glucose et pression artérielle (PA)
• IMC, DPF, taux d'insuline et épaisseur de la peau.
Ensuite, le clustering k-means a été utilisé avec différentes valeurs de k et observé. D'après la
figure 5, nous pouvons voir que k = 2 permet la meilleure séparation des frontières ou des
groupes, mais k = 3 permet également un regroupement décent et pourrait être utile.
l semble y avoir une différence démontrable dans la performance et l'efficacité des modèles de
classification de prédiction en fonction de la méthodologie de prétraitement. Par conséquent,
lors de la première série d'expériences, un prétraitement minimal a été effectué. La deuxième
fois, cependant, des algorithmes de sélection des caractéristiques ont été appliqués.
Comme il n'y avait pas de valeurs manquantes ou nulles, une seule technique de prétraitement
des données a été appliquée lors du premier tour. Il s'agissait d'imputer la valeur médiane sur
les caractéristiques qui avaient des valeurs nulles invalides.
Les algorithmes d'arbres tels que les arbres de décision, les modèles Naïve Bayes et les forêts
aléatoires ne sont pas très sensibles aux données non normalisées, de sorte qu'aucune mise à
l'échelle n'a été effectuée afin de maintenir les tests similaires pour les trois modèles
d'apprentissage automatique.
Avec seulement huit caractéristiques, il peut sembler contre-intuitif de réduire davantage les
caractéristiques, mais cela peut réduire une partie du bruit dans la classification et mettre en
évidence des groupements subtils synthétisés en combinant des classes existantes. Lors des
deuxièmes et troisièmes séries d'expériences, les méthodologies de sélection des
caractéristiques utilisées étaient les suivantes : PCA, le clustering k-means et le classement
par importance

" Conclusion :

. Pour résumer, cette étude montre que la prédiction de la probabilité de diabète peut être
améliorée en utilisant des caractéristiques telles que la glycémie, l'IMC, l'âge, le diabète
antérieur et le nombre de grossesses. Il est important de continuer à étudier ces relations pour
mieux comprendre la maladie et pour améliorer les méthodes de prévention et de traitement
du diabète
La glycémie, l'IMC, l'âge, le diabète antérieur et le nombre de grossesses sont tous des facteurs de
risque pour le diabète de type 2. La glycémie élevée est un indicateur de diabète, car elle peut
indiquer une résistance à l'insuline ou une insuffisance pancréatique. L'IMC élevé est également un
facteur de risque, car il est associé à une augmentation de la graisse corporelle, qui peut entraîner
une résistance à l'insuline. Les personnes âgées ont également un risque accru de développer un
diabète, car leur capacité à produire de l'insuline peut diminuer avec l'âge. Les antécédents familiaux
de diabète et le nombre de grossesses sont également des facteurs de risque importants. Plusieurs
de ces facteurs peuvent être utilisés pour évaluer le risque de développer un diabète de type 2 et
pour décider si des mesures préventives doivent être prises.
Le glucose est le facteur le plus important pour déterminer l'apparition du diabète, suivi par l'IMC et
l'âge. D'autres facteurs tels que la fonction Pedigree du diabète, les grossesses, la pression artérielle,
l'épaisseur de la peau et l'insuline contribuent également à la prédiction.
Comme nous pouvons le constater, les résultats dérivés de Feature Importance sont logiques car l'un
des premiers éléments contrôlés chez les patients à haut risque est le taux de glucose. Un IMC élevé
peut également indiquer un risque de développer un diabète de type II. Normalement, surtout dans
le cas du diabète de type II, le risque est élevé lorsque l'âge de la personne augmente (compte tenu
d'autres facteurs).
Le diabète de grossesse, également appelé diabète gestationnel, est un type de diabète qui se
développe uniquement pendant la grossesse. Il se produit lorsque la femme enceinte ne produit pas
suffisamment d'insuline pour compenser l'augmentation de la demande en insuline pendant la
grossesse. Cela peut entraîner une augmentation des niveaux de sucre dans le sang et un risque
accru de complications pour la mère et l'enfant. Les facteurs de risque pour le diabète gestationnel
comprennent l'âge maternel avancé, l'obésité, les antécédents familiaux de diabète, les grossesses
antérieures avec des complications liées au diabète et certaines populations ethniques. Le diabète
gestationnel peut généralement être géré avec un régime alimentaire sain, des activités physiques
et, si nécessaire, des médicaments pour réguler les niveaux de sucre dans le sang. Il est important de
surveiller les niveaux de sucre dans le sang pendant la grossesse pour minimiser les risques pour 
