---
title: Gestion des Secrets
type: stream
url: ./model/implementation/secure-deployment/stream-b/
business_function: Implémentation
business_function_url: implementation
practice: Déploiement Sécurisé
stream: B
description: Implémentation / Déploiement Sécurisé
keywords: ["Business function", "Practice", "Implémentation", "Déploiement Sécurisé"]
aliases:
    - /fr/model/I-SD-B-1
    - /fr/model/I-SD-B-2
    - /fr/model/I-SD-B-3
    - /fr/model/I-SD-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Accès limité et défini à vos secrets de production
        activity: |
            Les développeurs ne devraient pas avoir accès aux secrets ou aux informations d'identification des environnements de production. Ayez un mécanisme en place pour protéger adéquatement les secrets de production, par exemple (i) en ayant des personnes spécifiques qui les ajoutent aux fichiers de configuration pertinents au moment du déploiement (le principe de séparation du devoir) ou (ii) en chiffrant les secrets de production contenus dans les fichiers de configuration.

            N'utilisez pas de secrets de production dans les fichiers de configuration pour les environnements de développement ou de test, car il se peut que ces environnements aient une posture de sécurité nettement plus faible. De même, ne gardez pas les secrets non protégés dans des fichiers de configuration stockés dans des dépôts de code.

            Stockez les identifiants sensibles et les secrets pour les systèmes de production sous forme chiffrée tout le temps. Envisagez d'utiliser un outil spécifiquement conçu pour cela. Gérez soigneusement la gestion des clés de sorte que seul le personnel responsable des déploiements en production soit en mesure d’accéder à ces données.

        question: Limitez-vous l'accès aux secrets de l'application selon le principe du moindre privilège?
        quality_criteria:
            - Vous stockez les secrets de production de façon sûre dans un endroit sécurisé
            - Les développeurs n'ont pas accès aux secrets de production
            - Les secrets de production ne sont pas disponibles hors de l'environnement de production

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Détection de fuites potentielles de secrets de production
        activity: |
            Ayez un processus automatisé pour ajouter des informations d'identification et des secrets aux fichiers de configuration pendant le processus de déploiement aux étapes concernées. De cette façon, les développeurs et les personnes en charge des déploiements ne voient pas ou ne gèrent pas ces valeurs sensibles.

            Mettez en œuvre des vérifications qui détectent la présence de secrets dans les dépôts de code et les fichiers et exécutez-les périodiquement. Configurez les outils pour rechercher des chaînes connues et des chaînes potentiellement dangereuses inconnues. Dans les systèmes tels que les dépôts de code où il y a un historique, incluez les versions dans les vérifications. Marquez les secrets potentiels que vous découvrirez comme des valeurs sensibles et retirez-les lorsque c'est pertinent. Si vous ne pouvez pas les supprimer d'un fichier historique dans un dépôt de code par exemple, vous devrez peut-être actualiser la valeur sur le système qui consomme le secret. De cette façon, si un attaquant découvre le secret, il ne leur sera pas utile.

            Rendez le système utilisé pour stocker et traiter les secrets et les identifiants robustes du point de vue de la sécurité. Chiffrez tous les secrets au repos et en transit. Les utilisateurs qui configurent ce système et les secrets qu'il contient sont soumis au principe du moindre privilège. Par exemple, un développeur peut avoir besoin de gérer les secrets d'un environnement de développement, mais pas d'un environnement de test ou de production de validation utilisateur.

        question: Injectez-vous les secrets de production dans les fichiers de configuration pendant le déploiement?
        quality_criteria:
            - Les fichiers de code source ne contiennent plus les secrets actifs de l'application
            - Dans des circonstances normales, aucun humain n'accède aux secrets lors des procédures de déploiement
            - Vous enregistrez et avertissez de tout accès anormal aux secrets

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Possibilité réduite et détection rapide d'abus de secrets de production
        activity: |
            Mettez en œuvre la gestion du cycle de vie des secrets de production et assurez la génération de nouveaux secrets autant que possible, et cela pour chaque instance d'application. L'utilisation de secrets par instance d'application garantit que les comportements inattendus de l'application peut être retracé et correctement analysés. Des outils peuvent aider à mettre à jour automatiquement et de façon transparente les secrets dans tous les endroits pertinents lors de la survenue de changements.

            Assurez-vous que tous les accès aux secrets (en lecture et en écriture) sont enregistrés dans une infrastructure centrale. Examinez régulièrement ces journaux pour identifier les comportements inattendus et effectuez une analyse adéquate pour comprendre pourquoi cela s'est produit. Envoyez les problèmes et les causes racines vers la pratique de gestion des défauts pour gerantir que l'organisation prendra en compte toutes les situations inacceptables.

        question: Pratiquez-vous une gestion adéquate du cycle de vie des secrets de l'application?
        quality_criteria:
            - Vous générez et synchronisez les secrets en utilisant une solution éprouvée
            - Les secrets sont différents entre les différentes instances de l'application
            - Les secrets sont régulièrement mis à jour

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
