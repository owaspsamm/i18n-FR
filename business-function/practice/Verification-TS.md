---
title: Tests de sécurité
url: ./model/verification/security-testing/
business_function: "Vérification"
business_function_url: "verification"
keywords: ["Business function", "Practice", "Tests de sécurité"]
aliases:
    - /fr/model/V-ST
type: practice

practice_maturity_1_description: Effectuer des tests de sécurité (à la fois manuels et basés sur des outils) pour découvrir les défauts de sécurité.
practice_maturity_2_description: Rendre les tests de sécurité plus complets et plus efficaces au cours du développement grâce à l'automatisation complétée par des tests de pénétration manuels réguliers.
practice_maturity_3_description: Intégrer les tests de sécurité dans les processus de développement et de déploiement.

stream_a: Base de référence à l'échelle

stream_a_maturity_1_activity: Utiliser des outils de test de sécurité automatisés
stream_a_maturity_2_activity: Employer l'automatisation des tests de sécurité spécifiques à l'application
stream_a_maturity_3_activity: Intégrer les tests de sécurité automatisés dans le processus de génération et de déploiement

stream_b: Compréhension Approfondie

stream_b_maturity_1_activity: Effectuer des tests de sécurité manuels sur les composants à haut risque
stream_b_maturity_2_activity: Effectuer un test de pénétration manuel
stream_b_maturity_3_activity: Intégrer les tests de sécurité dans le processus de développement
---

La pratique des Tests de Sécurité (TS) tire parti du fait que, bien que les tests de sécurité automatisés soient rapides et adaptés à de nombreuses applications, des tests approfondis basés sur une bonne connaissance d'une application et de sa logique métier n'est souvent possible que par des tests de sécurité plus lents et manuels réalisés par un expert. Chaque flux a donc une approche propre.

Le premier flux se concentre sur l'établissement d'une référence de sécurité commune pour détecter automatiquement ce que l'on appelle les "fruits à portée de main". Personnalisez progressivement les tests automatisés pour chaque application et augmentez leur fréquence d'exécution pour détecter plus de bogues et de régressions plus tôt, aussi près que possible de leur introduction. Plus les processus automatisés peuvent détecter de bogues, plus les experts ont le temps d'utiliser leurs connaissances et leur créativité pour se concentrer sur des vecteurs d'attaque plus complexes et faire des tests approfondis sur l'application dans le second flux. Comme l'examen manuel est lent et difficile à mettre à l'échelle, les experts hiérarchisent les tests sur les composants en fonction de leurs risques, des changements récents pertinents ou des prochaines versions majeures. Les organisations peuvent également bénéficier d'expertise externe en participant à des programmes de primes à la défaillance détectée, par exemple.

Contrairement à la pratique de tests basée sur les exigences qui se concentre sur la vérification que les applications implémentent correctement leurs exigences, le but de cette pratique est de découvrir les faiblesses techniques et de logique métier dans l'application et de les rendre visibles à la direction et aux acteurs de l'entreprise, indépendamment des exigences.

