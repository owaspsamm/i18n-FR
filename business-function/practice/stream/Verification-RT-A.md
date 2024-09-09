---
title: Vérification des contrôles
type: stream
url: ./model/verification/requirements-driven-testing/stream-a/
business_function: Vérification
business_function_url: verification
practice: Tests axés sur les exigences
stream: A
description: Vérification / Tests axés sur les exigences
keywords: ["Business function", "Practice", "Vérification", "Tests axés sur les exigences"]
aliases:
    - /fr/model/V-RT-A-1
    - /fr/model/V-RT-A-2
    - /fr/model/V-RT-A-3
    - /fr/model/V-RT-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Efficacité vérifiée de vos contrôles de sécurité standards
        activity: |
            Effectuez des tests de sécurité pour vérifier que les contrôles standards de sécurité logiciels fonctionnent comme prévu. À un haut niveau, cela signifie tester le bon fonctionnement des contrôles liés à la confidentialité, à l'intégrité et à la disponibilité des données ainsi que du service. Les tests de sécurité comprennent au moins des tests d'authentification, de contrôle d'accès, de validation des entrées, d'encodage, d'échappement des données et de chiffrement. L'objectif des tests est de valider que les contrôles de sécurité sont correctement implémentés.

            Les tests de sécurité valident les contrôles de sécurité logiciels nécessaires. Effectuez des tests de sécurité de vérification des contrôles manuellement ou avec des outils à chaque fois que l'application change son utilisation des contrôles. Les techniques telles que les basculements de fonctionnalités et les tests A/B peuvent être utilisées pour exposer progressivement des fonctionnalités à un public plus large au fur et à mesure qu'elles sont suffisamment validées. La vérification des contrôles logiciels est obligatoire pour tous les logiciels qui font partie du programme SAMM.

        question: Testez-vous les applications quant au bon fonctionnement des contrôles de sécurité standards?
        quality_criteria:
            - Les tests de sécurité vérifient au moins l'implémentation de l'authentification, du contrôle d'accès, de la validation des entrées, de l'encodage et de l'échappement des données et des contrôles de chiffrement
            - Les tests de sécurité s'exécutent chaque fois que l'application change son utilisation des contrôles

        answers:
            - "No"
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level2:
        level: 2
        benefit: |
            Intégration des exigences de sécurité dans les scénarios de test
        activity: |
            À partir des exigences de sécurité, identifiez et implémentez un ensemble de scénarios de tests de sécurité afin de vérifier si le fonctionnement du logiciel est correct. Pour avoir un programme de test réussi, il est impératif de connaître les objectifs de test, spécifiés par les exigences de sécurité.

            Dérivez les cas de tests de sécurité pour les applications visées à partir des exigences de sécurité créées dans le cadre de la pratique "Exigences de Sécurité" du SAMM. Pour valider les exigences de sécurité avec des tests de sécurité, les exigences de sécurité sont basées sur des actions et mettent en évidence les fonctionnalités attendues (le quoi) et, implicitement, l'implémentation (le comment). Ces exigences sont également appelées « exigences positives », car elles indiquent les fonctionnalités attendues qui peuvent être validées par le biais de tests de sécurité. Parmi les exemples de conditions positives, citons : « l'application va verrouiller la session de l'utilisateur après six tentatives de connexion invalides» ou « les mots de passe doivent comporter au moins six caractères alphanumériques ». La validation des exigences positives consiste à confirmer la fonctionnalité attendue. Vous pouvez faire cela en recréant les conditions de test et en exécutant le test selon des entrées prédéfinies. Affichez les résultats sous la forme d'échec ou de réussite.

            Souvent, il est plus efficace d'utiliser du temps de l'équipe du projet pour construire des cas de test spécifiques à une application et d'employer des ressources disponibles au public ou des bases de connaissances achetées à l'extérieur pour sélectionner les cas de tests généraux applicables à la sécurité. Le personnel compétent en matière de développement, de sécurité et d'assurance qualité examine les cas de test candidats pour leur applicabilité, leur efficacité et leur faisabilité. Etablissez les cas de test pendant la rédaction des exigences et / ou la phase de conception de la fonctionnalité. Tester les exigences de sécurité fait partie des tests fonctionnels du logiciel.

        question: Écrivez-vous et exécutez-vous de façon cohérente des scripts de test pour vérifier la bonne mise en place des exigences de sécurité?
        quality_criteria:
            - Vous adaptez les tests à chaque application et confirmez les fonctionnalités de sécurité attendues
            - Vous capturez les résultats de test comme une condition de réussite ou d'échec
            - Les tests utilisent un cadre standardisé ou DSL

        answers:
            - "No"
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level3:
        level: 3
        benefit: |
            Détection rapide et fiable des violations des exigences de sécurité
        activity: |
            Écrivez et automatisez les tests de régression pour tous les bogues identifiés (et corrigés) afin de vous assurer que ceux-ci forment un harnais de tests empêchant des problèmes similaires d'être introduits dans les versions ultérieures. Les tests unitaires de sécurité devraient vérifier dynamiquement (à savoir au moment de l'exécution) que les composants fonctionnent comme prévu et devraient valider que les changements de code sont correctement implémentés.

            Une bonne pratique pour les développeurs est de construire des cas de tests de sécurité sous la forme d'une suite de tests de sécurité génériques faisant partie de l'environnement de tests unitaires existant. Une suite de tests de sécurité génériques peut inclure des cas de tests de sécurité pour valider les exigences à la fois positives et négatives pour les contrôles de sécurité tels que l'Identification, l'Authentification & le Contrôle d'accès, la Validation et l'Encodage des entrées, la Gestion des utilisateurs et des sessions, la Gestion des erreurs et des exceptions, le Chiffrement et l'Audit et la Journalisation. Vérifiez la bonne exécution des tests de sécurité aussi tôt que possible. Si possible par exemple, envisagez d'exécuter les tests de sécurité dans le cadre des exigences d'intégration avant de permettre à du nouveau code d'entrer dans la base de code principale. Sinon, envisagez leur exécution comme condition à la validation d"une génération.

            Pour les tests fonctionnels de sécurité, utilisez des tests de niveau unitaire pour les fonctionnalités de contrôle de sécurité au niveau des composants logiciels, comme les fonctions, les méthodes ou les classes. Par exemple, un cas de test pourrait vérifier la validation des entrées et des sorties (par ex., l'assainissement des variables) et vérifier les limites des variables en confirmant les fonctionnalités attendues du composant.

        question: Testez-vous automatiquement les applications pour les régressions de sécurité ?
        quality_criteria:
            - Vous écrivez systématiquement des tests pour tous les bogues identifiés (dépassant éventuellement un seuil de sévérité prédéfini)
            - Vous rassemblez les tests de sécurité dans une suite de tests qui fait partie du cadre de référence des tests unitaires existants

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
