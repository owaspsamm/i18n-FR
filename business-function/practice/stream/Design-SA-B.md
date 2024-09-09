---
title: Gestion de la technologie
type: stream
url: ./model/design/secure-architecture/stream-b/
business_function: Conception
business_function_url: design
practice: Architecture de Sécurité
stream: B
description: Conception / Architecture de Sécurité
keywords: ["Business function", "Practice", "Conception", "Architecture de Sécurité"]
aliases:
    - /fr/model/D-SA-B-1
    - /fr/model/D-SA-B-2
    - /fr/model/D-SA-B-3
    - /fr/model/D-SA-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Visibilité sur less technologies introduisant un risque de sécurité
        activity: |
            C'est souvent le chemin avec le moindre effort qui est adopté pour le développement, le déploiement ou l'exploitation d'une solution logicielle. Les nouvelles technologies sont souvent adoptées si elles réduisent l'effort ou facilitent le passage à l'échelle. Ces nouvelles technologies pourraient néanmoins introduire de nouveaux risques pour l'organisation qu'il faudrait gérer.

            Identifiez les technologies, les frameworks et les outils les plus utilisés pour chaque application. Etudiez les environnements de développement et d'exploitation ainsi que les artefacts. Ensuite, évaluez leur sécurité et relevez les écarts importants pour les gérer.

        question: Évaluez-vous la qualité de sécurité des technologies importantes utilisées pour le développement ?
        quality_criteria:
            - Vous avez une liste des technologies les plus importantes utilisées dans ou pour chaque application
            - Vous identifiez et suivez les risques technologiques
            - Vous vous assurez que les risques de ces technologies sont conformes à la référence organisationnelle

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Des technologies avec un niveau de sécurité approprié à la disposition des équipes produit
        activity: |
            Identifiez les technologies, les environnements et les outils couramment utilisés dans les projets logiciels à travers l'organisation, en vous concentrant sur la capture des technologies de haut niveau.

            Créez une liste et partagez-la à travers l'organisation de développement en tant que technologies recommandées. Lors de leur sélection, considérez l'historique des incidents, la liste des évènements passés concernant la réponse aux vulnérabilités, la pertinence des fonctionnalités pour l'organisation, une trop grande complexité d'utilisation de la composante tierce et des connaissances suffisantes au sein de l'organisation.

            Cette liste est créée par les développeurs et architectes seniors, en prenant en compte les commentaires des gestionnaires et des auditeurs de sécurité. Partagez cette liste de composants recommandés avec l'organisation de développement. En fin de compte, l'objectif est de fournir des solutions de référence bien identifiées aux équipes projet. Effectuez un examen périodique de ces technologies à propos de la sécurité et de la pertinence.

        question: Avez-vous une liste de technologies recommandées pour l'organisation ?
        quality_criteria:
            - La liste est basée sur les technologies utilisées dans le portefeuille de logiciels
            - Les architectes de référence et les développeurs révisent et approuvent la liste
            - Vous partagez la liste à travers l'organisation
            - Vous révisez et mettez à jour la liste au moins une fois par an

        answers:
            - "No"
            - Oui, pour certains domaines technologiques
            - Oui, pour au moins la moitié des domaines technologiques
            - Oui, pour la plupart ou tous les domaines technologiques

    level3:
        level: 3
        benefit: |
            Surface d'attaque limitée en raison de l'utilisation de technologies éprouvées
        activity: |
            Pour tout développement propriétaire (interne ou acquis), imposez et surveillez l'utilisation de technologies standards. Selon votre organisation, mettez en œuvre ces restrictions soit dans les outils de génération ou de déploiement via une analyse automatisée des artefacts d'application (e.g., code source, fichiers de configuration ou artefacts de déploiement), soit par une révision périodique en se focalisant sur l'utilisation correcte de ces environnements.

            Vérifiez plusieurs facteurs avec les équipes projet. Identifiez l'utilisation de technologies non-recommandées pour déterminer s'il y a des écarts entre les recommandations et les besoins de l'organisation. Examinez les modèles de conception et les modules des plateformes de référence non-utilisés ou mal utilisés pour déterminer si des mises à jour sont nécessaires. De plus, implémentez des fonctionnalités dans les platesformes de référence au fur et à mesure que l'organisation évolue et que les équipes projet le demandent.

        question: Mettez-vous en application l'utilisation de technologies recommandées au sein de l'organisation?
        quality_criteria:
            - Vous surveillez régulièrement les applications quant à l'utilisation correcte des technologies recommandées
            - Vous résolvez les violations de la liste selon les politiques organisationnelles
            - Vous prenez des mesures si le nombre de violations dépasse les objectifs annuels

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
