---
title: Formation et Sensibilisation
type: stream
url: ./model/governance/education-and-guidance/stream-a/
business_function: Gouvernance
business_function_url: governance
practice: Éducation & Orientation
stream: A
description: Gouvernance / Éducation & Orientation
keywords: ["Business function", "Practice", "Gouvernance", "Éducation & Orientation"]
aliases:
    - /fr/model/G-EG-A-1
    - /fr/model/G-EG-A-2
    - /fr/model/G-EG-A-3
    - /fr/model/G-EG-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Sensibilisation de base à la sécurité pour tous les employés impliqués
        activity: |
            Menez une formation de sensibilisation à la sécurité pour tous les rôles actuellement impliqués dans la gestion, le développement, le test ou l'audit du logiciel. L’objectif est d’accroître la sensibilisation aux menaces et aux risques liés à la sécurité des applications, aux bonnes pratiques en matière de sécurité et aux principes de conception de logiciels sécurisés. Développez la formation en interne ou achetez-là à une tierce partie. Idéalement, dispensez la formation en personne afin que les participants puissent avoir des discussions en tant qu'équipe, mais la formation par ordinateur (FAO) est également une option.

            Le contenu du cours devrait inclure une palette de sujets ayant trait à la sécurité des applications et au respect de la vie privée, tout en restant accessible à un public non-technique. Les concepts appropriés sont des principes de conception sécurisée incluant le moindre privilège, la défense en profondeur, la sécurité intégrée (sécurisée), la médiation complète, la gestion des sessions, la conception ouverte et l'acceptabilité psychologique. De plus, la formation devrait inclure des références à toutes les normes, politiques et procédures de l’organisation visant à l'amélioration de la sécurité des applications. Les vulnérabilités Top 10 de l'OWASP devraient être abordées à un niveau élevé.

            La formation est obligatoire pour tous les employés et les sous-traitants impliqués dans le développement de logiciels et doit faire intervenir une validation du stagiaire par signature pour démontrer la conformité à cette obligation. Il est conseillé d'intégrer des modes de formation innovants (comme la gamification) pour maximiser son efficacité et lutter contre la désensibilisation.

        question: Exigez-vous que les employés impliqués dans le développement d'applications suivent une formation SDLC ?
        quality_criteria:
            - Les formations sont répétables, cohérentes et disponibles pour toute personne impliquée dans le cycle de vie du développement logiciel
            - Les formations comprennent le dernier Top 10 de l'OWASP s'il est pertinent et incluent des concepts tels que le moindre privilège, la défense en profondeur, la défaillance sécurisée, la médiation entière, la gestion des sessions, la conception ouverte et l'acceptabilité psychologique
            - La formation nécessite une signature ou un accusé de réception de la part des participants
            - Vous avez mis à jour la formation au cours des 12 derniers mois
            - La formation est obligatoire lors du processus d'intégration des employés

        answers:
            - Non
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level2:
        level: 2
        benefit: |
            Employés à des postes pertinents formés en fonction de leur rôle spécifique
        activity: |
            Menez des formations sur la sécurité en présentiel ou en distanciel spécifiques aux rôles et aux technologies de l'organisation, en commençant par l'équipe de développement principale. L'organisation particularise la formation pour les gestionnaires de produit, les développeurs logiciels, les testeurs et les auditeurs de la sécurité en fonction des besoins techniques de chaque groupe.

            - les gestionnaires de produit sont formés sur les sujets en lien avec les fonctions d'affaire du SAMM et les pratiques de sécurité, en mettant l'accent sur les exigences de sécurité, la modélisation des menaces et le suivi des défauts.
            - les développeurs sont formés sur les normes de codage et les bonnes pratiques en lien avec les technologies avec lesquelles ils travaillent pour garantir que la formation bénéficie directement à la sécurité des applications. Ils devront avoir une bonne compréhension technique des vulnérabilités du Top 10 de l'OWASP ou des faiblesses similaires liées aux technologies et environnements utilisés (p. ex. mobiles) et des stratégies de résolution associées à chaque problème.
            - les testeurs sont formés aux différents outils de test et aux bonnes pratiques liées aux technologies présentes au sein de l'organisation, ainsi qu'aux outils qui permettent d'identifier les défauts de sécurité.
            - les auditeurs de la sécurité sont formés au cycle de vie de développement logiciel, aux mécanismes de sécurité des applications utilisés au sein de l'organisation et au process de soumission de défauts de sécurité en vue de leur correction.
            - les Champions de la sécurité sont formés aux sujets liés à la sécurité lors des différentes phases du SDLC. Ils reçoivent la même formation que les développeurs et les testeurs, mais reçoivent aussi des éléments quant à la compréhension de la modélisation des menaces et de la conception sécurisée, tout comme sur les outils de sécurité et les technologies qui peuvent être intégrés dans l'environnement de génération.

            Incluez tout le contenu de formation des activités du Niveau 1 de Maturité et tout le contenu supplémentaire lié à un rôle ou à une technologie. Eliminez les aspects inutiles de la formation. 

            Idéalement, identifiez un expert sur le sujet de chaque technologie pour aider à l'achat ou au développement du contenu de la formation et à sa mise à jour régulière. La formation doit contenir des démonstrations de l'exploitation de vulnérabilités en utilisant des applications intentionnellement vulnérables telles que WebGoat ou JuiceShop. Ajouter des informations sur les compromissions passées en tant qu'exemples de vulnérabilités et de stratégies de correction mises en place. Demandez à un pentesteur de contribuer avec des développements de démonstrations d'exploitation de vulnérabilités.

            La formation est obligatoire pour tous les employés et sous-traitants impliqués dans le développement de logiciels et comportent une phase de signature afin de pouvoir démontrer la conformité. Tant que faire se peut, la formation devrait comporter un test pour garantir la bonne compréhension, et pas seulement la conformité. Mettez à jour la formation et redéployez-là chaque année pour incorporer les changements dans l'organisation, la technologie et les tendances. Faites un sondage auprès des participants pour évaluer la qualité et la pertinence de la formation. Recueillez des suggestions ou toute autre information à propos de leur travail ou de leur environnement.

        question: La formation est-elle adaptée à des rôles donnés tels que les développeurs, les testeurs ou les champions de sécurité?
        quality_criteria:
            - La formation comprend tous les sujets de la maturité niveau 1 et ajoute des outils, des techniques et des démonstrations plus spécifiques
            - La formation est obligatoire pour tous les employés et les sous-traitants
            - La formation comprend les contributions des experts sur le sujet internes et des stagiaires
            - La formation comprend des démonstrations d'outils et de techniques développés en interne
            - Vous utilisez les commentaires pour améliorer la formation et la rendre plus pertinente pour l'avenir

        answers:
            - Non
            - Oui, pour une partie de la formation
            - Oui, pour au moins la moitié de la formation
            - Oui, pour la majeure partie ou la totalité de la formation

    level3:
        level: 3
        benefit: |
            S'assurer que tous les employés ont une connaissance adéquate de la sécurité avant de travailler sur des tâches critiques
        activity: |
            Mettez en place un programme de formation formel exigeant que toute personne impliquée dans le cycle de vie du développement logiciel suive une formation ciblée sur son rôle et propre aux technologies utilisées dans le cadre du processus d'intégration. Sur la base du niveau de criticité de l’application et du rôle de la personne, il est raisonnable d'envisager de restreindre l’accès jusqu’à ce que la formation d’intégration soit terminée. Tandis qu'il est possible que des modules soient fournis depuis l'extérieur, le programme est impulsé et géré en interne et comprend du contenu spécifique à l'organisation allant au-delà des bonnes pratiques de sécurité générale. Le curriculum du programme est bien défini, la participation est vérifiée et la compréhension et la compétence sont testées. La formation consiste en une combinaison de bonnes pratiques dans l’industrie et de normes internes à l’organisation, y compris une formation sur des systèmes spécifiques utilisés par l’organisation.

            En plus des questions directement liées à la sécurité, l'organisation ajoute d'autres normes au programme, comme celles touchant à la complexité du code, à la documentation du code, à la convention de nommage et autres disciplines connexes. Cette formation minimise les problèmes découlant des pratiques suivies par les employés en dehors de l'organisation et assure la continuité du style et de la compétence du code.

            Pour faciliter le suivi des progrès et la réussite à chaque module de formation, l'organisation a une plate-forme de gestion de la formation ou tout autre portail centralisé avec des fonctionnalités similaires. Les employés peuvent suivre leurs progrès et avoir accès à toutes les ressources de formation même après avoir terminé la formation initiale.

            Examinez les problèmes résultant des employés qui ne suivent pas les normes établies, les politiques, les procédures, ou les bonnes pratiques de sécurité au moins une fois par an pour évaluer l'efficacité de la formation et s'assurer qu'elle couvre toutes les questions pertinentes pour l'organisation. Mettre à jour la formation périodiquement et formez les employés à tous les changements et les carences les plus courantes en matière de sécurité.

        question: Avez-vous mis en place un système de gestion de l'apprentissage ou équivalent pour suivre les processus de formation et de certification des employés?
        quality_criteria:
            - Un système de gestion de l'apprentissage (LMS) est utilisé pour suivre les formations et les certifications
            - La formation est basée sur des normes, des politiques et des procédures internes
            - Vous utilisez des programmes de certification ou des preuves de présence pour donner accès aux systèmes de développement et aux ressources

        answers:
            - Non
            - Oui, pour une partie de la formation
            - Oui, pour au moins la moitié de la formation
            - Oui, pour la majeure partie ou la totalité de la formation

---
