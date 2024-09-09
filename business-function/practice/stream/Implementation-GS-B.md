---
title: Dépendances du Logiciel
type: stream
url: ./model/implementation/secure-build/stream-b/
business_function: Implémentation
business_function_url: implementation
practice: Génération Sécurisée
stream: B
description: Implémentation / Génération Sécurisée
keywords: ["Business function", "Practice", "Implémentation", "Génération Sécurisée"]
aliases:
    - /fr/model/I-SB-B-1
    - /fr/model/I-SB-B-2
    - /fr/model/I-SB-B-3
    - /fr/model/I-SB-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Informations disponibles sur les problèmes de sécurité connus dans les dépendances
        activity: |
            Gardez un enregistrement de toutes les dépendances utilisées dans l'environnement de production cible. Cela est parfois appelé "nomenclature". Gardez en tête que différents composants de l'application peuvent utiliser des dépendances complètement différentes. Par exemple, si le logiciel est une application web, couvrez à la fois le code côté serveur et les scripts côté client. Lors de la construction de ces enregistrements, considérez les différents endroits où les dépendances peuvent être spécifiées comme les fichiers de configuration, le répertoire du projet sur le disque, un outil de gestion des paquets ou le code réel (par ex. via un EDI qui prend en charge la liste des dépendances).

            Rassemblez les informations suivantes sur chaque dépendance :

            * quand elle est utilisée ou référencée,
            * la version utilisée,
            * la licence,
            * les informations liées à sa source (lien vers le référentiel, nom de l'auteur, etc.),
            * la prise en charge et le statut de maintenance de la dépendance.

            Vérifiez les enregistrements pour découvrir les dépendances avec des vulnérabilités connues et mettez-les à jour ou remplacez-les en conséquence.

        question: Avez-vous une bonne connaissance des dépendances sur lesquelles votre logiciel est construit?
        quality_criteria:
            - Vous avez une nomenclature (BOM) à jour pour chaque application
            - Vous pouvez rapidement savoir quelles applications sont affectées par une CVE particulière
            - Vous avez analysé, traité et documenté les dépendances au moins une fois au cours des trois derniers mois

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Transparence totale des problèmes de sécurité connus dans les dépendances
        activity: |
            Évaluez les dépendances utilisées et établissez une liste des dépendances acceptables approuvées pour utilisation dans un projet, par une équipe ou l'organisation au sens large selon un ensemble de critères définis.

            Introduisez un référentiel central concernant les dépendances à partir duquel tout logiciel peut être construit.

            Revoyez régulièrement les dépendances utilisées pour vous assurer que :

            * elles restent correctement sous licence,
            * aucune vulnérabilité connue et significative impactant vos applications sont présentes,
            * la dépendance est toujours activement prise en charge et maintenue,
            * vous utilisez une version à jour,
            * il y a une raison valable d'inclure la dépendance.

            Réagissez rapidement et de manière appropriée aux non-conformités en les traitant comme des défauts. Envisagez d'utiliser un outil automatisé pour rechercher les dépendances vulnérables et d'affecter les problèmes identifiés aux équipes de développement concernées.

        question: Est-ce que vous gérez le risque associé à une dépendance à une tierce partie par un processus formel ?
        quality_criteria:
            - Vous gardez une liste des dépendances approuvées qui répondent à des critères prédéfinis
            - Vous évaluez automatiquement les dépendances par rapport aux nouvelles CVE et avertissez le personnel responsable
            - Vous détectez automatiquement les changements de licence et alertez automatiquement lorsqu'il existe un impact éventuel sur le droit d'utilisation
            - Vous suivez et alertez sur l'utilisation des dépendances non maintenues
            - Vous détectez et supprimez du logiciel de manière fiable les dépendances inutiles

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Gestion des problèmes de sécurité dans les dépendances comparable à celles de votre propre code
        activity: |
            Maintenez une liste blanche des dépendances approuvées et de leurs versions et assurez-vous que le processus de génération échoue lorsqu'il détecte la présence de dépendances ne se trouvant pas dans la liste. Incluez un processus de validation par signature pour gérer les exceptions à cette règle si besoin.

            Effectuez les activités de vérification de sécurité envers les dépendances de la liste blanche d'une manière comparable à celle faite sur les applications cibles elles-mêmes (par ex. en utilisant le SAST et en analysant les dépendances transitoires). Assurez-vous que ces vérifications visent également à identifier les portes dérobées ou les oeufs de Pâques éventuellement présents dans les dépendances. Établissez des processus de divulgation de vulnérabilités avec les auteurs des dépendances, y compris des CNS pour corriger les problèmes. Dans le cas où la mise en place de CNS serait impossible (par ex. pour les dépendances en source ouverte), assurez-vous que les cas les plus probables sont gérables et que vous êtes en mesure de mettre en œuvre des mesures compensatoires en temps opportun. Implémentez des tests de régression pour les corrections des problèmes identifiés.

            Suivez tous les problèmes identifiés et leur état à l'aide de votre système de suivi des défauts. Intégrez votre chaîne de génération avec ce système pour entraîner l'échec de la génération chaque fois que les dépendances incluses contiennent des problèmes au-dessus d'un niveau de criticité défini.

        question: Empêchez-vous la génération de logiciels si des vulnérabilités dans les dépendances apparaissent?
        quality_criteria:
            - Votre système de génération est connecté à un système permettant de suivre les risques des dépendances provenant de tiers et causant l'échec de la génération à moins que la vulnérabilité ne soit évaluée comme étant un faux positif ou que le risque soit explicitement accepté
            - Vous scannez vos dépendances à l'aide d'un outil d'analyse statique
            - Vous rapportez les problèmes identifiés aux auteurs des dépendances en utilisant un processus de divulgation responsable établi
            - L'utilisation d'une nouvelle dépendance non évaluée pour des risques de sécurité entraîne l'échec de la génération

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
