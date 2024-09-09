---
title: Mesurer et Améliorer
type: stream
url: ./model/governance/strategy-and-metrics/stream-b/
business_function: Gouvernance
business_function_url: governance
practice: Stratégie & Métriques
stream: B
description: Gouvernance / Stratégie & Métriques
keywords: ["Business function", "Practice", "Gouvernance", "Stratégie & Métriques"]
aliases:
    - /fr/model/G-SM-B-1
    - /fr/model/G-SM-B-2
    - /fr/model/G-SM-B-3
    - /fr/model/G-SM-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Des informations de premier niveau sur l'efficacité et la mise en œuvre de votre programme AppSec
        activity: |
            Définissez et documentez des métriques dans le but d'évaluer l'efficacité opérationnelle du programme de sécurité applicative. De cette manière, les améliorations sont mesurables et vous pouvez les utiliser pour sécuriser les besoins futurs en support et en budget pour le programme. Prenant en compte la nature dynamique de la plupart des environnements de développement, les métriques devraient comprendre des mesures dans les catégories suivantes :

                        * Les métriques sur les 'Actions' mesurent les actions faites sur la sécurité. Par exemple, les heures de formation, le temps passé à faire des revues de code et le nombre d'applications scannées quant aux vulnérabilités.
            * Les métriques sur les 'Résultats' mesurent les résultats des actions sur la sécurité. Des exemples sont : nombre de correctifs avec des défauts de sécurité significatifs et nombre d'incidents de sécurité impliquant des vulnérabilités dans une application.
            * Les métriques sur l''Environnement' rapportent des données sur l'environnement dans lequel les actions de sécurité surviennent. Par exemple, nombre d'applications ou de lignes de code mesurant la complexité ou la difficulté.

            Chaque métrique prise isolément est utile dans un but donné, mais la combinaison de deux ou trois métriques peut aider à expliquer les pics dans les tendances des métriques. Par exemple, un pic dans le nombre total de vulnérabilités peut être causé par le fait que l'organisation a incorporé plusieurs nouvelles applications qui n'ont pas été prises en compte précédemment par les mécanismes de sécurité applicatives en place. Par ailleurs, une augmentation dans la métrique 'Environnement' sans augmentation parallèle des métriques 'Actions' ou 'Résultats' pourrait être un indicateur d'un programme de sécurité mûr et efficace.

            Lors de l'identification des métriques, il est toujours recommandé de se tenir aux métriques qui remplissent plusieurs critères :

                        * Mesurées de façon cohérente,
            * Peu chères à mesurer,
            * Exprimées sous la forme de nombres cardinaux ou de pourcentage,
            * Exprimées en tant qu'unité de mesure.

            Documentez les métriques et incluez des descriptions des méthodes les meilleures et les plus efficaces pour collecter des données, aussi bien que les méthodes recommandées pour combiner des mesures données pour produire des métriques parlantes. Par exemple, le nombre d'applications et le nombre total de défauts dans l'ensemble des applications ne sont peut-être pas utiles en tant que tels mais, lorsqu'on les combine en tant que nombre de défauts impactants de niveau élevé par application, ils fournissent une métrique bien plus exploitable.

        question: Utilisez-vous un ensemble de métriques pour mesurer l'efficacité et l'efficience du programme de sécurité applicative à travers les applications?
        quality_criteria:
            - Vous documentez chaque métrique avec notamment la description des sources, le périmètre de mesure et des conseils sur la façon de l'utiliser pour expliquer les tendances de la sécurité de l'application
            - Les métriques incluent les mesures des efforts, des résultats et des catégories de mesure de l'environnement
            - La plupart des métriques sont souvent mesurées, faciles ou peu coûteuses à rassembler et exprimées en nombre cardinal ou en pourcentage
            - Les équipes de sécurité des applications et de développement publient des métriques

        answers:
            - "No"
            - Oui, pour une catégorie de métriques
            - Oui, pour deux catégories de métriques
            - Oui, pour les trois catégories de métriques

    level2:
        level: 2
        benefit: |
            Transparence sur la performance de votre programme AppSec
        activity: |
            Une fois que l'organisation a défini ses métriques de sécurité applicative, collectez suffisamment d'informations pour établir des objectifs réalistes. Testez les métriques identifiées pour vous assurer que vous pouvez collecter des données de façon cohérente et efficace sur une courte période. Après la période d'essai initiale, l'organisation devrait disposer de suffisamment d'informations pour s'engager à respecter les buts et les objectifs exprimés au moyen d'indicateurs clés de performance (ICP).

            Bien que plusieurs mesures soient utiles pour surveiller le programme de sécurité de l'information et son efficacité, les indicateurs clés de performance font partie des métriques les plus significatives et efficaces. Éliminez la volatilité, qui est courante dans les environnements de développement d'applications, des ICP pour réduire les risques d'indicateurs défavorables résultant de mesures isolées temporaires ou trompeuses. Basez les ICP sur les métriques considérées comme précieuses non seulement pour les professionnels de la sécurité de l'information, mais aussi pour les personnes responsables du succès global de l'application et la direction de l’organisation. Voyez les ICP comme des indicateurs définitifs de la réussite de l'ensemble du programme et considérez-les comme applicables.

            Documentez entièrement les ICP et distribuez-les aux équipes qui contribuent au succès du programme ainsi qu'au management de l'organisation. Idéalement, incluez une brève explication des sources d'information de chaque ICP et de la signification si les chiffres sont hauts ou bas. Incluez les objectifs à court et à long terme et des fourchettes pour les mesures inacceptables nécessitant une intervention immédiate. Partagez les plans d’action avec les équipes de sécurité des applications et de développement des applications afin d’assurer une transparence totale dans la compréhension des objectifs et des buts de l’organisation.

        question: Avez-vous défini les indicateurs clés de perfomance (KPI) à partir des métriques disponibles sur la sécurité applicatives?
        quality_criteria:
            - Vous avez défini les indicateurs clés de performance après avoir recueilli suffisamment d'informations pour établir des objectifs réalistes
            - Vous avez développé des KPI validés par la direction et les équipes responsables de la sécurité des applications
            - Des KPI sont disponibles pour les équipes en charge des applications et incluent des seuils d'acceptabilité et des conseils dans le cas où les équipes auraient à prendre des mesures
            - Le succès du programme de sécurité applicative est sans ambigüité selon les KPIs définis

        answers:
            - "No"
            - Oui, pour certains métriques
            - Oui, pour au moins la moitié des métriques
            - Oui, pour la plupart ou toutes les métriques

    level3:
        level: 3
        benefit: |
            Amélioration continue de votre programme en fonction des résultats
        activity: |
            Définissez des lignes directrices pour influencer le programme de Sécurité Applicative en vous basant sur des ICP et d'autres métriques de sécurité applicative. Ces lignes directrices combinent la maturité du processus et des procédures de développement d'application avec différentes métriques afin de rendre le programme plus efficace. Les exemples suivants montrent la relation entre les mesures et les façons de faire évoluer et d'améliorer la sécurité dans les applications :

                        * Se concentrer sur la maturité du cycle de vie de développement réduit le coût relatif par défaut en appliquant la sécurité de manière proactive.
            * Surveiller l'équilibre entre les métriques concernant les actions, les résultats et l'environnement améliore l'efficacité du programme et permet de justifier toute automatisation supplémentaire et autres méthodes d'amélioration des réferences plancher de la sécurité globale de l'application.
            * Les pratiques individualisées de sécurité peuvent fournir des indicateurs de réussite ou d'échec des initiatives individualisées de sécurité applicative.
            * Les métriques sur les actions aident à garantir que les initiatives sur la sécurité des applications sont dirigés vers les technologies et les disciplines les plus pertinentes et les plus importantes.

            Lors de la définition de la stratégie globale concernant les métriques, gardez à l'esprit l'objectif final et définissez quelles décisions peuvent être prises à la suite de modifications des Indicateurs Clés de Performance et des métriques dès que possible, afin d'aider à guider le développement des métriques.

        question: Mettez-vous à jour la stratégie et la feuille de route de sécurité des applications en fonction des indicateurs de sécurité des applications et des indicateurs clés de performance?
        quality_criteria:
            - Vous réexaminez les indicateurs clés de performance au moins une fois par an par rapport à leur efficacité et leur opérationnalité
            - Les indicateurs clés de performance et les métriques de sécurité applicative sont la cause de la plupart des changements de la stratégie de sécurité applicative

        answers:
            - "No"
            - Oui, mais la revue est ad-hoc
            - Oui, nous le revoyons régulièrement
            - Oui, nous le revoyons au moins une fois par an

---
