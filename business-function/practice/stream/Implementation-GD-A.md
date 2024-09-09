---
title: Suivi des Défauts
type: stream
url: ./model/implementation/defect-management/stream-a/
business_function: Implémentation
business_function_url: implementation
practice: Gestion des Défauts
stream: A
description: Implémentation / Gestion des Défauts
keywords: ["Business function", "Practice", "Implémentation", "Gestion des Défauts"]
aliases:
    - /fr/model/I-DM-A-1
    - /fr/model/I-DM-A-2
    - /fr/model/I-DM-A-3
    - /fr/model/I-DM-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Transparence des défauts de sécurité connus impactant des applications particulières
        activity: |
            Introduisez une définition / une compréhension commune de ce qu'est un défaut de sécurité et définissez les méthodes les plus courantes pour les identifier. Celles-ci comprennent, mais ne se limitent pas à:

                        * Évaluation de la menace
            * Tests de pénétration
            * Résultats d'outils d'analyse statique et dynamique
            * Processus de divulgation responsable ou prime de bogue

            Promouvez une culture de la transparence et évitez de blâmer toute équipe pour l'introduction ou l'identification de défauts de sécurité. Enregistrez et suivez tous les défauts de sécurité dans un emplacement défini. Cet emplacement n'a pas nécessairement à être centralisé pour l'ensemble de l'organisation, cependant assurez-vous de pouvoir avoir une vue d'ensemble de tous les défauts qui affectent une application donnée à n'importe quel moment. Définissez et appliquez des règles d'accès pour les défauts de sécurité suivis afin d'atténuer le risque de fuite et d'abus de ces informations.

            Introduisez a minima une classification qualitative rudimentaire des défauts de sécurité afin que vous soyez en mesure de prioriser les efforts de correction d'une manière satisfaisante. Efforcez-vous de limiter la duplication des informations et la présence de faux positifs afin d’accroître la fiabilité du processus.

        question: Tracez-vous tous les défauts de sécurité connus dans des endroits accessibles ?
        quality_criteria:
            - Vous pouvez facilement avoir une vue d'ensemble de tous les défauts de sécurité impactant une application
            - Vous avez a minima un système de classification rudimentaire en place
            - Le processus inclut une stratégie pour gérer les faux positifs et les doublons
            - Le système de gestion des défauts couvre les défauts provenant de diverses sources et activités

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Classification cohérente des défauts de sécurité avec des attentes claires quant à leur manipulation
        activity: |
            Introduisez et appliquez une méthodologie d'évaluation bien définie pour vos défauts de sécurité d'une façon cohérente à travers toute l'organisation, en vous basant sur la probabilité et l'impact attendu du défaut exploité. Cela vous permettra d'identifier les applications qui nécessitent une attention accrue et des investissements. Dans le cas où vous ne stockeriez pas les informations sur les défauts de sécurité centralement, assurez-vous que vous êtes toujours en mesure de récupérer facilement les informations depuis toutes les sources et d'obtenir un aperçu des « points chauds » qui nécessitent votre attention.

            Introduisez des contrats de niveau de service (CNS) pour garantir une correction des défauts de sécurité à temps selon leur niveau de criticité et surveillez de manière centralisée et faire un retour régulier sur les violations des CNS. Définissez un processus pour les cas où il n'est pas faisable ou économiquement raisonnable de corriger un défaut dans le délai défini par les CNS. Cela devrait au moins garantir que toutes les parties prenantes concernées ont une bonne compréhension du risque impliqué. Si c'est applicable, mettez en place des contrôles compensatoires pour ces cas.

            Même si vous n'avez pas de CNS formels pour corriger des défauts de faible gravité, veillez à ce que les équipes responsables obtiennent toujours un aperçu régulier des problèmes qui affectent leurs applications et comprennent comment des problèmes particuliers s’affectent ou s’amplifient les uns les autres.

        question: Gardez-vous une vue d'ensemble de l'état des défauts de sécurité au sein de l'organisation?
        quality_criteria:
            - Un système de sévérité unique est appliqué à tous les défauts à travers l'organisation
            - Le schéma inclut les SLAs pour la correction de classes de sévérité particulières
            - Vous partagez régulièrement des données sur la conformité aux SLA

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Garantie que les défauts de sécurité sont gérés selon des SLA prédéfinis
        activity: |
            Implémentez une alerte automatique sur les temps de correction des défauts de sécurité si la durée dépasse celle définie dans les Contrats de Niveau de Service (CNS). Assurez-vous que ces défauts sont automatiquement transférés dans le processus de gestion des risques et évalués selon une méthodologie quantitative cohérente. Évaluez comment des défauts donnés s'influencent / s'amplifient les uns avec les autres non seulement au niveau des équipes, mais aussi au niveau de l'ensemble de l'organisation. Utilisez la connaissance de la chaîne de compromission complète pour hiérarchiser, introduire et suivre les contrôles compensatoires atténuant les risques d'affaire respectifs.

            Intégrez votre système de gestion des défauts avec les outils automatisés introduits par d'autres pratiques, par ex.

                        * Génération et déploiement : faîtes échouer le processus de génération / déploiement si des défauts de sécurité supérieurs à une certaine sévérité affectent l'artefact final, à moins que quelqu'un ne signe explicitement l'exception.
            * Surveillance : si possible, faîtes en sorte que l'abus d'une faille de sécurité dans l'environnement de production soit détecté et déclenche une alerte.

        question: Est-ce que vous imposez des SLAs pour la correction des défauts de sécurité?
        quality_criteria:
            - Vous alertez automatiquement des violations du SLA et transférez les défauts associés au processus de gestion des risques
            - Vous intégrez les outils pertinents (par exemple pour la surveillance, la génération, le déploiement) avec le système de gestion des défauts

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
