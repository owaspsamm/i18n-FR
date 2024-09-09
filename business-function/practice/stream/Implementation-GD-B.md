---
title: Métriques et Commentaires
type: stream
url: ./model/implementation/defect-management/stream-b/
business_function: Implémentation
business_function_url: implementation
practice: Gestion des Défauts
stream: B
description: Implémentation / Gestion des Défauts
keywords: ["Business function", "Practice", "Implémentation", "Gestion des Défauts"]
aliases:
    - /fr/model/I-DM-B-1
    - /fr/model/I-DM-B-2
    - /fr/model/I-DM-B-3
    - /fr/model/I-DM-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Identification des victoires rapides obtenues à partir des informations disponibles concernant les défauts
        activity: |
            Une fois par période de temps définie (généralement au moins une fois par an), passez en revue vos défauts de sécurité à la fois résolus et encore ouverts dans chaque équipe et extrayez les métriques simples à partir des données disponibles. Ceux-ci peuvent inclure :

                        * le nombre total de défauts par rapport au nombre total d'activités de vérification. Cela peut vous donner une idée de si vous recherchez des défauts avec une intensité et une qualité adéquates,
            * Les composants logiciels dans lesquels résident ces défauts. Cela peut indiquer où l'attention pourrait être la plus nécessaire et où les défauts de sécurité pourraient apparaître à nouveau dans le futur,
            * Le type ou la catégorie du défaut, ce qui suggère les domaines où l'équipe de développement a besoin d'une formation plus approfondie,
            * La sévérité du défaut, ce qui peut aider l'équipe à comprendre l'exposition au risque du logiciel.

            Identifiez et menez à bien des activités sensées à victoire rapide que vous pouvez construire à partir des connaissances nouvellement acquises. Cela peut inclure des choses comme une session de partage de connaissances sur un type de vulnérabilité donné ou effectuer / automatiser une analyse de sécurité.

        question: Utilisez-vous des métriques élémentaires sur les défauts de sécurité enregistrés afin de mener à bien des activités d'amélioration rapides ?
        quality_criteria:
            - Vous avez analysé vos métriques enregistrées au moins une fois l'année dernière
            - Au moins des informations de base sur cette initiative sont enregistrées et disponibles
            - Vous avez identifié et réalisé au moins une activité d'amélioration rapide basée sur les données

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Amélioration de l'apprentissage à partir des défauts de sécurité dans votre organisation
        activity: |
            Définissez, collectez et calculez des métriques unifiées à travers l'ensemble de l'organisation. Elles peuvent inclure :

                        * la quantité totale d'activités de vérification et de défauts identifiés,
            * les types et la sévérité des défauts identifiés,
            * les temps de détection et de résolution des défauts,
            * les fenêtres d'exposition des défauts présents sur les systèmes en production,
            * le nombre de régressions / de vulnérabilités rouvertes,
            * la couverture des activités de vérification pour certains composants logiciels,
            * le montant de risque accepté,
            * le ratio d'incidents de sécurité causés par des défauts de sécurité inconnus ou non documentés.

            Générez un rapport régulier (par exemple, mensuel) pour un public approprié. Cela touche généralement un public tel que les gestionnaires et les officiers de sécurité et les ingénieurs. Utilisez les informations contenues dans le rapport comme une contribution à votre stratégie de sécurité, par exemple pour améliorer les formations ou les activités de vérification de la sécurité.

            Partagez les détails techniques les plus importants ou les plus intéressants sur les défauts de sécurité, y compris la stratégie de correction, avec d'autres équipes une fois que ces défauts ont été corrigés, par ex. dans le cadre d’une réunion régulière de partage des connaissances. Cela aidera à démultiplier l'effet d'apprentissage suite à des défauts vers l'ensemble de l'organisation et limitera leur apparition dans le futur.

        question: Améliorez-vous votre programme d'assurance sécurité au moyen de métriques standardisées?
        quality_criteria:
            - Vous documentez les métriques de classification et de catégorisation des défauts et les maintenez à jour
            - La direction reçoit régulièrement des informations sur les défauts et a agi dessus au cours de l'année écoulée
            - Vous partagez régulièrement des détails techniques sur les défauts de sécurité entre les équipes

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Une stratégie de sécurité optimisée basée sur les informations liées aux défauts
        activity: |
            Réexaminez régulièrement (au moins une fois par an) les métriques de gestion des défauts que vous collectez et comparez les efforts nécessaires pour les collecter et les suivre aux résultats escomptés. Prenez des décisions éclairées quant à la suppression des métriques qui ne fournissent pas la valeur attendue. Dans la mesure du possible, incluez et automatisez les activités de vérification pour la qualité des données collectées et garantissez une amélioration durable si des écarts sont détectés.

            Agrégez les données avec vos métriques de cyberveille et de gestion des incidents et utilisez les résultats comme apports pour d'autres initiatives à travers l'ensemble de l'organisation, tels que :

                        * La planification de formations à la sécurité pour divers typologies de personnels
            * L'amélioration des activités de vérification de la sécurité pour les développements internes et externes
            * La gestion de la chaîne d'approvisionnement, c.a.d. effectuer des audits de sécurité des organisations partenaires
            * La surveillance des attaques contre votre infrastructure et vos applications
            * L'investissement dans des infrastructures de sécurité ou des contrôles compensatoires
            * Le recrutement pour votre équipe de sécurité et le cadrage du budget lié à la sécurité

        question: Évaluez-vous régulièrement l'efficacité de vos métriques de sécurité afin qu'elles soient toujours pertinentes pour contribuer à piloter votre stratégie de sécurité?
        quality_criteria:
            - Vous avez analysé l'efficacité des métriques de sécurité au moins une fois l'année dernière
            - Partout où cela est possible, vous vérifiez automatiquement la justesse des données
            - Les métriques sont agrégées avec d'autres sources comme le renseignement sur les menaces ou la gestion des incidents
            - Vous avez tiré au moins une initiative stratégique des indicateurs au cours de l'année écoulée.

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
