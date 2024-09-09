---
title: Conception d'architecture
type: stream
url: ./model/design/secure-architecture/stream-a/
business_function: Conception
business_function_url: design
practice: Architecture de Sécurité
stream: A
description: Conception / Architecture de Sécurité
keywords: ["Business function", "Practice", "Conception", "Architecture de Sécurité"]
aliases:
    - /fr/model/D-SA-A-1
    - /fr/model/D-SA-A-2
    - /fr/model/D-SA-A-3
    - /fr/model/D-SA-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            L'ensemble des principes de base de la sécurité à la disposition des équipes produit
        activity: |
            Lors de la phase de conception, le personnel technique de l'équipe produit utilise une courte checklist des principes de sécurité. Généralement, les principes de sécurité incluent : la défense en profondeur, la sécurisation du plus faible maillon, l'utilisation de valeurs par défaut sécurisées, éviter une conception complexe des fonctionnalités de sécurité, la bascule en mode dégradé en cas d'échec, l'équilibre entre sécurité et ergonomie, l'exécution avec le moindre privilège, proscrire la sécurité par l'obscurité, etc.

            Pour les interfaces, l'équipe considère chaque principe dans le contexte global du système et identifie les fonctionnalités qui peuvent renforcer la sécurité de chacune de ces interfaces. Il faut limiter ces fonctionnalités à celles qui ne demandent qu'un petit effort supplémentaire au-delà du coût de mise en œuvre normal des exigences fonctionnelles. Notez les fonctionnalités plus coûteuses et planifiez-les pour les versions futures.

            Dispensez à chaque équipe produit une formation de sensibilisation à la sécurité en amont de ce processus et intégrez plus de personnel averti en matière de sécurité pour aider aux prises de décision lors de la phase de conception.

        question: Les équipes utilisent-elles les principes de sécurité au cours de la conception ?
        quality_criteria:
            - Vous avez une liste de contrôle validée des principes de sécurité
            - Vous stockez votre liste de contrôle dans un endroit accessible
            - Les parties prenantes concernées comprennent les principes de sécurité

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Mutualiser des services de sécurité avec les équipes produit
        activity: |
            Identifiez l'infrastructure ou les services partagés présentant des fonctionnalités de sécurité. Ceux-ci incluent généralement des systèmes d'authentification unique, des services de contrôle d'accès ou d'autorisation, des services de journalisation et de surveillance ou un pare-feu applicatif. Enumérer et évaluer ces services partagés pour dresser une liste de ces ressources et les catégoriser selon la fonction de sécurité qu'elles remplissent. Envisagezr chaque ressource en fonction de son utilité et ses bénéfices pour l'équipe produit.

            S'il existe plusieurs ressources dans chaque catégorie, sélectionnez un ou plusieurs services partagés à standariser par catégorie. Étant donné que le développement futur des logiciels s'appuiera sur ces services, examinez-les soigneusement pour vous assurer de maitriser comment leur sécurité évoluera dans le temps. Pour chaque service sélectionné, créez des recommandation pour la conception afin que les équipes produit sachent comment les intégrer au système. Partager ces recommandations par le biais de la formation, du mentorat, des lignes directrices et des standards.

            Établissez les meilleures pratiques pour implémenter les fonctionnalités de sécurité. Rendez-les disponibles par des fonctions de recherche et/ou d'achat et pensez à les personnaliser pour les faire correspondre à la charte graphique de votre organisation pour une meilleure intégration. Des exemples de modèles incluent un sous-système d'authentification unique, un modèle de délégation à plusieurs niveaux, un modèle d'autorisation de séparation des tâches, un modèle de journalisation centralisé, etc.

            Ces modèles peuvent provenir de projets ou d'applications spécifiques, mais assurez-vous de les partager entre les différentes équipes de l'organisation pour une application efficace et cohérente des solutions de sécurité appropriées.

            Pour augmenter l'adoption de ces modèles, interfacez-les avec les services de sécurité partagés ou implémentez-les sous forme de composants qui peuvent être facilement intégrées dans une application. Soutenez les technologies clés au sein de l'organisation, par exemple dans le cas de différents environnements de développement. Gérez ces solutions comme de véritables applications avec un support approprié.

        question: Utilisez-vous des services de sécurité partagés au cours de la conception ?
        quality_criteria:
            - Vous avez une liste documentée de services de sécurité réutilisables, à la disposition des parties prenantes concernées
            - Vous avez vérifié la posture de sécurité de base pour chaque service sélectionné
            - Vos concepteurs sont formés à l'intégration de chaque service sélectionné selon les conseils disponibles

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Transparence totale de la qualité et de l'utilisabilité des solutions de sécurité tierces centralisées
        activity: |
            Construisez un ensemble d'architectures de référence qui sélectionne et combine un ensemble de composants de sécurité validés afin de garantir une conception appropriée de la sécurité. Les plateformes de référence ont l'avantage de raccourcir les audits et les revues de sécurité, d'améliorer l'efficacité lors du développement et de diminuer la charge de maintenance. Maintenez et améliorez continuellement l'architecture de référence en fonction des retours au sein de l'organisation et de la communauté. Faites participer les architectes, les développeurs seniors et tout autre intervenant technique à la conception et à la création des plateformes de référence. Après la phase de création, les équipes doivent continuer à fournir du support et des mises à jour.

            Les architectures de référence peuvent se matérialiser sous la forme d'un ensemble de librairies logicielles et d'outils avec lesquels les équipes projet construisent les logiciels. Ils sont le point de départ pour la standardisation d'une approche par la configuration sécurisée et la sécurité par défaut. Il est possible d'amorcer la construction de l'environnement en sélectionnant un projet donné tôt dans le cycle de vie et d'impliquer une équipe compétente en sécurité en renfort pour construire la fonctionnalité de sécurité de façon générique pour qu'il soit possible de l'extraire ultérieurement du projet et de l'utiliser ailleurs dans l'organisation. 

            Suivez continuellement les faiblesses ou les écarts dans l'ensemble de solutions de sécurité disponibles au sein de l'organisation lors des discussions concernant l'architecture, le développement ou l'exploitation. Ceci constitue un entrant pour l'amélioration de la pertinence et de l'efficacité des architectures de référence en place.

        question: Basez-vous votre conception sur des architectures de référence disponibles?
        quality_criteria:
            - Vous avez une ou plusieurs architectures de référence approuvées et documentées et qui sont à la disposition des parties prenantes
            - Vous améliorez continuellement les architectures de référence en fonction des connaissances et des bonnes pratiques
            - Vous fournissez un ensemble de composants, bibliothèques et outils pour implémenter chaque architecture de référence

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
