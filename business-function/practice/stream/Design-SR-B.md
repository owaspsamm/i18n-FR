---
title: Sécurité du Fournisseur
type: stream
url: ./model/design/security-requirements/stream-b/
business_function: Conception
business_function_url: design
practice: Exigences de Sécurité
stream: B
description: Conception / Exigences de Sécurité
keywords: ["Business function", "Practice", "Conception", "Exigences de Sécurité"]
aliases:
    - /fr/model/D-SR-B-1
    - /fr/model/D-SR-B-2
    - /fr/model/D-SR-B-3
    - /fr/model/D-SR-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Transparence des pratiques de sécurité de vos fournisseurs de logiciels
        activity: |
            Les compétences et les habitudes en matière de sécurité des fournisseurs externes impliqués dans le développement de votre logiciel peuvent avoir un impact significatif sur la posture de sécurité du produit final. Par conséquent, il est important de connaître et d'évaluer vos fournisseurs sur ce point.

            Effectuez une évaluation de chacun de vos fournisseurs pour comprendre leurs forces et leurs faiblesses. Utilisez une liste de contrôle de base ou conduisez des entretiens pour examiner leurs pratiques et leurs comportements habituels. Cela vous donne une idée de la façon dont ils s'organisent et des éléments pour évaluer si vous avez besoin de prendre des mesures complémentaires pour atténuer des risques potentiels. Idéalement, parlez à différents intervenants au sein de l'organisation, voire même mettez en place une petite évaluation de maturité à cette fin. Des fournisseurs avec un fort niveau de maturité exécuteront leur propre programme d'assurance logicielle et seront en mesure de répondre à la plupart de vos questions. Si les fournisseurs ont des compétences faibles en matière de sécurité logicielle, discutez avec eux de la manière et dans quelle mesure ils comptent travailler sur cette question et évaluez si cela suffit pour votre organisation. Il se peut qu'un fournisseur de logiciel travaille sur un projet à faible risque, mais ce niveau de risque pourrait changer.

            Il est important que vos fournisseurs comprennent et s'alignent sur l'appétit du risque et soient en mesure de répondre à vos exigences dans ce domaine. Explicitez ce que vous attendez d'eux et discutez-en clairement.

        question: Les parties prenantes examinent-elles les collaborations avec les fournisseurs en ce qui concerne les exigences de sécurité et la méthodologie?
        quality_criteria:
            - Vous pensez à inclure des exigences spécifiques à la sécurité, aux activités et aux processus lors de la création de contrats avec vos fournisseurs
            - Un questionnaire concernant les fournisseurs est disponible et est utilisé pour l'évaluation des forces et des faiblesses de vos fournisseurs

        answers:
            - Non
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

    level2:
        level: 2
        benefit: |
            Des responsabilités de sécurité clairement définies chez vos fournisseurs de logiciels
        activity: |
            Améliorez votre confiance dans les aptitudes de vos fournisseurs en matière de sécurité logicielle. Discutez des responsabilités et des attentes concrètes de vos fournisseurs et de votre propre organisation et établissez un contrat avec le fournisseur. Les responsabilités peuvent être des exigences spécifiques de qualité ou des tâches particulières, et un service minimal peut être détaillé dans un accord de niveau de service (SLA). Un exemple d'exigence de qualité est qu'ils livreront des logiciels qui implémentent des protections contre le Top 10 de l'OWASP et, lors de la détection d'éventuels problèmes, ceux-ci seront résolus. Un exemple de tâche est qu'ils doivent effectuer une analyse statique de code en continu ou effectuer un test de pénétration indépendant avant une version majeure. L'accord prévoit les responsabilités et les couvertures au cas où un problème important arriverait.

            Une fois que vous avez mis cela en œuvre pour quelques fournisseurs, travaillez à un accord type pour tous les fournisseurs afin qu'il constitue la base de vos négociations. Vous pouvez vous écarter de cet accord standard au cas par cas, mais cela vous aidera à être sûr de ne pas négliger des sujets importants.

        question: Les fournisseurs remplissent-ils les responsabilités en matière de sécurité et les niveaux de qualité des accords de niveau de service définis par l'organisation?
        quality_criteria:
            - Vous discutez des exigences de sécurité avec le fournisseur lors de l'établissement des accords avec le fournisseur
            - Les accords avec les fournisseurs fournissent des directives spécifiques sur la correction des défauts de sécurité dans un délai convenu
            - L'organisation a un modèle d'accord des responsabilités et des niveaux de service pour les processus des fournisseurs de sécurité clés
            - Vous mesurez les indicateurs clés de performance

        answers:
            - Non
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

    level3:
        level: 3
        benefit: |
            Alignement des pratiques de développement de logiciels avec les fournisseurs pour limiter les risques de sécurité
        activity: |
            La meilleure façon de minimiser le risque de problèmes dans les logiciels est de s'aligner au maximum et de s'intégrer étroitement entre les différentes parties. Du point de vue des processus, cela signifie utiliser des paradigmes de développement similaires et introduire des jalons réguliers pour assurer un alignement correct et des progrès qualitatifs. Du point de vue des outils, cela pourrait signifier utiliser des environnements similaires de génération, de vérification et de déploiement, et partager d'autres outils de support (par ex. concernant les exigences, les outils d'architecture ou les dépôts de code).

            Si les fournisseurs ne peuvent pas atteindre les objectifs que vous avez fixés, mettez en œuvre des contrôles compensatoires afin que, globalement, les objectifs soient atteints. Exécutez des activités supplémentaires (par ex. la modélisation des menaces avant de commencer le cycle de mise en œuvre réelle) ou mettez en œuvre des outils supplémentaires (p. ex. d'analyse de bibliothèques tierces lors de l'intégration de solutions). Plus les fournisseurs s'écartent de vos exigences, plus l'effort de correction des écarts sera important.

        question: Les fournisseurs sont-ils alignés sur les contrôles de sécurité standards et les outils et processus de développement de logiciels que l'organisation utilise?
        quality_criteria:
            - Le fournisseur a un SDLC pour la sécurité qui inclut une génération sécurisée, un déploiement sécurisé, une gestion des défauts et une gestion des incidents qui s'alignent sur ceux utilisés dans votre organisation
            - Vous vérifiez que la solution répond aux objectifs de qualité et de sécurité avant chaque publication majeure
            - Lorsque des processus de vérification standard ne sont pas disponibles, vous utilisez des contrôles compensatoires tels que l'analyse de la composition du logiciel et des tests de pénétration indépendants

        answers:
            - Non
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

---
