---
title: Protection des Données
type: stream
url: ./model/operations/operational-management/stream-a/
business_function: Opérations
business_function_url: operations
practice: Gestion opérationnelle
stream: A
description: Opérations / Gestion opérationnelle
keywords: ["Business function", "Practice", "Opérations", "Gestion opérationnelle"]
aliases:
    - /fr/model/O-OM-A-1
    - /fr/model/O-OM-A-2
    - /fr/model/O-OM-A-3
    - /fr/model/O-OM-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Compréhension de la sensibilité des données traitées avec des mesures dérivées à impact rapide
        activity: |
            Comprenez les types et la sensibilité des données stockées et traitées par vos applications et garantissez la bonne compréhension du devenir des données traitées (par ex. sauvegardes, partage avec des partenaires externes). À ce niveau de maturité, les informations recueillies peuvent être saisies sous différentes formes et dans différents endroits ; aucun catalogue de données à l'échelle de l'organisation n'est supposé exister. Protégez et gérez toutes les données associées à une application donnée conformément aux exigences de protection applicables aux données stockées et traitées les plus sensibles.

            Mettez en place des contrôles de base pour empêcher la propagation de données sensibles non assainies depuis les environnements de production vers des environnements de plus bas niveau. En veillant à ce que les données de production non assainies ne soient jamais propagées vers des environnements de plus bas niveau (non-production), vous pouvez concentrer les politiques et les activités de protection des données sur la production.

        question: Protégez-vous et gérez-vous les informations stockées et traitées par chaque application selon les exigences de protection des données?
        quality_criteria:
            - Vous connaissez les éléments de données traités et stockés par chaque application
            - Vous connaissez le type et le niveau de sensibilité de chaque élément de données identifié
            - Vous avez des contrôles pour empêcher la propagation de données sensibles non assainies de l'environnement de production vers les environnements inférieurs

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Gestion standardisée des différentes classes de données sensibles
        activity: |
            À ce niveau de maturité, les activités de protection de données se concentrent sur votre façon de gérer les données en votre possession. Établissez des contrôles techniques et administratifs pour protéger la confidentialité des données sensibles ainsi que l'intégrité et la disponibilité de toutes les données en votre possession, de leur création / réception initiale jusqu'à la destruction des sauvegardes à la fin de leur période de rétention.

            Identifiez les données stockées, traitées et transmises par des applications et enregistrez les informations concernant leur type, leur niveau de sensibilité (classification) et leur(s) lieu(x) de stockage dans votre catalogue de données. Identifiez clairement les enregistrements ou les éléments de données soumis à une réglementation spécifique. Établir une source de référence concernant les données avec lesquelles vous travaillez permet une sélection plus fine de contrôles pour leur protection. La collecte de ces informations améliore l'exactitude, la pertinence et l'efficacité de vos réponses aux requêtes liées aux données (par ex. de la part des auditeurs, des équipes de réponse à incident ou des clients) et facilite les activités de modélisation des menaces et de conformité.

            Sur la base de votre politique de protection des données, établissez des processus et des procédures pour la protection et la conservation des données tout au long de leur cycle de vie, que ce soit au repos, en cours de traitement, ou en transit. Portez une attention particulière à la manipulation et à la protection des données sensibles en dehors du système de traitement actif, incluant, mais sans s'y limiter, le stockage, la rétention et la destruction des sauvegardes, et l'étiquetage, le chiffrement et la protection physique des supports de stockage hors ligne. Vos processus et procédures couvrent la mise en œuvre de tous les contrôles adoptés pour se conformer à la réglementation, aux restrictions contractuelles ou autres sur les lieux de stockage, l'accès de la part du personnel et autres facteurs.

        question: Maintenez-vous un catalogue de données incluant les types, les niveaux de sensibilité et les emplacements de traitement et de stockage ?
        quality_criteria:
            - Le catalogue de données est stocké dans un endroit accessible
            - Vous savez quels éléments de données sont soumis à une réglementation spécifique
            - Vous avez des contrôles pour protéger et préserver les données tout au long de leur durée de vie
            - Vous avez des exigences de rétention des données et vous détruisez les sauvegardes en temps voulu à la fin de la période de rétention

        answers:
            - "No"
            - Oui, pour certaines de nos données
            - Oui, pour au moins la moitié de nos données
            - Oui, pour la plupart ou toutes nos données

    level3:
        level: 3
        benefit: |
            Conformité par la technique de votre politique de protection des données
        activity: |
            Les activités à ce niveau de maturité sont axées sur l'automatisation de la protection des données, ce qui réduit votre dépendance à l'égard des efforts humains pour l'évaluation et la gestion de la conformité aux politiques. L’accent est mis sur les mécanismes de retours d'expérience et les examens proactifs, afin d’identifier et d’agir sur les possibilités d’amélioration des processus.

            Mettez en œuvre des contrôles techniques pour rendre le respect de votre politique de protection des données obligatoire et rendez opérationnel un suivi automatique pour détecter les infractions potentielles ou avérées. Vous pouvez utiliser une palette d'outils disponibles concernant la prévention des pertes de données, le contrôle d'accès et le suivi, ou la détection de comportements anormaux.

            Vérifiez régulièrement la conformité aux contrôles administratifs en vigueur et surveillez de près les performances et le fonctionnement opérationnel des mécanismes automatisés, y compris les sauvegardes et les suppressions d'enregistrements. Surveiller les outils permet de détecter et de signaler rapidement les pannes de l'automatisation, ce qui permet de prendre des mesures correctives efficacement.

            Révisez et mettez à jour régulièrement le catalogue de données afin de maintenir son exacte réflexion de votre jeu de données. Des examens et des mises à jour régulières des processus et des procédures maintiennent leur alignement sur vos politiques et vos priorités.

        question: Examinez-vous et mettez-vous à jour régulièrement le catalogue de données et vos politiques et procédures en matière de protection des données?
        quality_criteria:
            - Vous avez une surveillance automatisée pour détecter les violations potentielles ou réelles de la politique de protection des données
            - Vous avez des outils pour la prévention des pertes de données, le contrôle d'accès et la journalisation, ou la détection de comportements anormaux
            - Vous contrôlez périodiquement le bon fonctionnement des mécanismes automatisés, y compris les sauvegardes et les suppressions d'enregistrements

        answers:
            - "No"
            - Oui, nous le faisons à la demande
            - Oui, nous le faisons toutes les quelques années
            - Oui, nous le faisons au moins une fois par an

---
