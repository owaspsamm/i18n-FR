---
title: Base de référence à l'échelle
type: stream
url: ./model/verification/security-testing/stream-a/
business_function: Vérification
business_function_url: verification
practice: Tests de sécurité
stream: A
description: Vérification / Tests de sécurité
keywords: ["Business function", "Practice", "Vérification", "Tests de sécurité"]
aliases:
    - /fr/model/V-ST-A-1
    - /fr/model/V-ST-A-2
    - /fr/model/V-ST-A-3
    - /fr/model/V-ST-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Détection de vulnérabilités communes faciles à trouver
        activity: |
            Utilisez des outils de test de sécurité statique et dynamique automatisés pour les logiciels, ce qui permet des tests de sécurité plus efficaces et des résultats de meilleure qualité. Augmentez progressivement la fréquence des tests de sécurité et augmentez la couverture du code.

            Les tests de sécurité des applications peuvent être effectués statiquement, en inspectant le code source d'une application sans l'exécuter, ou dynamiquement en observant simplement le comportement de l'application en réponse à diverses conditions d'entrée. La première approche est souvent appelée « Static Application Security Testing » (SAST), la seconde étant appelée « Dynamic Application Security Testing » (DAST). Une approche hybride, connue sous le nom de Tests de Sécurité Intéractifs d'Applications (IAST), combine les forces des deux approches (au prix d'efforts supplémentaires) en testant dynamiquement des applications automatiquement instrumentées, permettant un suivi précis de l'état interne de l'application en réponse à une entrée externe.

            Beaucoup de vulnérabilités de sécurité sont très difficiles à détecter sans inspecter soigneusement le code source. Bien que cette tâche soit idéalement effectuée par des experts ou par des pairs, il s'agit d'une tâche lente et coûteuse. Bien que "plus bruyant" et souvent moins précis que des examens menés par des experts, les outils automatisés SAST sont moins chers, bien plus rapides et plus cohérents que les humains. Un certain nombre d'outils commerciaux ou gratuits sont capables de détecter efficacement les bogues et vulnérabilités suffisamment importants dans de grandes bases de code.

            Les tests dynamiques ne nécessitent pas le code source de l'application, ce qui le rend idéal pour les cas où le code source n'est pas disponible. Il identifie également des cas concrets de vulnérabilités. En raison de son approche "boîte noire", sans instrumentation, il est plus susceptible de découvrir des bogues peu enfouis. Les outils de test dynamiques ont besoin d'une grande source de données de test, dont la génération manuelle est prohibitive. De nombreux outils existent qui génèrent les données de test appropriées automatiquement, conduisant à des tests de sécurité plus efficaces et à des résultats de meilleure qualité.

            Sélectionnez les outils appropriés en fonction de plusieurs facteurs, notamment la profondeur et la précision de l'inspection, la robustesse et la précision des cas de tests de sécurité, les possibilités d'intégration avec d'autres outils, l'utilisation qui en sera faite et le modèle de coûts, etc. Lorsque vous sélectionnez des outils, prenez en compte les commentaires du personnel technique compétent en matière de sécurité ainsi que ceux des développeurs et des gestionnaires de développement et examinez les résultats avec les parties prenantes.

        question: Analysez-vous les applications avec des outils de test de sécurité automatisés?
        quality_criteria:
            - Vous générez dynamiquement des entrées pour les tests de sécurité à l'aide d'outils automatisés
            - Vous choisissez des outils de test de sécurité adaptés à l'architecture de l'organisation et à la pile technologique, et trouvez un juste équilibre entre la profondeur et la précision de l'inspection d'une part et la facilité d'utilisation des résultats pour l'organisation d'autre part

        answers:
            - Non
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level2:
        level: 2
        benefit: |
            Détection des vulnérabilités faciles à trouver spécifiques à l'organisation
        activity: |
            Augmentez l'efficacité des outils de test de sécurité automatisés en les ajustant et les personnalisant à vos piles technologiques et applications. Les outils de test de sécurité automatisés ont deux caractéristiques importantes : leur taux de faux positifs, c.-à-d. les bogues inexistants et les vulnérabilités qu'ils signalent de façon erronée ; leur taux de faux négatifs, c'est-à-dire les bogues réels et les vulnérabilités qu'ils ne détectent pas. À mesure que vous améliorez votre maturité dans l'utilisation d’outils de test automatisés, vous vous efforcez de minimiser leurs taux de faux négatifs et de faux positifs. Cela maximise le temps que les équipes de développement passent à examiner et à traiter les vrais problèmes de sécurité dans leurs applications et réduit les frictions typiquement associées à l'utilisation d'outils d'analyse de sécurité automatisés non ajustés.

            Commencez par désactiver la prise en charge des outils pour les technologies et les environnements que vous n'utilisez pas et ciblez les versions spécifiques dans la mesure du possible. Cela augmentera la vitesse d'exécution et réduira le nombre de résultats erronés signalés. Faites confiance à des experts d’outils de sécurité ou à des équipes de sécurité partagées pour piloter les outils en coordination avec un groupe d’équipes de développement motivées sélectionnées. Cela permettra d'identifier les interprétations faussement positives à ignorer ou à supprimer des résultats des outils. Identifiez les problèmes de sécurité spécifiques et les contre-modèles et favorisez le meilleur outil pour les détecter.

            Tirez parti des fonctionnalités des outils disponibles pour prendre en compte les styles de codage spécifiques aux applications et à l'organisation ainsi que les normes techniques. De nombreux outils d'analyse automatique statique permettent aux utilisateurs d'écrire leurs propres règles ou de personnaliser les règles d'analyse par défaut aux interfaces logicielles spécifiques au projet en cours de test afin d'atteindre une meilleure précision et une profondeur de couverture améliorée. Par exemple, les entrées potentiellement dangereuses (autrement dit, polluées) peuvent être marquées comme sûres après leur passage à travers une méthode d'assainissement appropriée donnée.

            Stratégiquement, il est préférable de détecter de manière fiable un sous-ensemble limité de problèmes de sécurité via un outillage automatisé et d'étendre progressivement la couverture, plutôt que d'essayer de détecter immédiatement tous les problèmes connus. Une fois que les outils ont été suffisamment ajustés, ils peuvent être mis à la disposition de plus d'équipes de développement. Il est important de surveiller continuellement leur efficacité perçue au sein des équipes de développement. Dans des formes plus élaborées, des techniques d'apprentissage automatique peuvent être adoptées pour identifier et filtrer automatiquement les faux positifs probables à l'échelle.

        question: Personnalisez-vous les outils de sécurité automatisés à vos applications et vos piles technologiques?
        quality_criteria:
            - Vous réglez et sélectionnez les fonctionnalités de l'outil qui correspondent à votre application ou votre pile de technologies
            - Vous minimisez les faux positifs en réduisant au silence ou en filtrant automatiquement les avertissements non pertinents ou les trouvailles de faible probabilité
            - Vous minimisez les faux négatifs en tirant parti des extensions des outils ou des DSLs pour personnaliser les outils pour votre application ou vos normes organisationnelles

        answers:
            - Non
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level3:
        level: 3
        benefit: |
            Identification des vulnérabilités identifiables automatiquement lors des étapes le plus possible en amont
        activity: |
            Les projets au sein de l'organisation exécutent régulièrement des tests de sécurité automatisés et examinent les résultats durant le développement. Configurez les outils de test de sécurité pour qu'ils s'exécutent automatiquement dans le cadre du processus de génération et de déploiement afin de permettre à ce système de passer à l'échelle à peu de frais. Inspectez les problèmes au fur et à mesure qu'ils sont détectés.

            Effectuez des tests de sécurité dès les phases de gestion des exigences ou de conception peut être bénéfique. Bien que traditionnellement utilisé pour les cas de tests fonctionnels, ce type d’approche de développement piloté par les tests implique l’identification et l’exécution de cas pertinents de tests de sécurité au début du cycle de développement. Avec l'exécution automatique de cas de tests de sécurité, les projets entrent dans la phase d'implémentation avec un certain nombre de tests défaillants en raison des fonctionnalités inexistantes ; l'implémentation est terminée lorsque tous les tests sont exécutés avec succès. Ceci fournit un objectif clair aux développeurs tôt dans le cycle de développement tout en diminuant le risque de retarder une livraison en raison de problèmes de sécurité ou de devoir accepter certains risques pour respecter les échéances du projet.

            Rendez les résultats des tests de sécurité automatisés et manuels visibles via des tableaux de bord et présentez-les régulièrement à la direction et aux parties prenantes métier (par ex. avant chaque version) pour revue. S'il persiste des problèmes non résolus acceptés comme risques pour la livraison, les parties prenantes et les gestionnaires du développement travaillent ensemble pour établir un calendrier concret pour les traiter. Examinez et améliorez continuellement la qualité des tests de sécurité.

            Considérez et mettez en place des outils de corrélation de test de sécurité pour automatiser la mise en correspondance et la fusion des résultats de test provenant de scanners d'applications dynamiques, statiques et interactifs dans un tableau de bord central fournissant une entrée directe vers le système de gestion des défauts. Diffusez les connaissances liées aux tests de sécurité créés et aux résultats au sein de l'équipe de développement afin d'améliorer les connaissances et la sensibilisation à la sécurité au sein de l'organisation.

        question: Intégrez-vous des tests de sécurité automatisés dans le processus de génération et de déploiement ?
        quality_criteria:
            - Les parties prenantes du management et des affaires suivent et revoient les résultats des tests tout le long du cycle de développement
            - Vous fusionnez les résultats des tests dans un tableau de bord central et les transmettez à la gestion des défauts

        answers:
            - Non
            - Oui, certain(e)s
            - Oui, au moins la moitié
            - Oui, la plupart ou la totalité

---
