---
title: Mise à jour et Correctifs
type: stream
url: ./model/operations/environment-management/stream-b/
business_function: Opérations
business_function_url: operations
practice: Gestion de l'environnement
stream: B
description: Opérations / Gestion de l'environnement
keywords: ["Business function", "Practice", "Opérations", "Gestion de l'environnement"]
aliases:
    - /fr/model/O-EM-B-1
    - /fr/model/O-EM-B-2
    - /fr/model/O-EM-B-3
    - /fr/model/O-EM-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Atténuation des problèmes connus dans les composants tiers
        activity: |
            Identifiez les applications et les composants tiers qui doivent être mis à jour ou corrigés, y compris les systèmes d'exploitation sous-jacents, les serveurs d'applications et les bibliothèques de codes provenant de tiers.

            À ce niveau de maturité, vos activités d'identification et de correction sont en fonction de vos moyens et ad hoc, sans processus géré pour le suivi des versions des composants, des disponibilités des mises à jour et du statut des correctifs. Cependant, des exigences de haut niveau pour les activités liées aux correctifs (p. ex. tester les correctifs avant de les déployer en production) peuvent exister, les équipes produits faisant de leur mieux pour se conformer à ces exigences.

            Sauf pour les mises à jour de sécurité critiques (par ex. une preuve de concept pour un composant tiers publiquement publiée), les équipes tirent parti des fenêtres de maintenance en place à d'autres fins pour appliquer les correctifs des composants. Pour les logiciels développés par l'organisation, les correctifs des composants sont livrés aux clients et aux solutions gérées par l'organisation uniquement dans le cadre des versions contenant des fonctionnalités.

            Les équipes partagent leur connaissance des mises à jour disponibles et leurs expériences de correction sur une base ad hoc. Veillez à ce que les équipes soient en mesure de déterminer les versions de tous les composants utilisés afin de pouvoir évaluer si leurs produits sont affectés par une vulnérabilité de sécurité lorsqu'ils sont notifiés. Cependant, le processus de génération et de mise à jour des listes de composants peut nécessiter un effort considérable de la part des analystes.

        question: Identifiez-vous et déployez-vous les correctifs pour les composants vulnérables ?
        quality_criteria:
            - Vous avez une liste à jour des composants comprenant les informations de version
            - Vous examinez régulièrement les sources publiques à propos des vulnérabilités liées à vos composants

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

    level2:
        level: 2
        benefit: |
            Mise à jour cohérente et proactive des composants de la pile technologique
        activity: |
            Développez et suivez un processus bien défini de gestion des correctifs des composants d'application à travers les piles technologiques utilisées. Assurez-vous que les processus incluent des plans de travail réguliers pour l'application des mises à jour des fournisseurs, alignés sur les calendriers de mise à jour des fournisseurs (par exemple, Microsoft Patch Tuesday). Pour les logiciels développés par l'organisation, livrez des versions et autres solutions gérées par l'organisation aux clients sur une base régulière (par ex. mensuellement), que vous incluiez de nouvelles fonctionnalités ou non.

            Créez de la documentation pour prioriser les patchs de composants en reflétant votre tolérance au risque et vos objectifs de gestion. Prenez en compte les facteurs opérationnels (par exemple la criticité de l'application ou la sévérité des vulnérabilités traitées) dans la détermination des priorités de test et d'application des correctifs.

            En cas de notification d'une vulnérabilité critique dans un composant tandis qu'aucun correctif n'est encore disponible, orientez et traitez la situation comme un problème de gestion des risques (c.a.d. mettez en place des contrôles compensatoires, obtenez l'acceptation du risque de la part du client ou désactivez les applications / fonctionnalités affectées).

        question: Suivez-vous un processus établi pour la mise à jour des composants de vos piles technologiques?
        quality_criteria:
            - Le processus inclut les informations du fournisseur pour les correctifs provenant de tiers
            - Le processus prend en compte les sources externes pour le recueil des informations sur les attaques zéro jour et comprend des étapes pertinentes pour l'atténuation des risques
            - Le processus comprend des conseils pour établir des priorités sur les mises à jour de composants

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

    level3:
        level: 3
        benefit: |
            Transparence sur l'état de mise à jour des composants pour éviter les non-conformités
        activity: |
            Élaborez et utilisez des tableaux de bord / rapports de gestion pour suivre la conformité avec les processus sur les correctifs et les ANS à travers le portefeuille. Veillez à ce que la gestion des dépendances et les processus d'empaquetage d'applications puissent prendre en charge l'application de correctifs au niveau des composants à tout moment afin de répondre aux ANS requis.

            Traitez les mises à jour manquantes comme des défauts des produits liés à la sécurité, et gérez leur triage et leur correction conformément à votre pratique établie de gestion des défauts.

            Ne comptez pas sur les notifications de routine des fournisseurs de composants pour en savoir plus sur les vulnérabilités et les correctifs associés. Surveillez une sélection de sources externes de renseignements sur les menaces pour en savoir plus sur les vulnérabilités zéro jour ; gérez celles qui affectent vos applications comme des problématiques de gestion des risques.

        question: Évaluez-vous régulièrement les composants et revoyez-vous l'état de la mise à niveau?
        quality_criteria:
            - Vous mettez à jour la liste avec les composants et les versions
            - Vous identifiez et mettez à jour les mises à jour manquantes selon le SLA existant
            - Vous revoyez et mettez à jour le processus en fonction des commentaires des personnes qui déploient les correctifs

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

---
