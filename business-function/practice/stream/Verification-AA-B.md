---
title: Réduction de risques architecturale
type: stream
url: ./model/verification/architecture-assessment/stream-b/
business_function: Vérification
business_function_url: verification
practice: Évaluation de l'architecture
stream: B
description: Vérification / Évaluation de l'architecture
keywords: ["Business function", "Practice", "Vérification", "Évaluation de l'architecture"]
aliases:
    - /fr/model/V-AA-B-1
    - /fr/model/V-AA-B-2
    - /fr/model/V-AA-B-3
    - /fr/model/V-AA-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            S'assure que l'architecture protège des menaces de sécurité typiques.
        activity: |
            Examinez l'architecture pour trouver des menaces de sécurité typiques. Le personnel technique compétent en matière de sécurité conduit cette analyse avec les commentaires des architectes, des développeurs, des gestionnaires et des représentants du client en fonction du besoin pour s'assurer que l'architecture prend en compte toutes les menaces courantes que les équipes de développement qui n'ont pas d'expertise spécialisée en sécurité peuvent avoir négligées.

            Les menaces typiques dans une architecture peuvent être liées à des hypothèses incorrectes ou à une dépendance trop forte envers des mécanismes de sécurité tels que l'authentification, la gestion des autorisations, des utilisateurs et des droits, la communication sécurisée, la protection des données, la gestion des clés ou la gestion des journaux. A l'opposé, les menaces peuvent être liées à des limitations ou des problèmes connus dans des composants ou des environnements technologiques qui font partie de la solution et pour lesquels une atténuation insuffisante a été mise en place.

        question: Passez-vous en revue l'architecture de l'application afin d'atténuer les menaces typiques de manière ponctuelle ?
        quality_criteria:
            - Vous avez un modèle validé de l'architecture globale du logiciel
            - Le personnel compétent en matière de sécurité conduit l'examen
            - Vous considérez différents types de menaces, y compris celles venant de l'intérieur et celles liées aux données

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Toutes les menaces identifiées envers l'application sont traitées de manière adéquate.
        activity: |
            Examinez systématiquement chaque menace identifiée lors des activités d'évaluation des menaces et vérifiez la manière dont l'architecture les atténue. Utilisez un processus standardisé pour analyser les architectures systèmes et le flux de données à l'intérieur de celles-ci. Ceci est généralement lié au modèle de menace utilisé (par ex. STRIDE) afin d’identifier les objectifs de sécurité pertinents qui répondent à chaque type de menace. Pour chaque menace, identifiez les fonctionnalités de niveau conception de l'architecture qui la contrecarrent et évaluez son efficacité.

            Lorsqu'elles sont disponibles, revoyez les informations concernant les décisions architecturales afin de comprendre les contraintes d'architecture et les compromis réalisés lors de la conception. Tenez compte de leurs impacts ainsi que de toutes les hypothèses liées à la sécurité sur lesquelles le fonctionnement sûr du système repose et réévaluez-les.

            Enrichissez votre modèle de menace précédemment créé de telle sorte que chaque menace et l'impact estimé associé soient liés au contrôle correspondant. Produisez un document de cartographie ou un tableau de bord dans un outil spécialisé afin de rendre l'information disponible et visible aux parties prenantes concernées.

        question: Évaluez-vous régulièrement les menaces qui pèsent sur votre architecture ?
        quality_criteria:
            - Vous examinez systématiquement chaque menace identifiée lors de l'évaluation des menaces
            - Des personnes formées ou expérimentées mènent l'exercice de revue
            - Vous identifiez des fonctionnalités d'atténuation de niveau conception pour chaque menace identifiée
            - Vous enregistrez les menaces non prises en compte comme des défauts

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Amélioration continue de l'architecture d'entreprise basée sur les revues d'architecture
        activity: |
            En tant qu'organisation, vous pouvez encore améliorer votre posture de sécurité logicielle en comprenant les menaces qui ne sont pas traitées dans les architectures logicielles et en adaptant vos tactiques pour éviter cela. Formalisez un processus pour utiliser les identifications de problèmes d'architecture récurrents comme déclencheur afin d'identifier les causes des lacunes dans l'évaluation de la sécurité et y faire face. Renvoyez les résultats vers la phase de conception en créant ou en mettant à jour les architectures de référence pertinentes, les solutions de sécurité existantes ou les principes et modèles de conception de l'organisation.

        question: Mettez-vous régulièrement à jour vos architectures de référence en fonction des résultats de l'évaluation de l'architecture ?
        quality_criteria:
            - Vous évaluez vos architectures de manière standardisée et documentée
            - Vous utilisez les découvertes récurrentes pour déclencher une révision des architectures de référence
            - Vous examinez de façon indépendante la qualité des revues d'architecture de manière ponctuelle
            - Vous utilisez les mises à jour de l'architecture de référence pour déclencher des examens des solutions partagées pertinentes, en fonction des risques.

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
