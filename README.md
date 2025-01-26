Modèle de Simulation d'Évacuation en NetLogo

Ce modèle NetLogo simule l'évacuation d'une bibliothèque en cas d'incendie. Il met en scène des agents (personnes) qui doivent trouver leur chemin vers les sorties tout en évitant les obstacles et en gérant leur patience et leur impatience. Le modèle inclut également la propagation du feu et son impact sur les agents.

Objectif du Modèle

L'objectif de ce modèle est de simuler les comportements des individus lors d'une évacuation d'urgence, en tenant compte de facteurs tels que la patience, l'impatience, et la propagation du feu. Le modèle permet d'observer comment ces facteurs influencent le temps d'évacuation et le nombre de victimes.

Fonctionnement du Modèle

Agents et Environnement

- Agents (Turtles) : Les agents représentent les personnes dans la bibliothèque. Ils sont de deux types :

- Patients : Ces agents sont plus calmes et attendent patiemment que le chemin se libère avant de se déplacer.

- Impatients : Ces agents sont plus agressifs et essaient de se frayer un chemin même si le passage est bloqué.

- Environnement : La bibliothèque est représentée par une grille de patches. Les obstacles (tables, murs, etc.) sont dessinés en jaune, les sorties en rouge, et le feu en orange.

Règles de Comportement

- Déplacement : Les agents se déplacent vers la sortie la plus proche. S'ils rencontrent un obstacle, ils essaient de le contourner. Les agents impatients peuvent pousser d'autres agents pour avancer, tandis que les agents patients attendent que le chemin se libère.

- Propagation du Feu : Le feu se propage aléatoirement sur les patches adjacents. Les agents qui se trouvent à proximité du feu perdent de la vie et peuvent mourir si leur vie atteint zéro.

- Sortie : Lorsqu'un agent atteint une sortie (patch rouge), il est considéré comme évacué et disparaît de la simulation.

Variables Globales

- death-counter : Compte le nombre d'agents morts.

- free-counter : Compte le nombre d'agents ayant réussi à évacuer.

- walk-counter : Compte le nombre de pas effectués par les agents.

Comment Utiliser le Modèle

Interface :

- Setup : Initialise la simulation en plaçant les agents, les obstacles, et le feu.

- Go : Lance la simulation.

Sliders :

- impatients : Nombre d'agents impatients.

- patients : Nombre d'agents patients.

- turtle-patience : Niveau de patience des agents patients.

Monitors :

- death-counter : Affiche le nombre d'agents morts.

- free-counter : Affiche le nombre d'agents évacués.

- walk-counter : Affiche le nombre de pas effectués.

Exécution :

Cliquez sur Setup pour initialiser la simulation.

Cliquez sur Go pour démarrer la simulation.

Observez comment les agents se déplacent, comment le feu se propage, et comment les compteurs évoluent.

Observations à Faire
Impact de la Patience : Observez comment le niveau de patience des agents affecte le temps d'évacuation et le nombre de victimes.

- Propagation du Feu : Notez comment la propagation du feu influence la survie des agents.

- Comportement des Agents : Observez les différences de comportement entre les agents patients et impatients.

Extensions Possibles

- Ajouter plus de Sorties : Modifiez le modèle pour inclure plusieurs sorties et observez comment cela affecte l'évacuation.

- Varier la Taille de la Bibliothèque : Changez la taille de l'environnement pour voir comment cela influence les résultats.

- Ajouter des Objets à Ramasser : Introduisez des objets que les agents doivent ramasser avant de sortir, ce qui ajoute une couche de complexité à la simulation.

- Fonctionnalités NetLogo Utilisées
Patches : Utilisés pour représenter l'environnement (murs, obstacles, sorties, feu).

- Turtles : Représentent les agents (personnes) dans la simulation.

- Cones : Utilisés pour la détection des obstacles et des autres agents.

- Randomness : La propagation du feu et les mouvements des agents sont partiellement aléatoires.

Modèles Connexes

- Fire : Un modèle de propagation de feu dans NetLogo.

- Traffic Basic : Un modèle de circulation qui explore les comportements des agents dans un environnement contraint.

