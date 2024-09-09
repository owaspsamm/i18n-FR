---
title: Validation de l'Architecture
type: stream
url: ./model/verification/architecture-assessment/stream-a/
business_function: Vérification
business_function_url: verification
practice: Évaluation de l'architecture
stream: A
description: Vérification / Évaluation de l'architecture
keywords: ["Business function", "Practice", "Vérification", "Évaluation de l'architecture"]
aliases:
    - /fr/model/V-AA-A-1
    - /fr/model/V-AA-A-2
    - /fr/model/V-AA-A-3
    - /fr/model/V-AA-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Compréhension de l'architecture de haut niveau et des mesures de sécurité adaptées
        activity: |
            Créez une vue d'ensemble de l'architecture et examinez-là pour vérifier la bonne présence de mécanismes de sécurité généraux tels que l'authentification, la gestion des autorisations, des utilisateurs et des droits, la communication sécurisée, la protection des données, la gestion des clés et la gestion des journaux. Considérez également le soutien à la protection de la vie privée. Faites cela en utilisant les artefacts du projet tels que des documents d'architecture ou de conception, ou des entrevues avec les représentants du client et le personnel technique. Pensez également aux composants d'infrastructure - ce sont tous les systèmes, composants et bibliothèques (y compris les SDKs) qui ne sont pas spécifiques à l'application mais fournissent un support direct à l'utilisation ou à la gestion de l'application au sein de l'organisation.

            Mettez en exergue toutes les fonctionnalités liées à la sécurité dans l'architecture et validez sa pertinence. Faites cela de manière ad hoc, du point de vue des utilisateurs anonymes, des utilisateurs authentifiés et des rôles spécifiques à l'application.

        question: Examinez-vous l'architecture de l'application en fonction des principaux objectifs de sécurité de manière ponctuelle ?
        quality_criteria:
            - Vous avez un modèle validé de l'architecture globale du logiciel
            - Vous incluez les composants, les interfaces et les intégrations dans le modèle d'architecture
            - Vous vérifiez la bonne disposition des mécanismes de sécurité généraux
            - Vous enregistrez les contrôles de sécurité manquants comme des défauts

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Un processus cohérent de revue d'architecture à travers votre organisation
        activity: |
            Vérifiez que l'architecture de la solution répond à toutes les exigences de sécurité et de conformité identifiées. Pour chaque interface de l'application, itérez à travers la liste des exigences de sécurité et de conformité et analysez l'architecture pour valider leur bonne disposition. Effectuez également une analyse interactive ou une analyse du flux de données pour vous assurer que les exigences sont traitées de manière adéquate à travers les différents composants. Détaillez l'analyse jusqu'à montrer les caractéristiques de conception qui répondent à chaque exigence.

            Effectuez ce type d'analyse à la fois sur les interfaces internes, par exemple entre les composants, ainsi que sur les interfaces externes, par exemple celles faisant partie de la surface d'attaque. Identifiez et validez également les décisions de conception importantes prises dans le cadre du travail d'architecture, en particulier lorsqu'elles s'écartent des solutions de sécurité partagées disponibles au sein de l'organisation. Enfin, mettez à jour les résultats en fonction des modifications apportées pendant le cycle de développement et prenez note de toutes les exigences qui ne sont pas clairement identifiées au niveau de la conception comme ayant été traitées.

        question: Examinez-vous régulièrement les mécanismes de sécurité de votre architecture?
        quality_criteria:
            - Vous examinez la conformité avec les exigences internes et externes
            - Vous passez en revue systématiquement chaque interface du système
            - Vous utilisez une méthode de revue formalisée et une validation structurée
            - Vous enregistrez les mécanismes de sécurité manquants comme des défauts

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Garantie de l'efficacité des contrôles d'architecture
        activity: |
            Examinez l'efficacité des composants d'architecture et des mécanismes de sécurité qu'ils fournissent en termes d'alignement sur la stratégie globale de l'organisation et examinez attentivement le degré de disponibilité, de passage à l'échelle et de professionnalisme des solutions de sécurité choisies. Tandis que certains choix tactiques pour une application donnée peuvent avoir un sens dans des contextes spécifiques, Il est important de garder l'œil ouvert sur la situation générale et de garantir la pérennité de la solution conçue.

            Enregistrez toute anomalie dans le système de gestion des défauts pour contribuer à de futures améliorations de l'architecture.

        question: Examinez-vous régulièrement l'efficacité des contrôles de sécurité?
        quality_criteria:
            - Vous évaluez les capacités de prévention, de détection et de réponse des contrôles de sécurité
            - Vous évaluez l'alignement sur la stratégie, le support approprié et la capacité de mise à l'échelle des contrôles de sécurité
            - Vous évaluez l'efficacité au moins une fois par an
            - Vous enregistrez les lacunes identifiées comme des défauts

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
