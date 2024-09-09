---
title: Réponse à Incident
type: stream
url: ./model/operations/incident-management/stream-b/
business_function: Opérations
business_function_url: operations
practice: Gestion des incidents
stream: B
description: Opérations / Gestion des incidents
keywords: ["Business function", "Practice", "Opérations", "Gestion des incidents"]
aliases:
    - /fr/model/O-IM-B-1
    - /fr/model/O-IM-B-2
    - /fr/model/O-IM-B-3
    - /fr/model/O-IM-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Capacité à résoudre efficacement les incidents de sécurité les plus courants
        activity: |
            La première étape consiste à reconnaître la réalité de la compétence en matière de réponse à incident et à définir un responsable dédié. Fournissez-leur le temps et les ressources dont ils ont besoin pour suivre l'état actuel des bonnes pratiques en matière de gestion des incidents et des outils forensiques.

            À ce niveau de maturité, il se peut que vous n'ayez pas mis en place une équipe de réponse à incident dédiée, mais vous avez clarifié les participants au processus (généralement différents rôles). Définissez un point de contact unique pour le processus, connu de toutes les parties prenantes concernées. Veiller à ce que ce point de contact sache joindre chaque participant et définissez les responsabilités d'astreinte pour ceux qui en ont une.

            Lorsque des incidents de sécurité se produisent, documentez toutes les actions prises. Protégez ces informations contre tout accès non autorisé.

        question: Répondez-vous aux incidents détectés?
        quality_criteria:
            - Vous avez une personne ou un rôle défini pour la gestion des incidents
            - Vous documentez les incidents de sécurité

        answers:
            - Non
            - Oui, pour certains incidents
            - Oui, pour au moins la moitié des incidents
            - Oui, pour la plupart ou tous les incidents

    level2:
        level: 2
        benefit: |
            Compréhension et gestion efficace de la plupart des incidents de sécurité
        activity: |
            Mettez en place et documentez le processus officiel d'intervention en cas d'incident de sécurité. Assurez-vous que la documentation inclut des informations telles que :

            * les scénarios les plus probables / courants d'incidents de sécurité et des instructions de haut niveau pour les gérer ; pour de tels scénarios, utilisez également les connaissances publiques sur les incidents pertinents étant éventuellement survenus chez les tierces parties,
            * les règles pour orienter chaque incident,
            * les règles pour la participation des différentes parties prenantes, y compris la Direction Générale, les Relations Publiques, le Département Juridique, celui en charge de la Confidentialité, les Ressources Humaines, les autorités externes (Forces de l'Ordre) et les clients ; spécifiez le délai obligatoire pour ce faire, si nécessaire,
            * le processus pour effectuer une analyse de la cause racine et la documentation de ses résultats.

            Assurez-vous qu'une équipe d'intervention en cas d'incidents bien formée et bien informée est disponible pendant et en dehors des heures de bureau. Définissez les calendriers d'action et une salle de réunion de crise. Gardez les outils matériels et logiciels à jour et prêts à être utilisés à tout moment.

        question: Utilisez-vous un processus reproductible pour gérer les incidents ?
        quality_criteria:
            - Vous avez une classification des incidents validée
            - Le processus utilise l'analyse de cause racine pour les incidents de haute sévérité
            - Les employés responsables de la réponse à incident sont formés à ce processus
            - De l'outillage d'analyse forensique est disponible

        answers:
            - Non
            - Oui, pour certains types d'incident
            - Oui, pour au moins la moitié des types d'incidents
            - Oui, pour la plupart ou tous les types d'incidents

    level3:
        level: 3
        benefit: |
            Une réponse à incident efficace et indépendante du moment, de l'emplacement ou du type d'incident
        activity: |
            Mettez en place une équipe d'intervention dédiée en cas d'incident, disponible en permanence et responsable de l'amélioration continue du processus avec l'aide des ACR courantes. Pour les organisations éparses, définissez et documentez des règles logistiques pour tous les lieux pertinents si cela est raisonnable.

            Documentez des procédures détaillées de réponse à incident et tenez-les à jour. Automatisez les procédures lorsque cela est possible. Conservez toutes les ressources nécessaires à ces procédures (par ex., infrastructure de communication séparée ou emplacement externe fiable) prêtes à l'emploi. Détectez et corrigez l'indisponibilité de ces ressources en temps opportun.

            Effectuez des exercices de gestion des incidents et d'urgence régulièrement. Utilisez les résultats pour améliorer le processus.

            Définissez, recueillez, évaluez et agissez en fonction des métriques sur le processus de réponse à incident, y compris sur son amélioration continue.

        question: Avez-vous une équipe de réponse à incident dédiée et disponible?
        quality_criteria:
            - L'équipe effectue des analyses pour identifier la cause racine pour tous les incidents de sécurité sauf s'il y a une raison spécifique de ne pas le faire
            - Vous réexaminez et mettez à jour le processus de réponse au moins une fois par an

        answers:
            - Non
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

---
