---
title: Compréhension Approfondie
type: stream
url: ./model/verification/security-testing/stream-b/
business_function: Vérification
business_function_url: verification
practice: Tests de sécurité
stream: B
description: Vérification / Tests de sécurité
keywords: ["Business function", "Practice", "Vérification", "Tests de sécurité"]
aliases:
    - /fr/model/V-ST-B-1
    - /fr/model/V-ST-B-2
    - /fr/model/V-ST-B-3
    - /fr/model/V-ST-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Détection des vulnérabilités identifiables manuellement dans les composants critiques
        activity: |
            Effectuez des tests de sécurité manuels sélectifs, éventuellement en utilisant une combinaison d'outils d'analyse statique et dynamique pour guider ou cibler la revue, afin d'analyser plus en profondeur certaines parties de l'application comme le ferait un attaquant. Les outils automatisés sont efficaces pour trouver différents types de vulnérabilités, mais ne pourront jamais remplacer une revue manuelle par un expert.

            Les vulnérabilités au niveau du code dans les parties critiques pour la sécurité des logiciels peuvent avoir un impact considérablement accru, si bien que les équipes projet doivent revoir les modules à haut risque quant aux vulnérabilités courantes. Parmi les exemples courants de fonctionnalités à haut risque figurent les modules d'authentification, les endroits de mise en oeuvre du contrôle d'accès, les systèmes de gestion des sessions, les interfaces externes, les endroits pour la validation des entrées et les analyseurs de données. Les équipes peuvent combiner des métriques de niveau de code et des analyses automatisées ciblées pour déterminer où ils doivent cibler leurs efforts. Dans la pratique, l'activité peut prendre de nombreuses formes, y compris la programmation en binôme et l'évaluation par les pairs, des « poussées » de sécurité contraintes en temps impliquant toute l'équipe de développement, ou des revues spontanées indépendantes par des membres d'un groupe spécialisé dans la sécurité.

            Lors les cycles de développement où le code à haut risque est modifié et révisé, les gestionnaires du développement trient les résultats et priorisent de façon appropriée les mesures correctives en prenant en compte les commentaires des autres parties prenantes au projet.

        question: Examinez-vous manuellement la qualité de la sécurité des composants à haut risque sélectionnés?
        quality_criteria:
            - Des critères existent pour aider le réviseur à se concentrer sur les composants à haut risque
            - Le personnel qualifié mène les revues suivant des directives documentées
            - Vous traitez les résultats conformément à la politique de gestion des défauts de l'organisation

        answers:
            - "No"
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

    level2:
        level: 2
        benefit: |
            Compréhension de la résilience de l'application avec une perspective boîte noire
        activity: |
            En utilisant l'ensemble des cas de tests de sécurité identifiés pour chaque projet, effectuez des tests de pénétration manuels pour évaluer la performance du système dans chaque cas. Généralement, cela survient pendant la phase de test avant la livraison et inclut des tests de pénétration manuels statiques et dynamiques. Dans les cas où le logiciel ne peut pas être testé de manière réaliste en dehors de la production, l'utilisation de techniques telles que les déploiements bleu-vert ou les tests A/B peuvent permettre de rendre les tests de sécurité en production plus sûrs.

            Les cas de test de pénétration comprennent à la fois des tests spécifiques à l'application pour vérifier la robustesse de la logique métier et des tests de vulnérabilité courants pour vérifier la conception et l'implémentation. Une fois spécifiés, le personnel en charge de l'assurance qualité de la sécurité ou du développement peut exécuter les tests de sécurité. Le groupe central de sécurité logicielle supervise la première exécution des cas de tests de sécurité pour le bénéfice d'une équipe projet et apporte son aide au besoin et accompagne les champions de sécurité de l'équipe.

            De nombreuses organisations proposent des programmes de chasse aux bogues ("Bug Bounty") qui invitent les chercheurs en sécurité à trouver des vulnérabilités dans les applications et à les signaler de manière responsable en échange de primes. Cette approche permet aux organisations d’avoir accès à un plus grand ensemble de talents, en particulier à celles qui ne disposent pas de capacités internes suffisantes ou qui ont besoin d’une assurance supplémentaire.

            Avant la livraison ou le déploiement à grande échelle, les parties prenantes parcourent les résultats des tests de sécurité et acceptent les risques indiqués par des tests de sécurité négatifs au moment de la livraison. Établissez un calendrier concret pour corriger les écarts au fil du temps. Répandez la connaissance associée aux tests de sécurité manuels et aux résultats au sein de l'équipe de développement afin d'améliorer les connaissances et la sensibilisation en matière de sécurité au sein de l'organisation.

        question: Effectuez-vous des tests de pénétration pour vos applications à intervalles réguliers?
        quality_criteria:
            - Les tests d'intrusion utilisent des cas de test de sécurité spécifiques à l'application pour évaluer la sécurité
            - Les tests de pénétration recherchent des problèmes à la fois techniques et logiques dans l'application
            - Les parties prenantes examinent les résultats de test et les traitent selon la gestion de risque de l'organisation
            - Le personnel qualifié effectue des tests de pénétration

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Identification des problèmes de sécurité identifiables manuellement lors des étapes le plus possible en amont
        activity: |
            Intégres les tests de sécurité parallèlement à toutes les autres activités de développement, y compris l'analyse des exigences, la conception logicielle et sa construction.

            Avec la multiplication des outils de sécurité s'exécutant à chaque phase du développement, corriger les problèmes de sécurité à une étape donnée (par exemple pour les tests de pré-livraison) n’est plus approprié ou souhaitable. Les défauts de sécurité doivent être rapidement triés et leur résolution planifiée dans le cadre d'un compromis entre le risque et le coût de correction. Efforcez-vous continuellement de détecter les problèmes le plus tôt possible dans le cycle de vie de développement, via des tests automatisés spécifiques et à faible friction intégrés dans les outils de développement et le processus de génération, diminue le coût de correction et augmente ainsi la probabilité de résoudre rapidement les problèmes.

            Améliorez proactivement l'effort de test de sécurité intégré au processus de développement en propageant de façon adéquate les résultats d'autres activités de test de sécurité. Par exemple, si un test de pénétration de sécurité identifie des problèmes avec la gestion des sessions, toute modification de la gestion de session devrait déclencher des tests de sécurité explicites avant d'envoyer les changements en production.

            Les champions de la sécurité et le groupe central d'experts sur le logiciel sécurisé examinent en permanence les résultats des tests de sécurité automatisés et manuels durant le développement, y compris les résultats dans le cadre des formations de sensibilisation à la sécurité pour les équipes de développement. Intégrez les leçons tirées de l'expérience dans des manuels pour améliorer les tests de sécurité dans le cadre de la maturation de l'organisation. S'il y a des problèmes non résolus qui persistent en tant que risques acceptés pour la livraison, les parties prenantes et les gestionnaires du développement devraient travailler ensemble pour établir un calendrier concret pour les aborder.

        question: Utilisez-vous les résultats des tests de sécurité pour améliorer le cycle de vie de développement ?
        quality_criteria:
            - Vous utilisez les résultats d'autres activités de sécurité pour améliorer les tests de sécurité intégrés pendant le développement
            - Vous revoyez les résultats des tests et les incorporez dans les formations de sensibilisation à la sécurité et dans les manuels de tests de sécurité
            - Les parties prenantes revoient les résultats de test et les traitent selon la gestion des risques de l'organisation

        answers:
            - "No"
            - Oui, mais nous l'améliorons de façon ad-hoc
            - Oui, nous l'améliorons régulièrement
            - Oui, nous l'améliorons au moins une fois par an

---
