---
title: Modélisation des Menaces
type: stream
url: ./model/design/threat-assessment/stream-b/
business_function: Conception
business_function_url: design
practice: Évaluation de la menace
stream: B
description: Conception / Évaluation de la menace
keywords: ["Business function", "Practice", "Conception", "Évaluation de la menace"]
aliases:
    - /fr/model/D-TA-B-1
    - /fr/model/D-TA-B-2
    - /fr/model/D-TA-B-3
    - /fr/model/D-TA-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Identification des défauts de conception architecturale dans vos applications
        activity: |
            La modélisation des menaces est une activité structurée qui a pour but d'identifier, d'évaluer et de gérer les menaces du système, les défauts de conception de l'architecture et de recommander des mesures de sécurité. Elle est généralement effectuée dans le cadre de la phase de conception ou dans le cadre d'une évaluation de sécurité.

            La modélisation de menace est un exercice d'équipe, incluant les product owners, les architectes, les champions de la sécurité et les testeurs de la sécurité. À ce niveau de maturité, exposer les équipes et les parties prenantes à la modélisation des menaces afin d'accroître leur sensibilisation à la sécurité et de créer une vision partagée de la sécurité du système.

            Au niveau de maturité 1, vous réalisez la modélisation des menaces de façon ad hoc pour les applications à haut risque et utilisez de simples listes de contrôle de menaces, telles que STRIDE. Évitez de longs ateliers et des listes trop détaillées de menaces peu pertinentes. Effectuez la modélisation des menaces de manière itérative pour vous aligner sur les paradigmes de développement plus itératifs. Si vous ajoutez de nouvelles fonctionnalités à une application existante, n'examinez que les fonctions nouvellement ajoutées au lieu d'essayer de couvrir l'ensemble du périmètre. Un bon point de départ est les diagrammes existants que vous annotez lors des ateliers de discussion. Assurez-vous de toujours sauvegarder le résultat d'une discussion sur la modélisation des menaces pour une utilisation ultérieure.

            Votre outil le plus important pour démarrer la modélisation des menaces est un tableau blanc, un tableau intelligent ou un bout de papier. Visez la sensibilisation à la sécurité, un processus simple et des résultats réalisables sur lesquels vous vous mettez d'accord avec votre équipe.

        question: Identifiez-vous et gérez-vous les défauts de conception architecturaux avec la modélisation des menaces?
        quality_criteria:
            - Vous réalisez la modélisation des menaces pour les applications à haut risque
            - Vous utilisez des listes de contrôle de menace simples, telles que STRIDE
            - Vous archivez le résultat d'un modèle de menace pour une utilisation ultérieure

        answers:
            - Non
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level2:
        level: 2
        benefit: |
            Des attentes claires quant à la qualité des activités de modélisation des menaces
        activity: |
            Utilisez une méthodologie standardisée de modélisation des menaces pour votre organisation et alignez-la sur les niveaux de risque de votre application. Pensez à des moyens de permettre la mise à l'échelle de la modélisation des menaces pour l'ensemble de l'organisation.

            Formez vos architectes, vos champions de sécurité et autres parties prenantes sur la manière de faire opérationnellement la modélisation des menaces. La modélisation de la menace nécessite de la connaissance, des manuels et des modèles clairs, des exemples spécifiques à l'organisation et de l'expérience, ce qui est difficile à automatiser.

            Votre méthodologie de modélisation des menaces comprend au moins l'établissement de diagrammes, l'identification des menaces, l'atténuation des défauts de conception et la façon de valider les artéfacts de vos modèles de menaces. Votre diagramme de modélisation des menaces permet une compréhension détaillée de l'environnement et de la mécanique de l'application. Vous découvrez les menaces envers votre application ou d'autres menaces spécifiques à votre organisation avec des listes de contrôle telles que STRIDE. Pour les défauts de conception identifiés (classés en fonction du risque envers votre organisation), vous ajoutez des contrôles d'atténuation pour aider les parties prenantes à faire face à des menaces particulières. Définissez ce qui déclenche la mise à jour d'un modèle de menace, par exemple un changement de technologie ou le déploiement d'une application dans un nouvel environnement.

            Stockez les sorties de la modélisation des menaces au sein du processus de gestion des défauts pour un suivi adéquat. Capturez les artefacts de modélisation des menaces avec des outils qui sont utilisés par vos équipes applicatives.

        question: Utilisez-vous une méthodologie standard, en phase avec le niveau de risque de votre application ?
        quality_criteria:
            - Vous formez vos architectes, vos champions de sécurité et les autres parties prenantes sur la manière de modéliser les menaces de façon pratique
            - Votre méthodologie de modélisation des menaces comprend au moins la réalisation de diagrammes, l'identification des menaces, l'atténuation des défauts de conception et la validation des artefacts de votre modèle de menace
            - Les changements dans le contexte de l'application ou de l'entreprise déclenchent un examen des modèles de menace pertinents
            - Vous capturez les artefacts de modélisation des menaces avec des outils qui sont utilisés par vos équipes d'application

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Assurance de l'amélioration continue des activités de modélisation des menaces
        activity: |
            La modélisation des menaces est intégrée dans votre SDLC et fait partie de la culture de sécurité des développeurs. Des modèles de risque réutilisables, composé de bibliothèques de menaces, de défauts de conception et de mesures d'atténuation, sont créés et améliorés, en fonction des modèles de menace propres à l'organisation. Vous revoyez régulièrement (p. ex. annuellement) les modèles de menace existants pour vérifier qu’aucune nouvelle menace n’est devenue pertinente pour vos applications.

            Vous optimisez votre méthodologie de modélisation des menaces. Vous retenez les leçons tirées des modèles de menace et les utilisez pour améliorer votre méthodologie de modélisation des menaces. Vous examinez les catégories de menaces pertinentes à votre organisation et mettez à jour votre méthodologie en conséquence. De temps en temps, vous évaluez la qualité de vos modèles de menace de façon indépendante.

            Vous automatisez des parties de votre processus de modélisation des menaces avec des outils de modélisation des menaces. Vous intégrez vos outils de modélisation des menaces avec d'autres outils de sécurité, tels que les outils de vérification de la sécurité et les outils de suivi des risques. Vous étudiez la pratique de "modélisation des menaces en tant que code" pour intégrer des artefacts de modélisation des menaces au code de l'application.

        question: Revoyez-vous et mettez-vous à jour régulièrement la méthodologie de modélisation des menaces pour vos applications ?
        quality_criteria:
            - La méthodologie de modélisation des menaces prend en compte les retours d'expérience passés pour s'enrichir
            - Vous réexaminez régulièrement (par exemple annuellement) les modèles de menace existants pour vérifier qu'aucune nouvelle menace n'est pertinente pour vos applications
            - Vous automatisez des parties de votre processus de modélisation des menaces avec des outils de modélisation des menaces

        answers:
            - Non
            - Oui, mais la revue est ad-hoc
            - Oui, nous le revoyons régulièrement
            - Oui, nous le revoyons au moins une fois par an

---
