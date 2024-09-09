---
title: Politique & Normes
type: stream
url: ./model/governance/policy-compliance/stream-a/
business_function: Gouvernance
business_function_url: governance
practice: Politique & Conformité
stream: A
description: Gouvernance / Politique & Conformité
keywords: ["Business function", "Practice", "Gouvernance", "Politique & Conformité"]
aliases:
    - /fr/model/G-PC-A-1
    - /fr/model/G-PC-A-2
    - /fr/model/G-PC-A-3
    - /fr/model/G-PC-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Attente claire du niveau de sécurité minimum dans l'organisation
        activity: |
            Élaborez une bibliothèque de politiques et de normes pour diriger tous les aspects du développement logiciel au sein de l'organisation. Les politiques et les normes sont basées sur les textes existants dans l’industrie et s'appliquant à celle de l'organisation. En raison de l'étendue des limites propres aux technologies et aux bonnes pratiques, ré-examinez les normes proposées avec les différentes équipes produits. Avec l'objectif général d'augmenter la sécurité des applications et des infrastructures informatiques, invitez les équipes produits à fournir des commentaires sur tous les aspects des normes qui ne seraient pas réalisables ou rentables à mettre en œuvre, ainsi que sur la possibilité d'aller plus loin que les normes avec peu d'efforts de la part des équipes produits.

            Pour les politiques, mettez l'accent sur des définitions de haut niveau et des aspects de la sécurité des applications qui ne dépendent pas d'une technologie spécifique ou de l'environnement d'hébergement. Concentrez-vous sur les objectifs plus larges de l'organisation pour protéger l'intégrité de son environnement informatique, la sécurité et la confidentialité des données et la maturité des cycles de vie du développement logiciel. Dans le cas des grandes organisations, les politiques peuvent sélectionner des exigences spécifiques en fonction de la classification des données ou des fonctionnalité des applications, mais ne devraient pas être suffisamment détaillées pour offrir des conseils technologiques.

            Pour les normes, incorporez les exigences mises en avant par les politiques, et concentrez-vous sur des conseils de mise en œuvre spécifiques à des technologies destinées à tirer parti des fonctionnalités de sécurité des différents langages de programmation et des environnements associés. Les commentaires des développeurs et des architectes seniors considérés comme des experts dans les diverses technologies utilisées par l'organisation sont requis sur les normes. Créez-les dans un format qui permet des mises à jour périodiques. Labellisez les exigences individuelles avec la politique dont elle provient ou ce qui vient d'une tierce partie, afin de rendre la maintenance et les audits plus faciles et plus efficaces.

        question: Avez-vous et appliquez-vous un ensemble commun de politiques et de normes à travers toute votre organisation?
        quality_criteria:
            - Vous avez adapté les normes existantes appropriées à l’industrie de l’organisation pour tenir compte des considérations spécifiques à votre domaine
            - Vos normes sont alignées sur vos politiques et intègrent des conseils spécifiques de mise en œuvre pour une technologie donnée

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Compréhension commune pour les équipes produit de la manière d'être en conformité avec les politiques de sécurité
        activity: |
            Afin d'aider à la mise en œuvre et à la vérification de la conformité aux politiques et aux normes, particularisez le process concernant la sécurité des applications et développez des scripts de test appropriés liés à chaque exigence applicable. Organisez les documents associés en bibliothèques et les mettre à la disposition de toutes les équipes concernées dans les formats les plus propices à leur inclusion dans chaque application. Labellisez clairement les documents et liez-les aux politiques et aux normes qu'ils représentent, afin d'aider à la mise à jour et à la maintenance. Faites différentes versions des politiques et des normes et incluent des journaux détaillés concernant les modifications lors de chaque mise à jour itérative pour faciliter leur inclusion continue dans les produits du SDLC.

            Écrivez les exigences de sécurité des applications dans un format compatible avec les processus de gestion des exigences existants. Il est possible que vous ayez besoin de plusieurs versions pour les adapter à différentes méthodologies de développement ou à différentes technologies. Le but est de faciliter l’intégration par les différentes équipes produit des politiques et des normes dans les cycles de développement existants et de limiter l'interprétation des exigences.

            Les scripts de test contribuent à renforcer les exigences de sécurité applicatifs par des attentes claires sur la fonctionnalité de l'application et à guider les efforts de test automatisés ou manuels qui peuvent déjà faire partie du processus de développement. Ces efforts n'aident pas seulement chaque équipe à déterminer l'état actuel du respect des politiques et des normes existantes, mais aussi à assurer la conformité au fur et à mesure que les applications continuent d'évoluer.

        question: Publiez-vous les politiques de l'organisation sous forme de scripts de test ou de manuels d'exécution dans le but de faciliter leur interprétation par les équipes de développement?
        quality_criteria:
            - Vous créez des listes de vérification et des scripts de test quand c'est pertinent, conformément aux exigences de la politique et aux directives d'implémentation des normes associées
            - Vous créez des versions adaptées à chaque méthodologie de développement et à chaque technologie que l'organisation utilise

        answers:
            - "No"
            - Oui, du contenu
            - Oui, au moins la moitié du contenu
            - Oui, la plupart ou la totalité du contenu

    level3:
        level: 3
        benefit: |
            Comprendre le respect des politiques et des normes par votre organisation
        activity: |
            Élaborez un programme pour mesurer la conformité de chaque application aux politiques et aux normes existantes. Les exigences obligatoires devraient être motivées et communiquées de façon cohérentes à travers les différentes équipes. Dans la mesure du possible, liez le statut de conformité à des tests automatisés et faites un rapport pour chaque version. Les rapports de conformité contiennent la version des politiques et des normes et les indicateurs appropriés de couverture du code.

            Encouragez les équipes non-conformes à revoir les ressources disponibles telles que les exigences de sécurité et les scripts de test afin de vous assurer que la non-conformité n'est pas le résultat de conseils inadéquats. Faites suivre les problèmes résultant de conseils insuffisants aux équipes responsables de la publication des exigences d'application et des scripts de test afin d'inclure les corrections dans les versions futures. Faites remonter les problèmes résultant de l'incapacité à répondre aux politiques et aux normes vers les équipes qui gèrent les risques de sécurité des applications.

        question: Faites-vous régulièrement état du respect de la politique et des normes et utilisez-vous ces informations pour guider les efforts d’amélioration de la conformité?
        quality_criteria:
            - Vous avez des procédures (automatisées, si possible) pour générer régulièrement des rapports de conformité
            - Vous transmettez des rapports de conformité à toutes les parties prenantes concernées
            - Les parties prenantes utilisent les informations remontées sur l'état de conformité pour identifier les domaines à améliorer

        answers:
            - "No"
            - Oui, mais la remontée d'information est ad-hoc
            - Oui, nous remontons les informations régulièrement
            - Oui, nous remontons les informations au moins une fois par an

---
