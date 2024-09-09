---
title: Tests axés sur les exigences
url: ./model/verification/requirements-driven-testing/
business_function: "Vérification"
business_function_url: "verification"
keywords: ["Business function", "Practice", "Tests axés sur les exigences"]
aliases:
    - /fr/model/V-RT
type: practice

practice_maturity_1_description: Profiter des opportunités pour trouver des vulnérabilités simples et autres problèmes de sécurité.
practice_maturity_2_description: Effectuer une revue de l'implémentation pour découvrir les risques propres à l'application par rapport aux exigences de sécurité.
practice_maturity_3_description: Maintenir le niveau de sécurité de l'application après des corrections de bogues, des modifications ou pendant la maintenance.

stream_a: Vérification des contrôles

stream_a_maturity_1_activity: Tester les contrôles de sécurité logiciels
stream_a_maturity_2_activity: Dériver les cas de tests à partir des exigences de sécurité connues
stream_a_maturity_3_activity: Effectuer des tests de régression (avec des tests unitaires de sécurité)

stream_b: Tests de Mauvaise Utilisation / d'Abus

stream_b_maturity_1_activity: Effectuer des tests de fuzzing de sécurité
stream_b_maturity_2_activity: Créer et tester les cas d'abus et les défauts de la logique métier
stream_b_maturity_3_activity: Tests des dénis de service et de la sécurité aux limites
---

L'objectif de la pratique de Tests axés sur les Exigences (RT) est de s'assurer que les contrôles de sécurité implémentés fonctionnent comme prévu et répondent aux exigences de sécurité élicités dans le projet. Un ensemble de cas de test de sécurité et de régression est progressivement construit et régulièrement exécuté.

Un aspect clé de cette pratique est l'attention portée aux tests positifs et négatifs. Le premier vérifie que les contrôles de sécurité de l'application répondent aux exigences de sécurité élicitées et valident leur bon fonctionnement. Ces exigences sont typiquement fontionnelles par nature. Les tests négatifs traitent de la qualité de l'implémentation des contrôles de sécurité et ont pour but de détecter les défauts inattendus de conception et les bogues d'implémentation par des tests d'utilisation abusive et erronées. Dans ses formes les plus élaborées, la pratique favorise les tests de stress de sécurité, tels que les dénis de service, et s’efforce d’améliorer continuellement la sécurité des applications en automatisant constamment les tests unitaires de sécurité et en créant des tests de régression de sécurité pour tous les bogues identifiés et corrigés.

Bien que les deux pratiques de Tests axées sur les Exigences et les Tests de Sécurité concernent les tests de sécurité, la première se concentre sur la vérification de la bonne implémentation des exigences de sécurité, alors que cette dernière vise à découvrir les faiblesses de mise en œuvre technique dans une application, indépendamment des exigences.

