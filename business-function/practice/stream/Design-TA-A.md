---
title: Profil de risque de l'application
type: stream
url: ./model/design/threat-assessment/stream-a/
business_function: Conception
business_function_url: design
practice: Évaluation de la menace
stream: A
description: Conception / Évaluation de la menace
keywords: ["Business function", "Practice", "Conception", "Évaluation de la menace"]
aliases:
    - /fr/model/D-TA-A-1
    - /fr/model/D-TA-A-2
    - /fr/model/D-TA-A-3
    - /fr/model/D-TA-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Possibilité de classer les applications selon les risques
        activity: |
            Utilisez une méthode simple pour évaluer le risque associé à une application par application, tout en estimant l'impact potentiel que cela peut avoir sur l'entreprise en cas d'attaque. Pour y parvenir, évaluez l'impact d'une violation de la confidentialité, de l'intégrité et de la disponibilité des données ou du service. Envisagez d'utiliser un ensemble de 5 à 10 questions pour comprendre les caractéristiques importantes de l'application, par exemple si l'application traite des données financières, si elle est connectée à Internet ou si des données liées à la vie privée sont concernées. Le profil de risque de l'application vous indique si ces facteurs sont applicables et s'ils peuvent avoir un impact significatif sur l'organisation.

            Ensuite, utilisez un schéma pour classer les applications en fonction de ce risque. Un schéma simple et qualitatif (par exemple haut / moyen / bas) qui traduit ces caractéristiques en une valeur est souvent efficace. Il est important d'utiliser ces valeurs pour représenter et comparer le risque de différentes applications les unes par rapport aux autres. Les organisations matures utilisant fortement l'approche par les risques pourraient utiliser davantage de systèmes de risque quantitatifs. N’inventez pas un nouveau système de risque si votre organisation en a déjà un qui fonctionne bien.

        question: Classifiez-vous les applications en fonction du risque métier en fonction d'un ensemble de questions simple et prédéfini ?
        quality_criteria:
            - Une classification des risques validée existe
            - L'équipe applicative comprend la classification des risques
            - La classification des risques couvre les aspects critiques des risques commerciaux auxquels l'entreprise est confrontée
            - L'organisation a un inventaire des applications dans son périmètre

        answers:
            - Non
            - Oui, certains d'entre eux
            - Oui, au moins la moitié d'entre eux
            - Oui, la plupart ou tous

    level2:
        level: 2
        benefit: |
            Bien comprendre le niveau de risque de votre portefeuille d'applications
        activity: |
            Le but de cette activité est de bien comprendre le niveau de risque de toutes les applications au sein d'une organisation et de focaliser les efforts de vos activités d'assurance logicielle là où elles sont vraiment pertinentes.

            Du point de vue de l'évaluation des risques, le jeu de questions de base n'est pas suffisant pour bien évaluer le risques de l'ensemble des applications. Créez une manière uniforme et évolutive d'évaluer le risque d'une application (par exemple via leur impact sur la sécurité de l'information confidentialité, intégrite et disponibilité des données). Au delà de la sécurité, vous pouvez aussi évaluer le risque de l'application sur la vie privée. Comprenez les données que l'application traite et les potentielles violations de la vie privée. Enfin, étudiez l'impact que cette application peut avoir sur d'autres applications au sein de l'organisation (par exemple, l'application pourrait modifier des données qui ont été considérées comme étant en écriture seule dans un autre contexte). Evaluez toutes les applications au sein d'une organisation, y compris celles faisant partie de l'existant ou non-encore décommissionées.

            Tirez parti de l'analyse d'impact sur les affaires pour quantifier le risque applicatif et établir une classification. Un simple schéma qualitatif (tel que haut / moyen / bas) n'est pas suffisant pour gérer et comparer efficacement les applications au niveau de l'entreprise.

            En se basant sur ces éléments, les Officiers de Sécurité utilisent la classification pour définir le profile de risque afin de construire un inventaire centralisé de profils de risque et gérer la responsabilité. Cet inventaire donne aux propriétaires de produits, aux gestionnaires et aux autres parties prenantes de l'organisation une compréhension unique du niveau de risque d'une application dans le but d'assigner une priorité appropriée aux activités liées à la sécurité.

        question: Utilisez-vous des profils de risque d'applications centralisés et quantifiés pour évaluer les risques pour l'entreprise?
        quality_criteria:
            - Le profil de risque de l'application est conforme au niveau de risque défini par l'organisation
            - Le profil de risque de l'application couvre l'impact sur la sécurité et la vie privée
            - Vous validez la qualité du profil de risque manuellement et/ou automatiquement
            - Les profils de risque de l'application sont stockés dans un inventaire central

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Mise à jour rapide de la classification de l'application en cas de changement
        activity: |
            Le portefeuille d'applications d'une organisation évolue, tout comme les conditions et les contraintes dans lesquelles une application vit (p. ex. en fonction de la stratégie de l'entreprise). Revoyez périodiquement l’inventaire des risques pour garantir l’exactitude de l'évaluations des risques des différentes applications.

            Faites un examen périodique à l'échelle de l'entreprise. De plus, au fur et à mesure que votre entreprise mûrit dans le domaine de l'assurance logicielle, encouragez les équipes à s'interroger continuellement sur les changements de conditions qui pourraient affecter le profil de risque. Par exemple, une application interne peut devenir exposée sur Internet suite à une décision commerciale. Cela devrait inciter les équipes à refaire l'évaluation de risque et à mettre à jour le profil de risque de l'application en conséquence.

            Dans une mise en œuvre mûre de cette pratique, formez et informez continuellement les équipes sur les retours d'expérience et les bonnes pratiques d'évaluations des risques. Cela amène à une meilleure exécution et à une meilleure représentation du profil de risque de l'application.

        question: Examinez-vous et mettez-vous à jour régulièrement les profils de risque de vos applications?
        quality_criteria:
            - Le standard organisationnel pour le risque prend en compte les retours historiques afin d'améliorer la méthode d'évaluation
            - Des changements dans le contexte de l'application ou de l'entreprise déclenchent une revue des modèles de menace pertinents

        answers:
            - Non
            - Oui, sporadiquement
            - Oui, sur modification de l'application
            - Oui, au moins une fois par an

---
