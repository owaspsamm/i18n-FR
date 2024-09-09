---
title: Génération Sécurisée
url: ./model/implementation/secure-build/
business_function: "Implémentation"
business_function_url: "implementation"
keywords: ["Business function", "Practice", "Génération Sécurisée"]
aliases:
    - /fr/model/I-SB
type: practice

practice_maturity_1_description: Le processus de génération est répétable et cohérent.
practice_maturity_2_description: Le processus de génération est optimisé et entièrement intégré dans le flux de travail.
practice_maturity_3_description: Le processus de génération permet d'éviter que les défauts connus ne pénètrent dans l'environnement de production.

stream_a: Processus de Génération

stream_a_maturity_1_activity: Créer une définition formelle du processus de génération afin qu'il devienne cohérent et répétable.
stream_a_maturity_2_activity: Automatisez votre chaîne de génération et sécurisez l'outillage utilisé. Ajoutez des vérifications de sécurité dans la chaîne de génération.
stream_a_maturity_3_activity: Définir des vérifications de sécurité obligatoires dans le processus de génération et s'assurer que la construction des artefacts non conformes échoue.

stream_b: Dépendances du Logiciel

stream_b_maturity_1_activity: Créer des enregistrements avec la nomenclature de vos applications et analysez-les opportunément.
stream_b_maturity_2_activity: Évaluer les dépendances utilisées et s'assurer d'une réaction rapide aux situations présentant un risque pour vos applications.
stream_b_maturity_3_activity: Analyser les dépendances utilisées quant aux problèmes de sécurité d'une manière comparable à votre propre code.
---

La pratique Génération Sécurisée (GS) souligne l'importance de construire des logiciels d'une façon standardisée et reproductible, et de le faire en utilisant des composants sécurisés, y compris les dépendances de logiciels tiers.

Le premier flux se concentre sur la suppression de toute subjectivité du processus de génération en recherchant une automatisation complète. Un pipeline de génération automatique peut inclure des vérifications de sécurité supplémentaires automatisées telles que le SAST et le DAST pour améliorer le niveau de confiance et identifier les régressions de sécurité en faisant échouer la génération, par exemple.

Le second flux reconnaît l'importance des dépendances logicielles dans les applications modernes. Il vise à les identifier et à suivre leur statut de sécurité afin de contenir l'impact de leur insécurité sur une application par ailleurs sécurisée. Dans une forme élaborée, les vérifications de sécurité pour les dépendances du logiciel sont identiques à celles de l'application elle-même.

