---
title: Tests de Mauvaise Utilisation / d'Abus
type: stream
url: ./model/verification/requirements-driven-testing/stream-b/
business_function: Vérification
business_function_url: verification
practice: Tests axés sur les exigences
stream: B
description: Vérification / Tests axés sur les exigences
keywords: ["Business function", "Practice", "Vérification", "Tests axés sur les exigences"]
aliases:
    - /fr/model/V-RT-B-1
    - /fr/model/V-RT-B-2
    - /fr/model/V-RT-B-3
    - /fr/model/V-RT-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Aperçu du comportement de vos applications lorsque elles traitent des entrées inattendues
        activity: |
            Effectuez des tests en envoyant des données aléatoires ou malformées au sujet du test dans le but de le faire planter. Le test de génération aléatoire ou Fuzzing est une technique de test du logiciel en boîte noire qui consiste à trouver des bogues d'implémentation à l'aide de l'injection de données malformées ou semi-malformées de manière automatique. Faites au moins un fuzzing minimal pour découvrir les vulnérabilités liées aux paramètres d'entrée principaux de l'application.

            L'avantage des tests de fuzzing est sa simplicité de conception et son absence de supposition sur le comportement du système. Son approche stochastique permet la découverte de bugs que les humains ou des tests structurés manqueraient souvent. C'est aussi l'un des rares moyens d'évaluer la qualité d'un système fermé (comme un téléphone SIP). La simplicité du fuzzing est contrebalancée par la difficulté de détecter et de caractériser les plantages avec précision. Préférez les outils et les environnements de fuzzing existants afin de tirer parti des outils associés.

        question: Testez-vous les applications en utilisant des techniques de génération aléatoire?
        quality_criteria:
            - Les tests couvrent la plupart ou l'ensemble des paramètres d'entrée de l'application
            - Vous enregistrez et inspectez tous les plantages de l'application dans le but d'évaluer l'impact sur la sécurité en fonction de vos capacités

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Détection des défauts de la logique métier de l'application
        activity: |
            Les cas de mauvaise utilisation et d'utilisation abusive décrivent des scénarios d'utilisation non intentionnée ou malveillante de l'application, explicitant la manière dont un attaquant pourrait faire. Créez des cas de mauvaise utilisation et d’utilisation abusive pour mal utiliser ou exploiter les faiblesses des contrôles dans les fonctionnalités du logiciel dans le but d'attaquer une application. Utilisez des modèles de cas d'abus pour une application afin de permettre l'identification de tests de sécurité concrets qui exploitent directement ou indirectement les scénarios d'abus.

            L'abus de fonctionnalité, parfois appelé "attaque logique métier", est lié à la conception et la mise en œuvre des fonctionnalités de l'application. Un exemple est l'utilisation d'un canal de réinitialisation de mot de passe pour énumérer les comptes. Dans le cadre des tests de logique métier, identifiez les règles métier qui sont importantes pour l'application et faites des expérimentations afin de vérifier si l'application met en oeuvre correctement la règle métier. Par exemple, sur une application de transaction boursière, est-ce que l'attaquant est autorisé à démarrer une transaction au début de la journée et à verrouiller un prix, à maintenir la transaction ouverte jusqu'à la fin de la journée, puis accomplir la vente si le cours de l'action a augmenté ou l'annuler si le prix a baissé?

        question: Créez-vous des cas d'abus à partir des exigences fonctionnelles et utilisez-vous celles-ci pour piloter les tests de sécurité?
        quality_criteria:
            - Les fonctionnalités métiers importantes ont des cas d'abus correspondants
            - Vous construisez des cas d'abus de la sécurité autour d'acteurs types pertinents ayant des motivations et des caractéristiques bien définies
            - Vous capturez les faiblesses identifiées comme des exigences de sécurité

        answers:
            - "No"
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

    level3:
        level: 3
        benefit: |
            Transparence de la résilience envers les attaques par déni de service
        activity: |
            Les applications sont particulièrement susceptibles de subir des attaques par déni de service. Effectuez des tests de résistance de sécurité sur elles par déni de service dans des conditions contrôlées, de préférence dans les environnements d'acceptation utilisateurs.

            Les outils de test de charge génèrent du trafic artificiel, vous permettant de tester les performances de l'application sous une charge élevée. Un test important est le nombre de requêtes par seconde qu'une application peut gérer tout en respectant ses exigences de performance. Tester à partir d'une seule adresse IP est toujours utile car cela donne une indication du nombre de requêtes qu'un attaquant doit générer pour avoir un impact sur l'application.

            Les attaques par déni de service entraînent généralement un amoindrissement ou un épuisement des ressources de l'application. Pour déterminer si des ressources peuvent être victimes d'un déni de service, analysez chaque ressource de l'application pour voir comment elle peut être épuisée. Hiérarchisez les actions qu'un utilisateur non authentifié peut accomplir. Complétez l'ensemble des tests de déni de service par des tests de contraintes de sécurité pour effectuer des actions ou créer les conditions qui causent des retards, des interruptions ou des défaillances de l'application en train d'être testée.

        question: Effectuez-vous des tests de déni de service et de mise sous tension de la sécurité?
        quality_criteria:
            - Les tests sous contraintes ciblent les ressources spécifiques de l'application (par ex : éviter l'épuisement de la quantité de mémoire en évitant d'utiliser de grandes quantités de données lors d'une session utilisateur)
            - Vous concevez des tests autour d'acteurs pertinents ayant des caractéristiques bien définies (connaissances, ressources)
            - Vous ajoutez les résultats aux pratiques de conception

        answers:
            - "No"
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

---
