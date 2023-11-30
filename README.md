# Exam-design-Patterns-Julien-BERTRAND

# Question 1
Expliquez, de manière générale l'utilité des pattern de conception, quels mécanismes font-ils souvent intervenir ?

## Réponse 1 
Les pattern de conception permettent de répondre à un problème connu et fréquent. Ils constituent un ensemble d'objets décrits par des classes et des relations liant les objets. Pour cela, ils font intervenir certains mécanismes comme par exemple : la création d'objet, l'instanciation des classes concrète, la création d'interface permettant l'abstraction.

# Question 2
Analysez le code du fichier sample.cs dans le dossier 01, quel type de pattern est utilisé ici ? Décrivez son fonctionnement

## Réponse 2
Le code donné du fichier sample.cs dans le dossier 01 utilise le pattern de conception "Builder". Le pattern Builder est utilisé pour construire un objet complexe (dans notre cas, une voiture). Voici comment il fonctionne sur le code fournit : En premier lieu, le client crée une nouvelle instance de SedanCarBuilder. Ensuite, il va créer une nouvelle instance de CarManufacturer (manufacturer) en passant en paramètre la nouvelle instance de SedanCarBuilder (builder). Puis, le client va utiliser la méthode ConstructCar de manufacturer. Cette méthode va permettre de lancer le processus de construction de la voiture. Une fois que la construction de la voiture est terminée, le client récupère la voiture à l'aide de la méthode GetCar du CarBuilder. Enfin, la méthode Display de car va permettre au client de l'afficher.

# Question 3
Analysez le code du fichier sample.cs dans le dossier 02. Quel le principal inconvénient du code présenté  ?Quel type de pattern pourrait être utilisé ici ? Décrivez son fonctionnement.

## Réponse 3
Le principal inconvénient du code est qu'il crée une multitude d'instances de la classe "PoorlyDesignedClass".  Afin de résoudre le problème, nous pourrions utiliser le design pattern "Singleton". Le design pattern Singleton permet de garantir qu'une seul instance de la classe (dans notre cas "PoorlyDesignedClass") soit créée et partagée dans toute l'application.

# Question 4
Analysez le code du fichier sample.cs dans le dossier 03. Décrivez le code suivant, quel pattern le développeur a-t-il tenté d'utiliser ? Selon vous, Le code est-il correct ? Si non, quelles modifications pourraient-on apporter à ce programme ?

## Réponse 4
Le développeur a tenté d'utiliser le design pattern "Chain of Responsibility" pour gérer les différents processus de données. Pour moi, le code est correct et fonctionnel. Cependant, j'apporterai quelques modifications comme par exemple : je modifierai la classe "PoorlyDesignedCode" car elle effectue des vérifications presque identiques aux classes "IntDataHandler", "StringDataHandler" et "DoubleDataHandler".

# Question 5
Analysez le code du fichier sample.cs dans le dossier 04. Décrivez le code suivant, quel pattern le développeur a-t-il tenté d'utiliser ? Selon vous, Le code est-il correct ? Si non, quelles modifications pourraient-on apporter à ce programme ?

## Réponse question 5
Le développeur a tenté d'utiliser le design pattern "Decorator" pour ajouter une modification dynamique du comportement des objets. Le code répond bien à l'intention du design pattern "Decorator". Les classes sont correctement structurées. La class "Program" (client) illustre bien comment créer des formes, les regrouper et ajouter des fonctionnalités spécifiques comme avec l'exemple de "RedShapeD".
